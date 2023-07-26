# Comparing `tmp/async_poe_client-0.2.3.tar.gz` & `tmp/async_poe_client-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_poe_client-0.2.3.tar", max compression
+gzip compressed data, was "async_poe_client-0.2.4.tar", max compression
```

## Comparing `async_poe_client-0.2.3.tar` & `async_poe_client-0.2.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0       32 2023-07-22 14:46:24.800780 async_poe_client-0.2.3/async_poe_client/__init__.py
--rw-r--r--   0        0        0    49330 2023-07-26 07:15:35.882949 async_poe_client-0.2.3/async_poe_client/client.py
--rw-r--r--   0        0        0     1145 2023-07-19 06:18:30.461961 async_poe_client-0.2.3/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql
--rw-r--r--   0        0        0      536 2023-07-19 06:18:30.461961 async_poe_client-0.2.3/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql
--rw-r--r--   0        0        0      187 2023-07-19 06:18:30.461961 async_poe_client-0.2.3/async_poe_client/poe_graphql/AutoSubscriptionMutation.graphql
--rw-r--r--   0        0        0      701 2023-07-22 07:43:55.501987 async_poe_client-0.2.3/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql
--rw-r--r--   0        0        0      105 2023-07-19 06:18:30.461961 async_poe_client-0.2.3/async_poe_client/poe_graphql/BioFragment.graphql
--rw-r--r--   0        0        0      169 2023-07-22 05:55:18.261809 async_poe_client-0.2.3/async_poe_client/poe_graphql/BotDeletionButton_poeBotDelete_Mutation.graphql
--rw-r--r--   0        0        0       78 2023-07-19 06:18:30.462960 async_poe_client-0.2.3/async_poe_client/poe_graphql/ChatAddedSubscription.graphql
--rw-r--r--   0        0        0      106 2023-07-19 06:18:30.462960 async_poe_client-0.2.3/async_poe_client/poe_graphql/ChatFragment.graphql
--rw-r--r--   0        0        0    12084 2023-07-19 06:18:30.462960 async_poe_client-0.2.3/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql
--rw-r--r--   0        0        0      712 2023-07-19 06:18:30.462960 async_poe_client-0.2.3/async_poe_client/poe_graphql/ChatPaginationQuery.graphql
--rw-r--r--   0        0        0      162 2023-07-19 06:18:30.462960 async_poe_client-0.2.3/async_poe_client/poe_graphql/ChatViewQuery.graphql
--rw-r--r--   0        0        0      167 2023-07-19 06:18:30.463987 async_poe_client-0.2.3/async_poe_client/poe_graphql/DeleteHumanMessagesMutation.graphql
--rw-r--r--   0        0        0      129 2023-07-19 06:18:30.463987 async_poe_client-0.2.3/async_poe_client/poe_graphql/DeleteMessageMutation.graphql
--rw-r--r--   0        0        0      154 2023-07-19 06:18:30.463987 async_poe_client-0.2.3/async_poe_client/poe_graphql/DeleteUserMessagesMutation.graphql
--rw-r--r--   0        0        0     1148 2023-07-19 06:18:30.463987 async_poe_client-0.2.3/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql
--rw-r--r--   0        0        0      111 2023-07-19 06:18:30.463987 async_poe_client-0.2.3/async_poe_client/poe_graphql/HandleFragment.graphql
--rw-r--r--   0        0        0      319 2023-07-19 06:18:30.464960 async_poe_client-0.2.3/async_poe_client/poe_graphql/LoginWithVerificationCodeMutation.graphql
--rw-r--r--   0        0        0     1985 2023-07-19 06:18:30.464960 async_poe_client-0.2.3/async_poe_client/poe_graphql/MessageAddedSubscription.graphql
--rw-r--r--   0        0        0      141 2023-07-19 06:18:30.464960 async_poe_client-0.2.3/async_poe_client/poe_graphql/MessageDeletedSubscription.graphql
--rw-r--r--   0        0        0      207 2023-07-19 06:18:30.464960 async_poe_client-0.2.3/async_poe_client/poe_graphql/MessageFragment.graphql
--rw-r--r--   0        0        0      152 2023-07-19 06:18:30.464960 async_poe_client-0.2.3/async_poe_client/poe_graphql/MessageRemoveVoteMutation.graphql
--rw-r--r--   0        0        0      223 2023-07-19 06:18:30.465959 async_poe_client-0.2.3/async_poe_client/poe_graphql/MessageSetVoteMutation.graphql
--rw-r--r--   0        0        0     1832 2023-07-19 06:18:30.465959 async_poe_client-0.2.3/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql
--rw-r--r--   0        0        0      968 2023-07-19 06:18:30.465959 async_poe_client-0.2.3/async_poe_client/poe_graphql/PoeBotEditMutation.graphql
--rw-r--r--   0        0        0      963 2023-07-19 06:18:30.465959 async_poe_client-0.2.3/async_poe_client/poe_graphql/SendMessageMutation.graphql
--rw-r--r--   0        0        0      275 2023-07-19 06:18:30.465959 async_poe_client-0.2.3/async_poe_client/poe_graphql/SendVerificationCodeForLoginMutation.graphql
--rw-r--r--   0        0        0      222 2023-07-19 06:18:30.465959 async_poe_client-0.2.3/async_poe_client/poe_graphql/ShareMessagesMutation.graphql
--rw-r--r--   0        0        0      321 2023-07-19 06:18:30.466959 async_poe_client-0.2.3/async_poe_client/poe_graphql/SignupWithVerificationCodeMutation.graphql
--rw-r--r--   0        0        0      166 2023-07-19 06:18:30.466959 async_poe_client-0.2.3/async_poe_client/poe_graphql/StaleChatUpdateMutation.graphql
--rw-r--r--   0        0        0      170 2023-07-19 06:18:30.466959 async_poe_client-0.2.3/async_poe_client/poe_graphql/SubscriptionsMutation.graphql
--rw-r--r--   0        0        0       98 2023-07-19 06:18:30.466959 async_poe_client-0.2.3/async_poe_client/poe_graphql/SummarizePlainPostQuery.graphql
--rw-r--r--   0        0        0      150 2023-07-19 06:18:30.466959 async_poe_client-0.2.3/async_poe_client/poe_graphql/SummarizeQuotePostQuery.graphql
--rw-r--r--   0        0        0      183 2023-07-19 06:18:30.466959 async_poe_client-0.2.3/async_poe_client/poe_graphql/SummarizeSharePostQuery.graphql
--rw-r--r--   0        0        0      382 2023-07-19 06:18:30.467959 async_poe_client-0.2.3/async_poe_client/poe_graphql/UserSnippetFragment.graphql
--rw-r--r--   0        0        0      421 2023-07-19 06:18:30.467959 async_poe_client-0.2.3/async_poe_client/poe_graphql/ViewerInfoQuery.graphql
--rw-r--r--   0        0        0     1068 2023-07-19 06:18:30.467959 async_poe_client-0.2.3/async_poe_client/poe_graphql/ViewerStateFragment.graphql
--rw-r--r--   0        0        0      700 2023-07-19 06:18:30.467959 async_poe_client-0.2.3/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql
--rw-r--r--   0        0        0       53 2023-07-23 07:11:13.271223 async_poe_client-0.2.3/async_poe_client/requirements.txt
--rw-r--r--   0        0        0     2473 2023-07-26 03:41:48.482615 async_poe_client-0.2.3/async_poe_client/util.py
--rw-r--r--   0        0        0      467 2023-07-26 07:15:58.538162 async_poe_client-0.2.3/pyproject.toml
--rw-r--r--   0        0        0    17721 2023-07-25 06:52:50.946100 async_poe_client-0.2.3/README.md
--rw-r--r--   0        0        0    18004 1970-01-01 00:00:00.000000 async_poe_client-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       32 2023-07-22 14:46:24.800780 async_poe_client-0.2.4/async_poe_client/__init__.py
+-rw-r--r--   0        0        0    49508 2023-07-26 08:01:19.085533 async_poe_client-0.2.4/async_poe_client/client.py
+-rw-r--r--   0        0        0     1145 2023-07-19 06:18:30.461961 async_poe_client-0.2.4/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql
+-rw-r--r--   0        0        0      536 2023-07-19 06:18:30.461961 async_poe_client-0.2.4/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql
+-rw-r--r--   0        0        0      187 2023-07-19 06:18:30.461961 async_poe_client-0.2.4/async_poe_client/poe_graphql/AutoSubscriptionMutation.graphql
+-rw-r--r--   0        0        0      701 2023-07-22 07:43:55.501987 async_poe_client-0.2.4/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql
+-rw-r--r--   0        0        0      105 2023-07-19 06:18:30.461961 async_poe_client-0.2.4/async_poe_client/poe_graphql/BioFragment.graphql
+-rw-r--r--   0        0        0      169 2023-07-22 05:55:18.261809 async_poe_client-0.2.4/async_poe_client/poe_graphql/BotDeletionButton_poeBotDelete_Mutation.graphql
+-rw-r--r--   0        0        0       78 2023-07-19 06:18:30.462960 async_poe_client-0.2.4/async_poe_client/poe_graphql/ChatAddedSubscription.graphql
+-rw-r--r--   0        0        0      106 2023-07-19 06:18:30.462960 async_poe_client-0.2.4/async_poe_client/poe_graphql/ChatFragment.graphql
+-rw-r--r--   0        0        0    12084 2023-07-19 06:18:30.462960 async_poe_client-0.2.4/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql
+-rw-r--r--   0        0        0      712 2023-07-19 06:18:30.462960 async_poe_client-0.2.4/async_poe_client/poe_graphql/ChatPaginationQuery.graphql
+-rw-r--r--   0        0        0      162 2023-07-19 06:18:30.462960 async_poe_client-0.2.4/async_poe_client/poe_graphql/ChatViewQuery.graphql
+-rw-r--r--   0        0        0      167 2023-07-19 06:18:30.463987 async_poe_client-0.2.4/async_poe_client/poe_graphql/DeleteHumanMessagesMutation.graphql
+-rw-r--r--   0        0        0      129 2023-07-19 06:18:30.463987 async_poe_client-0.2.4/async_poe_client/poe_graphql/DeleteMessageMutation.graphql
+-rw-r--r--   0        0        0      154 2023-07-19 06:18:30.463987 async_poe_client-0.2.4/async_poe_client/poe_graphql/DeleteUserMessagesMutation.graphql
+-rw-r--r--   0        0        0     1148 2023-07-19 06:18:30.463987 async_poe_client-0.2.4/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql
+-rw-r--r--   0        0        0      111 2023-07-19 06:18:30.463987 async_poe_client-0.2.4/async_poe_client/poe_graphql/HandleFragment.graphql
+-rw-r--r--   0        0        0      319 2023-07-19 06:18:30.464960 async_poe_client-0.2.4/async_poe_client/poe_graphql/LoginWithVerificationCodeMutation.graphql
+-rw-r--r--   0        0        0     1985 2023-07-19 06:18:30.464960 async_poe_client-0.2.4/async_poe_client/poe_graphql/MessageAddedSubscription.graphql
+-rw-r--r--   0        0        0      141 2023-07-19 06:18:30.464960 async_poe_client-0.2.4/async_poe_client/poe_graphql/MessageDeletedSubscription.graphql
+-rw-r--r--   0        0        0      207 2023-07-19 06:18:30.464960 async_poe_client-0.2.4/async_poe_client/poe_graphql/MessageFragment.graphql
+-rw-r--r--   0        0        0      152 2023-07-19 06:18:30.464960 async_poe_client-0.2.4/async_poe_client/poe_graphql/MessageRemoveVoteMutation.graphql
+-rw-r--r--   0        0        0      223 2023-07-19 06:18:30.465959 async_poe_client-0.2.4/async_poe_client/poe_graphql/MessageSetVoteMutation.graphql
+-rw-r--r--   0        0        0     1832 2023-07-19 06:18:30.465959 async_poe_client-0.2.4/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql
+-rw-r--r--   0        0        0      968 2023-07-19 06:18:30.465959 async_poe_client-0.2.4/async_poe_client/poe_graphql/PoeBotEditMutation.graphql
+-rw-r--r--   0        0        0      963 2023-07-19 06:18:30.465959 async_poe_client-0.2.4/async_poe_client/poe_graphql/SendMessageMutation.graphql
+-rw-r--r--   0        0        0      275 2023-07-19 06:18:30.465959 async_poe_client-0.2.4/async_poe_client/poe_graphql/SendVerificationCodeForLoginMutation.graphql
+-rw-r--r--   0        0        0      222 2023-07-19 06:18:30.465959 async_poe_client-0.2.4/async_poe_client/poe_graphql/ShareMessagesMutation.graphql
+-rw-r--r--   0        0        0      321 2023-07-19 06:18:30.466959 async_poe_client-0.2.4/async_poe_client/poe_graphql/SignupWithVerificationCodeMutation.graphql
+-rw-r--r--   0        0        0      166 2023-07-19 06:18:30.466959 async_poe_client-0.2.4/async_poe_client/poe_graphql/StaleChatUpdateMutation.graphql
+-rw-r--r--   0        0        0      170 2023-07-19 06:18:30.466959 async_poe_client-0.2.4/async_poe_client/poe_graphql/SubscriptionsMutation.graphql
+-rw-r--r--   0        0        0       98 2023-07-19 06:18:30.466959 async_poe_client-0.2.4/async_poe_client/poe_graphql/SummarizePlainPostQuery.graphql
+-rw-r--r--   0        0        0      150 2023-07-19 06:18:30.466959 async_poe_client-0.2.4/async_poe_client/poe_graphql/SummarizeQuotePostQuery.graphql
+-rw-r--r--   0        0        0      183 2023-07-19 06:18:30.466959 async_poe_client-0.2.4/async_poe_client/poe_graphql/SummarizeSharePostQuery.graphql
+-rw-r--r--   0        0        0      382 2023-07-19 06:18:30.467959 async_poe_client-0.2.4/async_poe_client/poe_graphql/UserSnippetFragment.graphql
+-rw-r--r--   0        0        0      421 2023-07-19 06:18:30.467959 async_poe_client-0.2.4/async_poe_client/poe_graphql/ViewerInfoQuery.graphql
+-rw-r--r--   0        0        0     1068 2023-07-19 06:18:30.467959 async_poe_client-0.2.4/async_poe_client/poe_graphql/ViewerStateFragment.graphql
+-rw-r--r--   0        0        0      700 2023-07-19 06:18:30.467959 async_poe_client-0.2.4/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql
+-rw-r--r--   0        0        0       53 2023-07-23 07:11:13.271223 async_poe_client-0.2.4/async_poe_client/requirements.txt
+-rw-r--r--   0        0        0     2473 2023-07-26 03:41:48.482615 async_poe_client-0.2.4/async_poe_client/util.py
+-rw-r--r--   0        0        0      467 2023-07-26 08:06:10.677490 async_poe_client-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0    17726 2023-07-26 07:16:52.145077 async_poe_client-0.2.4/README.md
+-rw-r--r--   0        0        0    18009 1970-01-01 00:00:00.000000 async_poe_client-0.2.4/PKG-INFO
```

### Comparing `async_poe_client-0.2.3/async_poe_client/client.py` & `async_poe_client-0.2.4/async_poe_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -793,15 +793,15 @@
                         if retry == 0:
                             raise Exception(
                                 "Failed to get answer form poe too many times:No Reply!"
                             )
                         continue
                     message = json.loads(raw_data["messages"][-1])["payload"]["data"][
                         "messageAdded"
-                    ]  # noqa: E501
+                    ]
                     if message["messageId"] > human_message_id:
                         plain_text = message["text"][len(last_text) :]
                         last_text = message["text"]
                         if (
                             self.bots[url_botname]["defaultBotObject"][
                                 "hasSuggestedReplies"
                             ]
@@ -835,15 +835,17 @@
                                     if not yield_header:
                                         yield_header = True
                                         yield "\n\nSuggested Reply:"
                                     for suggest in message["suggestedReplies"]:
                                         if suggest not in suggestion_list:
                                             yield f"\n{str(len(suggestion_list)+1)}:{suggest}"
                                             suggestion_list.append(suggest)
+                                        self.bots[url_botname]["Suggestion"] = suggestion_list
                                     if len(suggestion_list) >= 3:
+                                        self.bots[url_botname]["Suggestion"] = suggestion_list
                                         break
                             else:
                                 retry -= 1
                                 await asyncio.sleep(1)
                                 continue
                         else:
                             if plain_text:
```

### Comparing `async_poe_client-0.2.3/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql` & `async_poe_client-0.2.4/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.2.3/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql` & `async_poe_client-0.2.4/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.2.3/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql` & `async_poe_client-0.2.4/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.2.3/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql` & `async_poe_client-0.2.4/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.2.3/async_poe_client/poe_graphql/ChatPaginationQuery.graphql` & `async_poe_client-0.2.4/async_poe_client/poe_graphql/ChatPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.2.3/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql` & `async_poe_client-0.2.4/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.2.3/async_poe_client/poe_graphql/MessageAddedSubscription.graphql` & `async_poe_client-0.2.4/async_poe_client/poe_graphql/MessageAddedSubscription.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.2.3/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql` & `async_poe_client-0.2.4/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.2.3/async_poe_client/poe_graphql/PoeBotEditMutation.graphql` & `async_poe_client-0.2.4/async_poe_client/poe_graphql/PoeBotEditMutation.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.2.3/async_poe_client/poe_graphql/SendMessageMutation.graphql` & `async_poe_client-0.2.4/async_poe_client/poe_graphql/SendMessageMutation.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.2.3/async_poe_client/poe_graphql/ViewerStateFragment.graphql` & `async_poe_client-0.2.4/async_poe_client/poe_graphql/ViewerStateFragment.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.2.3/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql` & `async_poe_client-0.2.4/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.2.3/async_poe_client/util.py` & `async_poe_client-0.2.4/async_poe_client/util.py`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.2.3/README.md` & `async_poe_client-0.2.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
        obtained using get_available_bots always equals url_botname.
 - 2.How to obtain p_b and formkey? ->  
     1. To obtain p_b: Open poe.com, press F12 to open the debugging tool, then select the application. You can find the value of p_b in the cookies.  
     2. To obtain formkey: Open poe.com, press F12 to open the debugging tool, then select Network. After chatting with a bot, you can see the gqlpost network request. Within the request headers, there is a separate key-value pair for the formkey.
 
 ## Step 1: Import the library and create a Poe_Client object
 
-If you don't formkey to the Poe_Client, you need to install node.js for generate form key.
+If you don't pass formkey to the Poe_Client, you need to install node.js for generate form key.
 Here is the download link.[node.js](https://nodejs.org/en)
 
 Before you can use any functionality of the `Poe_Client` library, you first need to import the library and create
 a `Poe_Client` object. You need to pass the `p_b token` and `formkey` to the constructor of `Poe_Client`, and then call the `create`
 method to initialize it. Here is an example:
 
 ```python
```

### Comparing `async_poe_client-0.2.3/PKG-INFO` & `async_poe_client-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-poe-client
-Version: 0.2.3
+Version: 0.2.4
 Summary: A stable, fast and convenient async client for poe.com
 Author: canxin
 Author-email: 1969730106@qq.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -61,15 +61,15 @@
        obtained using get_available_bots always equals url_botname.
 - 2.How to obtain p_b and formkey? ->  
     1. To obtain p_b: Open poe.com, press F12 to open the debugging tool, then select the application. You can find the value of p_b in the cookies.  
     2. To obtain formkey: Open poe.com, press F12 to open the debugging tool, then select Network. After chatting with a bot, you can see the gqlpost network request. Within the request headers, there is a separate key-value pair for the formkey.
 
 ## Step 1: Import the library and create a Poe_Client object
 
-If you don't formkey to the Poe_Client, you need to install node.js for generate form key.
+If you don't pass formkey to the Poe_Client, you need to install node.js for generate form key.
 Here is the download link.[node.js](https://nodejs.org/en)
 
 Before you can use any functionality of the `Poe_Client` library, you first need to import the library and create
 a `Poe_Client` object. You need to pass the `p_b token` and `formkey` to the constructor of `Poe_Client`, and then call the `create`
 method to initialize it. Here is an example:
 
 ```python
```

