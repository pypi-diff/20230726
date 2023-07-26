# Comparing `tmp/fabrictestbed-1.6.0b6.tar.gz` & `tmp/fabrictestbed-1.6.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-1.6.0b6.tar", last modified: Fri Jul 21 15:33:30 2023, max compression
+gzip compressed data, was "fabrictestbed-1.6.0b7.tar", last modified: Wed Jul 26 18:51:01 2023, max compression
```

## Comparing `fabrictestbed-1.6.0b6.tar` & `fabrictestbed-1.6.0b7.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1806 2023-07-13 18:40:33.774250 fabrictestbed-1.6.0b6/.gitignore
--rw-r--r--   0        0        0     1071 2023-07-13 18:40:33.774483 fabrictestbed-1.6.0b6/LICENSE
--rw-r--r--   0        0        0       24 2023-07-13 18:40:33.774598 fabrictestbed-1.6.0b6/MANIFEST.in
--rw-r--r--   0        0        0     5603 2023-07-13 18:40:33.774750 fabrictestbed-1.6.0b6/README.md
--rw-r--r--   0        0        0       24 2023-07-21 15:33:15.467809 fabrictestbed-1.6.0b6/fabrictestbed/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 18:40:33.775067 fabrictestbed-1.6.0b6/fabrictestbed/cli/__init__.py
--rw-r--r--   0        0        0    18169 2023-07-13 18:40:33.775336 fabrictestbed-1.6.0b6/fabrictestbed/cli/cli.py
--rw-r--r--   0        0        0     1452 2023-07-13 18:40:33.775647 fabrictestbed-1.6.0b6/fabrictestbed/cli/exceptions.py
--rw-r--r--   0        0        0     1914 2023-07-13 18:40:33.775918 fabrictestbed-1.6.0b6/fabrictestbed/slice_editor/__init__.py
--rw-r--r--   0        0        0      201 2023-07-13 18:40:33.776101 fabrictestbed-1.6.0b6/fabrictestbed/slice_manager/__init__.py
--rw-r--r--   0        0        0    20678 2023-07-21 15:24:31.637226 fabrictestbed-1.6.0b6/fabrictestbed/slice_manager/slice_manager.py
--rw-r--r--   0        0        0        0 2023-07-13 18:40:33.776619 fabrictestbed-1.6.0b6/fabrictestbed/util/__init__.py
--rw-r--r--   0        0        0     1452 2023-07-13 18:40:33.776762 fabrictestbed-1.6.0b6/fabrictestbed/util/constants.py
--rw-r--r--   0        0        0     1073 2023-07-21 15:33:10.715168 fabrictestbed-1.6.0b6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-13 18:40:33.777184 fabrictestbed-1.6.0b6/test/__init__.py
--rw-r--r--   0        0        0     2210 2023-07-13 18:40:33.777415 fabrictestbed-1.6.0b6/test/test_cli.py
--rw-r--r--   0        0        0     6536 1970-01-01 00:00:00.000000 fabrictestbed-1.6.0b6/PKG-INFO
+-rw-r--r--   0        0        0     1806 2023-07-13 18:40:33.774250 fabrictestbed-1.6.0b7/.gitignore
+-rw-r--r--   0        0        0     1071 2023-07-13 18:40:33.774483 fabrictestbed-1.6.0b7/LICENSE
+-rw-r--r--   0        0        0       24 2023-07-13 18:40:33.774598 fabrictestbed-1.6.0b7/MANIFEST.in
+-rw-r--r--   0        0        0     5603 2023-07-13 18:40:33.774750 fabrictestbed-1.6.0b7/README.md
+-rw-r--r--   0        0        0       24 2023-07-26 14:20:56.916539 fabrictestbed-1.6.0b7/fabrictestbed/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:40:33.775067 fabrictestbed-1.6.0b7/fabrictestbed/cli/__init__.py
+-rw-r--r--   0        0        0    26823 2023-07-26 18:36:12.647647 fabrictestbed-1.6.0b7/fabrictestbed/cli/cli.py
+-rw-r--r--   0        0        0     1452 2023-07-13 18:40:33.775647 fabrictestbed-1.6.0b7/fabrictestbed/cli/exceptions.py
+-rw-r--r--   0        0        0     1914 2023-07-13 18:40:33.775918 fabrictestbed-1.6.0b7/fabrictestbed/slice_editor/__init__.py
+-rw-r--r--   0        0        0      201 2023-07-13 18:40:33.776101 fabrictestbed-1.6.0b7/fabrictestbed/slice_manager/__init__.py
+-rw-r--r--   0        0        0    22416 2023-07-26 18:28:39.429612 fabrictestbed-1.6.0b7/fabrictestbed/slice_manager/slice_manager.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:40:33.776619 fabrictestbed-1.6.0b7/fabrictestbed/util/__init__.py
+-rw-r--r--   0        0        0     1547 2023-07-26 18:11:43.403641 fabrictestbed-1.6.0b7/fabrictestbed/util/constants.py
+-rw-r--r--   0        0        0     1693 2023-07-26 18:12:28.124750 fabrictestbed-1.6.0b7/fabrictestbed/util/utils.py
+-rw-r--r--   0        0        0     1073 2023-07-26 18:49:56.349934 fabrictestbed-1.6.0b7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-13 18:40:33.777184 fabrictestbed-1.6.0b7/test/__init__.py
+-rw-r--r--   0        0        0     2210 2023-07-13 18:40:33.777415 fabrictestbed-1.6.0b7/test/test_cli.py
+-rw-r--r--   0        0        0     6536 1970-01-01 00:00:00.000000 fabrictestbed-1.6.0b7/PKG-INFO
```

### Comparing `fabrictestbed-1.6.0b6/.gitignore` & `fabrictestbed-1.6.0b7/.gitignore`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b6/LICENSE` & `fabrictestbed-1.6.0b7/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b6/README.md` & `fabrictestbed-1.6.0b7/README.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b6/fabrictestbed/cli/cli.py` & `fabrictestbed-1.6.0b7/fabrictestbed/cli/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,39 +20,45 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Erica Fu (ericafu@renci.org), Komal Thareja (kthare10@renci.org)
 #
+import os
+import traceback
 from typing import Any
 
 import json
 import click
 from fabric_cf.orchestrator.orchestrator_proxy import SliceState
-from fabric_cf.orchestrator.swagger_client import Slice
+from fabric_cm.credmgr.credmgr_proxy import TokenType
 from fim.slivers.network_node import NodeSliver
 
 from .exceptions import TokenExpiredException
+from ..slice_manager import CredmgrProxy
 from ..slice_manager.slice_manager import SliceManager, Status
+from ..util.constants import Constants
 
 
 def __get_slice_manager(*, oc_host: str = None, cm_host: str = None, project_id: str = None, scope: str = "all",
-                        token_location: str = None) -> SliceManager:
+                        token_location: str = None, project_name: str = None) -> SliceManager:
     """
     Get Environment Variables
     @param oc_host Orchestrator host
     @param cm_host Credmgr Host
     @param project_id Project Id
+    @param project_name Project Name
     @param scope Scope
     @param token_location Absolute location of the tokens JSON file
     @raises ClickException in case of error
     """
     return SliceManager(oc_host=oc_host, cm_host=cm_host, project_id=project_id, scope=scope,
-                        token_location=token_location)
+                        token_location=token_location, project_name=project_name)
+
 
 def __unpack(data: Any) -> Any:
     """
     Recursivly unpacks JSON dictionaries or lists embedded in a list or dict.
     @param Any to unpack
     """
     if isinstance(data, str):
@@ -81,59 +87,227 @@
     """ Token management
         (set $FABRIC_CREDMGR_HOST => CredentialManager, $FABRIC_project_id => Project Id)
     """
 
 
 @tokens.command()
 @click.option('--cmhost', help='Credmgr Host', default=None)
-@click.option('--tokenlocation', help='location for the tokens', default=None)
-@click.option('--projectid', default=None, help='project name')
+@click.option('--projectid', default=None, help='Project id')
+@click.option('--projectname', default=None, help='Project name')
+@click.option('--lifetime', default=4, help='Token lifetime in hours')
+@click.option('--comment', default=None, help='Comment/note to associate with the token')
+@click.option('--browser', default="chrome", type=click.Choice(['chrome', 'firefox', 'safari', 'edge'],
+                                                               case_sensitive=False),
+              help='Browser to use to launch the web app!')
 @click.option('--scope', type=click.Choice(['cf', 'mf', 'all'], case_sensitive=False),
               default='all', help='scope')
+@click.option('--filename', help='Location and name of the while in which to store tokens', default=None)
+@click.pass_context
+def create(ctx, cmhost: str, projectid: str, projectname: str, lifetime: int, comment: str,
+           browser: str, scope: str, filename: str):
+    """Create token
+    """
+    try:
+        if cmhost is None and os.environ.get(Constants.FABRIC_CREDMGR_HOST) is None:
+            raise click.ClickException(f"Credential Manager Host must be specified!")
+
+        if projectname is None and os.environ.get(Constants.FABRIC_PROJECT_NAME) is None and projectid is None and \
+                os.environ.get(Constants.FABRIC_PROJECT_ID) is None:
+            raise click.ClickException(f"Either Project Name or Project Id must be specified!")
+
+        cookie_name = os.getenv(Constants.FABRIC_COOKIE_NAME)
+        if cmhost is None:
+            cmhost = os.getenv(Constants.FABRIC_CREDMGR_HOST)
+
+        if cookie_name is not None:
+            cm_proxy = CredmgrProxy(credmgr_host=cmhost, cookie_name=cookie_name)
+        else:
+            cm_proxy = CredmgrProxy(credmgr_host=cmhost)
+
+        status, token_or_exception = cm_proxy.create(project_id=projectid, project_name=projectname,
+                                                     life_time_in_hours=lifetime, comment=comment,
+                                                     browser_name=browser, scope=scope, file_name=filename)
+
+        from fabric_cm.credmgr.credmgr_proxy import Status as CmStatus
+        if status == CmStatus.OK:
+            if filename is None:
+                click.echo(f"Fabric Token: {token_or_exception}")
+            else:
+                click.echo(f"Fabric Token saved at: {filename}")
+        else:
+            raise click.ClickException(f"Token could not be created! Error encountered: {token_or_exception}")
+    except click.ClickException as e:
+        raise e
+    except Exception as e:
+        raise click.ClickException(str(e))
+
+
+@tokens.command()
+@click.option('--cmhost', help='Credmgr Host', default=None)
+@click.option('--tokenlocation', help='Location of the file which contains the valid tokens', default=None)
+@click.option('--projectid', default=None, help='Project Id')
+@click.option('--projectname', default=None, help='Project name')
+@click.option('--scope', type=click.Choice(['cf', 'mf', 'all'], case_sensitive=False),
+              default='all', help='Scope')
 @click.pass_context
-def refresh(ctx, cmhost, tokenlocation, projectid, scope):
+def refresh(ctx, cmhost: str, tokenlocation: str, projectid: str, projectname: str, scope: str):
     """Refresh token
     """
-    slice_manager = __get_slice_manager(cm_host=cmhost, project_id=projectid, scope=scope,
-                                        token_location=tokenlocation)
+    try:
+        if cmhost is None and os.environ.get(Constants.FABRIC_CREDMGR_HOST) is None:
+            raise click.ClickException(f"Credential Manager Host must be specified!")
+
+        if tokenlocation is None and os.environ.get(Constants.FABRIC_TOKEN_LOCATION) is None:
+            raise click.ClickException(f"Token location must be specified !")
+
+        if projectname is None and os.environ.get(Constants.FABRIC_PROJECT_NAME) is None and projectid is None and \
+                os.environ.get(Constants.FABRIC_PROJECT_ID) is None:
+            raise click.ClickException(f"Either Project Name or Project Id must be specified!")
+
+        if tokenlocation is None:
+            tokenlocation = os.getenv(Constants.FABRIC_TOKEN_LOCATION)
+
+        slice_manager = __get_slice_manager(cm_host=cmhost, project_id=projectid, scope=scope,
+                                            token_location=tokenlocation, project_name=projectname)
+
+        click.echo(f"ID Token: {slice_manager.get_id_token()}")
+        click.echo(f"Refresh Token: {slice_manager.get_refresh_token()}")
+        click.echo(f"Refreshed token saved at: {tokenlocation}")
+    except click.ClickException as e:
+        raise e
+    except Exception as e:
+        raise click.ClickException(str(e))
+
 
-    click.echo(f"ID Token: {slice_manager.get_id_token()}")
-    click.echo(f"Refresh Token: {slice_manager.get_refresh_token()}")
+@tokens.command()
+@click.option('--cmhost', help='Credmgr Host', default=None)
+@click.option('--tokenlocation', help='Location of the file which contains the valid tokens', default=None)
+@click.option('--refreshtoken', help='Refresh token to be revoked; '
+                                     'If specified refresh token from tokenlocation is ignored!', default=None)
+@click.option('--identitytoken', help='Identity token to authenticate the user; '
+                                      'If specified identity token from tokenlocation is ignored', default=None)
+@click.pass_context
+def revoke(ctx, cmhost: str, tokenlocation: str, refreshtoken: str, identitytoken: str):
+    """ Revoke token
+    """
+    try:
+        fail = False
+        if cmhost is None and os.environ.get(Constants.FABRIC_CREDMGR_HOST) is None:
+            raise click.ClickException(f"Credential Manager Host must be specified!")
+
+        if tokenlocation is None and os.environ.get(Constants.FABRIC_TOKEN_LOCATION) is None and \
+                refreshtoken is None and identitytoken is None:
+            raise click.ClickException(f"Either Token location must be specified or pass refresh "
+                                       f"token and identity token!")
+
+        # Token in the file located at tokenlocation is being revoked
+        if tokenlocation is not None or os.environ.get(Constants.FABRIC_TOKEN_LOCATION) is not None:
+            if tokenlocation is None:
+                tokenlocation = os.getenv(Constants.FABRIC_TOKEN_LOCATION)
+
+            if os.path.exists(tokenlocation):
+                with open(tokenlocation, 'r') as stream:
+                    tokens = json.loads(stream.read())
+                    refreshtoken = tokens.get(CredmgrProxy.REFRESH_TOKEN)
+                    identitytoken = tokens.get(CredmgrProxy.ID_TOKEN)
+            else:
+                raise click.ClickException(f"Token file '{tokenlocation}' does not exist!")
+
+        if cmhost is None:
+            cmhost = os.environ.get(Constants.FABRIC_CREDMGR_HOST)
+
+        cm_proxy = CredmgrProxy(credmgr_host=cmhost)
+
+        status, error_str = cm_proxy.revoke(refresh_token=refreshtoken, identity_token=identitytoken,
+                                            token_type=TokenType.Refresh)
+        from fabric_cm.credmgr.credmgr_proxy import Status as CmStatus
+        if status == CmStatus.OK:
+            click.echo("Token revoked successfully")
+        else:
+            raise click.ClickException(f"Token could not be revoked! Error encountered: {error_str}")
+    except click.ClickException as e:
+        raise e
+    except Exception as e:
+        traceback.print_exc()
+        raise click.ClickException(str(e))
 
 
 @tokens.command()
 @click.option('--cmhost', help='Credmgr Host', default=None)
 @click.option('--tokenlocation', help='location for the tokens', default=None)
-@click.option('--refreshtoken', help='Refresh token to be revoked', default=None)
+@click.option('--identitytoken', help='Identity token to be revoked', default=None)
+@click.option('--tokenhash', help='SHA256 hash for the token being revoked; If not specified, '
+                                  'it is assumed that the identity token being passed is being revoked', default=None)
 @click.pass_context
-def revoke(ctx, cmhost, tokenlocation, refreshtoken):
+def revoke_identity_token(ctx, cmhost: str, tokenlocation: str, identitytoken: str, tokenhash: str):
     """ Revoke token
     """
-    slice_manager = __get_slice_manager(cm_host=cmhost, token_location=tokenlocation)
+    try:
+        fail = False
+        if cmhost is None and os.environ.get(Constants.FABRIC_CREDMGR_HOST) is None:
+            raise click.ClickException(f"Credential Manager Host must be specified!")
+
+        if tokenlocation is None and os.environ.get(Constants.FABRIC_TOKEN_LOCATION) is None and \
+                identitytoken is None:
+            raise click.ClickException(f"Either Token location must be specified or pass identity token!")
+
+        if tokenlocation is not None or os.environ.get(Constants.FABRIC_TOKEN_LOCATION) is not None:
+            slice_manager = __get_slice_manager(cm_host=cmhost, token_location=tokenlocation)
+
+            status, error_str = slice_manager.revoke_token(token_type=TokenType.Identity)
+            if status != Status.OK:
+                fail = True
+        else:
+            if cmhost is None:
+                cmhost = os.environ.get(Constants.FABRIC_CREDMGR_HOST)
+
+            cm_proxy = CredmgrProxy(credmgr_host=cmhost)
+
+            status, error_str = cm_proxy.revoke(identity_token=identitytoken, token_hash=tokenhash,
+                                                token_type=TokenType.Identity)
+            from fabric_cm.credmgr.credmgr_proxy import Status as CmStatus
+            if status != CmStatus.OK:
+                fail = True
+
+        if not fail:
+            click.echo("Token revoked successfully")
+        else:
+            raise click.ClickException(f"Token could not be revoked! Error encountered: {error_str}")
+    except click.ClickException as e:
+        raise e
+    except Exception as e:
+        raise click.ClickException(str(e))
 
-    status, error_str = slice_manager.revoke_token(refresh_token=refreshtoken)
-    if status == Status.OK:
-        click.echo("Token revoked successfully")
-    else:
-        raise click.ClickException(f"Token could not be revoked! Error encountered: {error_str}")
 
 @tokens.command()
 @click.option('--cmhost', help='Credmgr Host', default=None)
 @click.option('--tokenlocation', help='location for the tokens', default=None)
 @click.pass_context
 def clear_cache(ctx, cmhost, tokenlocation):
     """ Clear cached token
     """
-    slice_manager = __get_slice_manager(cm_host=cmhost, token_location=tokenlocation)
-
-    status, error_str = slice_manager.clear_token_cache(file_name=tokenlocation)
-    if status == Status.OK:
-        click.echo("Token cache cleared successfully")
-    else:
-        raise click.ClickException(f"Token could not be revoked! Error encountered: {error_str}")
+    try:
+        if cmhost is None and os.environ.get(Constants.FABRIC_CREDMGR_HOST) is None:
+            raise click.ClickException(f"Credential Manager Host must be specified!")
+
+        if tokenlocation is None:
+            raise click.ClickException(f"Token location must be specified !")
+
+        slice_manager = __get_slice_manager(cm_host=cmhost, token_location=tokenlocation)
+
+        status, error_str = slice_manager.clear_token_cache(file_name=tokenlocation)
+        if status == Status.OK:
+            click.echo("Token cache cleared successfully")
+        else:
+            raise click.ClickException(f"Token could not be revoked! Error encountered: {error_str}")
+
+    except click.ClickException as e:
+        raise e
+    except Exception as e:
+        raise click.ClickException(str(e))
 
 
 @click.group()
 @click.pass_context
 def slices(ctx):
     """ Slice management
         (set $FABRIC_ORCHESTRATOR_HOST => Orchestrator, $FABRIC_CREDMGR_HOST => CredentialManager,
```

### Comparing `fabrictestbed-1.6.0b6/fabrictestbed/cli/exceptions.py` & `fabrictestbed-1.6.0b7/fabrictestbed/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b6/fabrictestbed/slice_editor/__init__.py` & `fabrictestbed-1.6.0b7/fabrictestbed/slice_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b6/fabrictestbed/slice_manager/slice_manager.py` & `fabrictestbed-1.6.0b7/fabrictestbed/slice_manager/slice_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,47 +33,53 @@
 from fabric_cf.orchestrator.swagger_client import Sliver, Slice
 from fabric_cf.orchestrator.swagger_client.models import PoaData
 from fabric_cm.credmgr.credmgr_proxy import TokenType
 
 from fabrictestbed.slice_editor import ExperimentTopology, AdvertisedTopology, Node, GraphFormat
 from fabrictestbed.slice_manager import CredmgrProxy, OrchestratorProxy, CmStatus, Status, SliceState
 from fabrictestbed.util.constants import Constants
+from fabrictestbed.util.utils import Utils
 
 
 class SliceManagerException(Exception):
     """ Slice Manager Exception """
 
 
 class SliceManager:
     """
     Implements User facing Control Framework API interface
     """
     def __init__(self, *, cm_host: str = None, oc_host: str = None, token_location: str = None,
-                 project_id: str = None, scope: str = "all", initialize: bool = True):
+                 project_id: str = None, scope: str = "all", initialize: bool = True,
+                 project_name: str = None):
         self.logger = logging.getLogger()
         if cm_host is None:
             cm_host = os.environ.get(Constants.FABRIC_CREDMGR_HOST)
         if oc_host is None:
             oc_host = os.environ.get(Constants.FABRIC_ORCHESTRATOR_HOST)
         self.cm_proxy = CredmgrProxy(credmgr_host=cm_host)
         self.oc_proxy = OrchestratorProxy(orchestrator_host=oc_host)
         self.token_location = token_location
         self.tokens = {}
         self.project_id = project_id
         if self.project_id is None:
             self.project_id = os.environ.get(Constants.FABRIC_PROJECT_ID)
+        self.project_name = project_name
+        if self.project_name is None:
+            self.project_name = os.environ.get(Constants.FABRIC_PROJECT_NAME)
         self.scope = scope
         if self.token_location is None:
             self.token_location = os.environ.get(Constants.FABRIC_TOKEN_LOCATION)
         self.initialized = False
         # Validate the required parameters are set
-        if self.cm_proxy is None or self.oc_proxy is None or self.token_location is None or self.project_id is None:
+        if self.cm_proxy is None or self.oc_proxy is None or self.token_location is None or \
+                (self.project_id is None and self.project_name is None):
             raise SliceManagerException(f"Invalid initialization parameters: cm_proxy={self.cm_proxy}, "
                                         f"oc_proxy={self.oc_proxy}, token_location={self.token_location}, "
-                                        f"project_id={self.project_id}")
+                                        f"project_id={self.project_id}, project_name={self.project_name}")
         if initialize:
             self.initialize()
 
     def initialize(self):
         """
         Initialize the Slice Manager object
         - Load the tokens
@@ -149,45 +155,69 @@
     def set_token_location(self, *, token_location: str):
         """
         Set token location: path of the file where tokens should be saved
         @param token_location file name along with complete path where tokens should be stored
         """
         self.token_location = token_location
 
+    def create_token(self, scope: str = "all", project_id: str = None, project_name: str = None, file_name: str = None,
+                     life_time_in_hours: int = 4, comment: str = "Created via API",
+                     browser_name: str = "chrome") -> Tuple[Status, Union[dict, Exception]]:
+        """
+        Create token
+        @param project_id: Project Id
+        @param project_name: Project Name
+        @param scope: scope
+        @param file_name: File name
+        @param life_time_in_hours: Token lifetime in hours
+        @param comment: comment associated with the token
+        @param browser_name: Browser name; allowed values: chrome, firefox, safari, edge
+        @returns Tuple of Status, token json or Exception
+        @raises Exception in case of failure
+        """
+        return self.cm_proxy.create(scope=scope, project_id=project_id, project_name=project_name,
+                                    file_name=file_name, life_time_in_hours=life_time_in_hours, comment=comment,
+                                    browser_name=browser_name)
+
     def refresh_tokens(self, *, refresh_token: str) -> Tuple[str, str]:
         """
         Refresh tokens
         User is expected to invoke refresh token API before invoking any other APIs to ensure the token is not expired.
         User is also expected to update the returned refresh token in the JupyterHub environment.
         @returns tuple of id token and refresh token
         @note this exposes an API for the user to refresh tokens explicitly only. CredMgrProxy::refresh already
         updates the refresh tokens to the token file atomically.
         """
         status, tokens = self.cm_proxy.refresh(project_id=self.project_id, scope=self.scope,
-                                               refresh_token=refresh_token, file_name=self.token_location)
+                                               refresh_token=refresh_token, file_name=self.token_location,
+                                               project_name=self.project_name)
         if status == CmStatus.OK:
             self.tokens = tokens
             return tokens.get(CredmgrProxy.ID_TOKEN, None), tokens.get(CredmgrProxy.REFRESH_TOKEN, None)
         raise SliceManagerException(tokens.get(CredmgrProxy.ERROR))
 
-    def revoke_token(self, *, refresh_token: str = None, id_token: str = None,
+    def revoke_token(self, *, refresh_token: str = None, id_token: str = None, token_hash: str = None,
                      token_type: TokenType = TokenType.Refresh) -> Tuple[Status, Any]:
         """
         Revoke a refresh token
         @param refresh_token Refresh Token to be revoked
         @param id_token Identity Token
         @param token_type type of the token being revoked
         @return Tuple of the status and revoked refresh token
         """
         if refresh_token is None:
             refresh_token = self.get_refresh_token()
         if id_token is None:
             id_token = self.get_id_token()
+        if token_hash is None:
+            token_hash = Utils.generate_sha256(token=id_token)
 
-        return self.cm_proxy.revoke(refresh_token=refresh_token, identity_token=id_token, token_type=token_type)
+        print(f"KOMAL ---- {refresh_token}  {id_token}  {token_hash} {token_type}")
+        return self.cm_proxy.revoke(refresh_token=refresh_token, identity_token=id_token, token_hash=token_hash,
+                                    token_type=token_type)
 
     def token_revoke_list(self, *, project_id: str) -> Tuple[Status, Union[Exception, List[str]]]:
         """
         Get Token Revoke list for a project
         @param project_id project_id
         @return token revoke list
         """
```

### Comparing `fabrictestbed-1.6.0b6/fabrictestbed/util/constants.py` & `fabrictestbed-1.6.0b7/fabrictestbed/util/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,8 +25,10 @@
 # Author: Komal Thareja (kthare10@renci.org)
 
 class Constants:
     CILOGON_REFRESH_TOKEN = "CILOGON_REFRESH_TOKEN"
     FABRIC_TOKEN_LOCATION = "FABRIC_TOKEN_LOCATION"
     FABRIC_CREDMGR_HOST = "FABRIC_CREDMGR_HOST"
     FABRIC_ORCHESTRATOR_HOST = "FABRIC_ORCHESTRATOR_HOST"
-    FABRIC_PROJECT_ID = "FABRIC_PROJECT_ID"
+    FABRIC_PROJECT_ID = "FABRIC_PROJECT_ID"
+    FABRIC_PROJECT_NAME = "FABRIC_PROJECT_NAME"
+    FABRIC_COOKIE_NAME = "FABRIC_COOKIE_NAME"
```

### Comparing `fabrictestbed-1.6.0b6/pyproject.toml` & `fabrictestbed-1.6.0b7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 dynamic = ["version"]
 
 keywords = ["Swagger", "FABRIC Python Client Library with CLI"]
 
 requires-python = '>=3.9'
 dependencies = [
     "click",
-    "fabric-credmgr-client==1.6.0b4",
+    "fabric-credmgr-client==1.6.0b8",
     "fabric-orchestrator-client==1.6.0b3",
     "paramiko"
     ]
 
 scripts = {"fabric-cli" = "fabrictestbed.cli.cli:cli"}
 
 [project.optional-dependencies]
```

### Comparing `fabrictestbed-1.6.0b6/test/test_cli.py` & `fabrictestbed-1.6.0b7/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b6/PKG-INFO` & `fabrictestbed-1.6.0b7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: fabrictestbed
-Version: 1.6.0b6
+Version: 1.6.0b7
 Summary: FABRIC Python Client Library with CLI
 Keywords: Swagger,FABRIC Python Client Library with CLI
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: click
-Requires-Dist: fabric-credmgr-client==1.6.0b4
+Requires-Dist: fabric-credmgr-client==1.6.0b8
 Requires-Dist: fabric-orchestrator-client==1.6.0b3
 Requires-Dist: paramiko
 Requires-Dist: coverage>=4.0.3 ; extra == "test"
 Requires-Dist: nose>=1.3.7 ; extra == "test"
 Requires-Dist: pluggy>=0.3.1 ; extra == "test"
 Requires-Dist: py>=1.4.31 ; extra == "test"
 Requires-Dist: randomize>=0.13 ; extra == "test"
```

