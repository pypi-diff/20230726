# Comparing `tmp/lrmatrix-0.1.3-py3-none-any.whl.zip` & `tmp/lrmatrix-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 29694 bytes, number of entries: 11
+Zip file size: 29980 bytes, number of entries: 11
 -rw-rw-r--  2.0 unx        0 b- defN 22-Nov-06 01:37 lrmatrix/__init__.py
 -rw-rw-r--  2.0 unx     8023 b- defN 23-Apr-02 22:39 lrmatrix/explanation.py
 -rw-rw-r--  2.0 unx    36769 b- defN 23-Apr-08 01:08 lrmatrix/matrixdraw.py
--rw-rw-r--  2.0 unx    38264 b- defN 23-Apr-03 14:05 lrmatrix/matrixmanager.py
+-rw-rw-r--  2.0 unx    39837 b- defN 23-Jul-26 00:21 lrmatrix/matrixmanager.py
 -rw-rw-r--  2.0 unx    28650 b- defN 23-Apr-08 01:50 lrmatrix/rulevectormatrix.py
 -rw-rw-r--  2.0 unx     1043 b- defN 22-Feb-25 12:46 lrmatrix/treevis.py
--rw-rw-r--  2.0 unx    15137 b- defN 23-Apr-08 03:06 lrmatrix-0.1.3.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     3598 b- defN 23-Apr-08 03:06 lrmatrix-0.1.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-08 03:06 lrmatrix-0.1.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-Apr-08 03:06 lrmatrix-0.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      874 b- defN 23-Apr-08 03:06 lrmatrix-0.1.3.dist-info/RECORD
-11 files, 132459 bytes uncompressed, 28226 bytes compressed:  78.7%
+-rw-rw-r--  2.0 unx    15137 b- defN 23-Jul-26 02:07 lrmatrix-0.1.4.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     3598 b- defN 23-Jul-26 02:07 lrmatrix-0.1.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-26 02:07 lrmatrix-0.1.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jul-26 02:07 lrmatrix-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      874 b- defN 23-Jul-26 02:07 lrmatrix-0.1.4.dist-info/RECORD
+11 files, 134032 bytes uncompressed, 28512 bytes compressed:  78.7%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: lrmatrix/rulevectormatrix.py
 Comment: 
 
 Filename: lrmatrix/treevis.py
 Comment: 
 
-Filename: lrmatrix-0.1.3.dist-info/LICENSE.txt
+Filename: lrmatrix-0.1.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: lrmatrix-0.1.3.dist-info/METADATA
+Filename: lrmatrix-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: lrmatrix-0.1.3.dist-info/WHEEL
+Filename: lrmatrix-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: lrmatrix-0.1.3.dist-info/top_level.txt
+Filename: lrmatrix-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: lrmatrix-0.1.3.dist-info/RECORD
+Filename: lrmatrix-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lrmatrix/matrixmanager.py

```diff
@@ -536,93 +536,128 @@
 
 
 
 
 
 
 	def calc_feature_importances( self, mode = 'supp' ):
+		
+		self.feature_importances_ = np.zeros( self.n_features_ )
+
+		self.feature_importances_ = self.__calc_feature_importances( mode = mode, rules = None )
+		
+
+
+
+
+
+
+
+
 
+	
+	def __calc_feature_importances( self, mode = 'supp', rules = None, class_mode = 'diff' ):
 		
+
 		if self._verbose > 0: print( 'starting feature importances calculation ...' )
 
 
-		self.feature_importances_ = np.zeros( self.n_features_ )
+		feature_importances = np.zeros( self.n_features_ )
+
+		if rules is None: rules = np.arange( self.n_rules_ )
 
 
 		if mode == 'supp':
 
 
 			# 2018 A Decision Rule Based Approach to Generational Feature Selection - Wieslaw Paja, using as measure of quality the rule coverage
 			
 			for f in self.features_used_:
 					
 				a = f * 2
 				b = a + 1
 
-				rules = self.rules_matrix_[ :, a ].nonzero()[ 0 ].tolist()
-				rules.extend( self.rules_matrix_[ :, b ].nonzero()[ 0 ].tolist() )
-				rules = np.unique( np.array( rules ) )
+				rules_subset = self.rules_matrix_[ rules, a ].nonzero()[ 0 ].tolist()
+				rules_subset.extend( self.rules_matrix_[ rules, b ].nonzero()[ 0 ].tolist() )
+				rules_subset = np.unique( np.array( rules_subset ) )
 
-				for r in rules:
-					self.feature_importances_[ f ] += self.rules_matrix_[ r, self.SUPPORT ]
+				for r in rules_subset:
+					feature_importances[ f ] += self.rules_matrix_[ r, self.SUPPORT ]
 
-			self.feature_importances_ /= self.feature_importances_.sum()
+			feature_importances /= feature_importances.sum()
 
 
 		elif mode == 'hdiff':
 
 
 			for f in self.features_used_:
 
 				if self._verbose > 1: print( 'calculating importance on feature ', f )			
 				
 				f_importance = 0
 
-				for r_1 in range( 0, self.n_rules_ ):
+				for r_1 in range( 0, rules.shape[ 0 ] ):
+
+					rule1 = rules[ r_1 ]
+
+					for r_2 in range( r_1 + 1, rules.shape[ 0 ] ):
 
-					for r_2 in range( r_1 + 1, self.n_rules_ ):
+						rule2 = rules[ r_2 ]
 
 						hist_diffs = 0
 						
-						
-						if self.rules_matrix_[ r_1, self.CLASS ] != self.rules_matrix_[ r_2, self.CLASS ]:
+						calc = False
+
+						if ( class_mode == 'diff' ) and ( self.rules_matrix_[ rule1, self.CLASS ] != self.rules_matrix_[ rule2, self.CLASS ] ):
+							# class_mode as 'diff' represents the original calculation, that is considering only rules from different classes
+							calc = True
+
+						elif( class_mode == 'all' ):
+							# for the case where local importance is being calculated over rules from the same class
+							calc = True 
+
+
+						if ( calc == True ):
 
 							for b in range( f * self.bins_, f * self.bins_ + self.bins_ ):
 
-								if ( self.histograms_matrix_[ r_1 + self.n_classes_, b ] == 0 ) or ( self.histograms_matrix_[ r_2 + self.n_classes_, b ] == 0 ):
+								if ( self.histograms_matrix_[ rule1 + self.n_classes_, b ] == 0 ) or ( self.histograms_matrix_[ rule2 + self.n_classes_, b ] == 0 ):
 
-									hist_diffs += ( self.histograms_matrix_[ r_1 + self.n_classes_, b ] + self.histograms_matrix_[ r_2 + self.n_classes_, b ] )
+									hist_diffs += ( self.histograms_matrix_[ rule1 + self.n_classes_, b ] + self.histograms_matrix_[ rule2 + self.n_classes_, b ] )
 
 						
-						# the highest value that hist_diff can have is 2.0, that is all instances from r_1 and r_2 belong to different bins
+						# the highest value that hist_diff can have is 2.0, that is all instances from rule1 and rule2 belong to different bins
 						hist_diffs /= 2
-						# the highest value that min can have is 1.0, when r_1 and r_2 support all instances from their classes (support = 1.0)
-						hist_diffs *= min( self.rules_matrix_[ r_1, self.SUPPORT ], self.rules_matrix_[ r_2, self.SUPPORT ] )
+						# the highest value that min can have is 1.0, when rule1 and rule2 support all instances from their classes (support = 1.0)
+						hist_diffs *= min( self.rules_matrix_[ rule1, self.SUPPORT ], self.rules_matrix_[ rule2, self.SUPPORT ] )
 
 						if f_importance < hist_diffs: f_importance = hist_diffs
 
 
-				self.feature_importances_ [ f ] = f_importance
+				feature_importances [ f ] = f_importance
 
 
-			self.feature_importances_ /= self.feature_importances_.sum()
+			feature_importances /= feature_importances.sum()
 
 		
 		if self._verbose > 0: print( 'feature importances calculation done' )
 
 
+		return feature_importances
+
+	
+
 
 
 
 
 
 
 
 
-	
 	def __order_by_link( self, matrix, method, optimal_ordering ):
 
 		try:
 
 			link_mat = hierarchy.linkage( matrix, method = method, optimal_ordering = optimal_ordering )
 			indexes = hierarchy.leaves_list( link_mat )			
 			return indexes
@@ -687,26 +722,21 @@
 
 
 
 
 
 
 
-	def order_cols( self, cols, criteria, rows,
-
-		link_method = 'complete', link_optimal_ordering = True ):
+	def order_cols( self, cols, criteria, rows, link_method = 'complete', link_optimal_ordering = True, local_feature_importances = None ):
 
 		
 		if criteria == 'importance':
-			indexes = np.argsort( self.feature_importances_[ cols ] )[ ::-1 ]
+			if local_feature_importances is None: indexes = np.argsort( self.feature_importances_[ cols ] )[ ::-1 ]
+			else: indexes = np.argsort( local_feature_importances[ cols ] )[ ::-1 ]
 			return indexes
-			# if self.feature_importances_ is not None:
-			# 	indexes = np.argsort( self.feature_importances_[ cols ] )[ ::-1 ]
-			# 	return indexes
-			# else: return cols
 
 		elif criteria == 'range-link':
 			rc_sel = np.ix_( rows, cols )
 			indexes = self.__order_by_link( self.rules_ranges_diameter_[ rc_sel ].toarray().T, link_method, link_optimal_ordering )
 			return indexes
 
 
@@ -715,15 +745,15 @@
 
 
 
 	
 
 
 
-	def explanation( self, exp_type = 'global', rules = None, x_k = None, X_s = None, r_model = None, r_node = None, r_support_min = None,  r_certainty_min = None, r_pvalue_max = None, r_class = None, r_order = 'raw', f_importance_min = None, f_order = 'raw', r_label_format = 'auto', data_coverage_max = None, info_text = None, show_rule_certainty = 'auto', show_rule_fisher_pvalue = 'auto', show_rule_data_coverage = 'auto', show_feature_importance = 'auto', show_feature_range = False, show_global_histograms = 'auto', draw_distribution = 'auto', show_info_text = True ):
+	def explanation( self, exp_type = 'global', rules = None, x_k = None, X_s = None, r_model = None, r_node = None, r_support_min = None,  r_certainty_min = None, r_pvalue_max = None, r_class = None, r_order = 'raw', f_importance_min = None, f_order = 'raw', r_label_format = 'auto', data_coverage_max = None, info_text = None, local_feature_importance_mode = None, show_rule_certainty = 'auto', show_rule_fisher_pvalue = 'auto', show_rule_data_coverage = 'auto', show_feature_importance = 'auto', show_feature_range = False, show_global_histograms = 'auto', draw_distribution = 'auto', show_info_text = True ):
 
 		
 		if self.goal_ == 'model':
 
 			if show_feature_importance == 'auto': show_feature_importance = True
 			if show_rule_data_coverage == 'auto': show_rule_data_coverage = False
 			if show_global_histograms == 'auto': show_global_histograms = False
@@ -879,26 +909,41 @@
 
 
 		if ( r_model is not None ) or ( r_node is not None ) or ( r_support_min is not None ) or ( r_certainty_min is not None ) or ( r_pvalue_max is not None ) or ( r_class is not None ): 
 			features = super()._get_features_used( rules )
 
 
 
+		feature_importances = self.feature_importances_.copy()
+
+		if local_feature_importance_mode is not None: 
+			feature_importances = self.__calc_feature_importances( mode = local_feature_importance_mode, rules = rules, class_mode = 'all' )
+
+
+
 		if f_importance_min is not None:	
 
-			indexes = np.argwhere( self.feature_importances_[ features ] >= f_importance_min )[ :, 0 ]
+			indexes = np.argwhere( feature_importances[ features ] >= f_importance_min )[ :, 0 ]
 			features = features[ indexes ]
 
 			info_text += 'importance >= ' + str( f_importance_min ) + '\n'
 
 
 			
 
 		if ( f_order != 'raw' ) and ( len( features ) != 1 ):
-			indexes = self.order_cols( features, f_order, rules )
+
+			if local_feature_importance_mode is not None:
+
+				indexes = self.order_cols( features, f_order, rules, local_feature_importances = feature_importances )
+
+			else:
+
+				indexes = self.order_cols( features, f_order, rules )
+
 			features = features[ indexes ]
 
 
 	
 
 		if ( r_order != 'raw' ) and ( len( rules ) != 1 ):
 
@@ -927,22 +972,34 @@
 			
 			rules = rules[ indexes ]
 			if old_rules is not None: old_rules = old_rules[ indexes ]
 			cumulative_data_coverage = cumulative_data_coverage[ indexes ]
 			info_text += 'data coverage <= ' + str( data_coverage_max ) + '\n'
 
 
+			if local_feature_importance_mode is not None:
+				feature_importances = self.__calc_feature_importances( mode = local_feature_importance_mode, rules = rules, class_mode = 'all' )
+
+
 			features = super()._get_features_used( rules )
 			if f_order != 'raw':
-				indexes = self.order_cols( features, f_order, rules )
+
+				if local_feature_importance_mode is not None:
+
+					indexes = self.order_cols( features, f_order, rules, local_feature_importances = feature_importances )
+
+				else: 
+
+					indexes = self.order_cols( features, f_order, rules )
+
 				features = features[ indexes ]
 
 
 			if f_importance_min is not None:
-				indexes = np.argwhere( self.feature_importances_[ features ] >= f_importance_min )[ :, 0 ]
+				indexes = np.argwhere( feature_importances[ features ] >= f_importance_min )[ :, 0 ]
 				features = features[ indexes ]		
 
 
 
 
 		features_used_ab = super()._to_features_ab( features )
 		rc_sel = np.ix_( rules, features_used_ab )
@@ -1041,22 +1098,22 @@
 
 			if x_k is not None: label += str( np.round( x_k[ f ], decimals = self.precision_ ) ) + ' | '				
 
 			label += self.feature_names_[ f ]
 
 			if show_feature_range: label += ' [' + str( np.round( self.feature_values_min_[ f ], decimals = self.precision_ ) ) + ', ' + str( np.round( self.feature_values_max_[ f ], decimals = self.precision_ ) ) + ']'
 
-			if show_feature_importance: label += ' | ' + str( np.round( self.feature_importances_[ f ], decimals = self.precision_ ) )
+			if show_feature_importance: label += ' | ' + str( np.round( feature_importances[ f ], decimals = self.precision_ ) )
 
 			feature_labels.append( label )
 
 		if x_k is not None: x_k = x_k[ features ]
 
 
-		if show_feature_importance: feature_importances = self.feature_importances_[ features ]
+		if show_feature_importance: feature_importances = feature_importances[ features ]
 		else: feature_importances = None
 
 
 		info_text += '\nrules ' + str( rules.shape[ 0 ] ) + '\nby ' + r_order + '\n'
 		info_text += '\nfeatures ' + str( features.shape[ 0 ] ) + '\nby ' + f_order
 
 		if show_info_text == False: info_text = ''
@@ -1343,15 +1400,15 @@
 			except Exception as e:
 				print( e )
 
 
 			try:
 
 				if self._verbose > 0: print( 'loading histograms_matrix_ ...' )
-				self.histograms_matrix_ = ssp.lil_matrix( np.loadtxt( file_name + '-histograms_matrix_.csv', delimiter = ';' ), dtype = int )
+				self.histograms_matrix_ = ssp.lil_matrix( np.loadtxt( file_name + '-histograms_matrix_.csv', delimiter = ';' ), dtype = np.float64 )
 				if self._verbose > 0: print( 'histograms_matrix_ loaded' )
 
 			except Exception as e:
 				print( e )
 
 		else:
```

## Comparing `lrmatrix-0.1.3.dist-info/LICENSE.txt` & `lrmatrix-0.1.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `lrmatrix-0.1.3.dist-info/METADATA` & `lrmatrix-0.1.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lrmatrix
-Version: 0.1.3
+Version: 0.1.4
 Summary: Logic Rules Matrix package to support the ExMatrix and VAX methods.
 Home-page: https://gitlab.com/popolinneto/
 Author: Mario Popolin Neto
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International
 Platform: UNKNOWN
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: OS Independent
```

## Comparing `lrmatrix-0.1.3.dist-info/RECORD` & `lrmatrix-0.1.4.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 lrmatrix/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lrmatrix/explanation.py,sha256=QLRubAeqX81I7djQbQT7rqQk8IJf7pkSGXnOV14bqc8,8023
 lrmatrix/matrixdraw.py,sha256=Vag_5NYvyRHZony9821RCNj6ntlpvtB_93dCPCscR4g,36769
-lrmatrix/matrixmanager.py,sha256=wNhNZXNjFE3rskuJLJNebyGqroCsL06KlCb9T3ZxXjE,38264
+lrmatrix/matrixmanager.py,sha256=k0xHViTj8z_Cw3IPFFNWGeddcQCidZhCElU8hPYSODE,39837
 lrmatrix/rulevectormatrix.py,sha256=VYakQxaXTLzIvhmy1H0BGVpBpYDspIbURYQbAVi-kcs,28650
 lrmatrix/treevis.py,sha256=DvVFBXbTFmY-p8-Z8yvC_zuH04rUKehn168HH93aAzQ,1043
-lrmatrix-0.1.3.dist-info/LICENSE.txt,sha256=jKiAwnpX2WQ78HnB_IEyAVxidGRr8pLIbUB9Zr0_WPU,15137
-lrmatrix-0.1.3.dist-info/METADATA,sha256=QwLqly8NtTK9YCLAqrFpbXIhGRrHxJM5af_kpnBdnWg,3598
-lrmatrix-0.1.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-lrmatrix-0.1.3.dist-info/top_level.txt,sha256=5F1NJYgyQUN8SeGGOtEp3BDd0H2QBYDBeRQm1B5feTk,9
-lrmatrix-0.1.3.dist-info/RECORD,,
+lrmatrix-0.1.4.dist-info/LICENSE.txt,sha256=jKiAwnpX2WQ78HnB_IEyAVxidGRr8pLIbUB9Zr0_WPU,15137
+lrmatrix-0.1.4.dist-info/METADATA,sha256=0aWpf2N_pjHEIXxwUUBnqOgA4rvAR-9rz-a1rtBcb9E,3598
+lrmatrix-0.1.4.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+lrmatrix-0.1.4.dist-info/top_level.txt,sha256=5F1NJYgyQUN8SeGGOtEp3BDd0H2QBYDBeRQm1B5feTk,9
+lrmatrix-0.1.4.dist-info/RECORD,,
```

