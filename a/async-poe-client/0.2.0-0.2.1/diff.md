# Comparing `tmp/async_poe_client-0.2.0.tar.gz` & `tmp/async_poe_client-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_poe_client-0.2.0.tar", max compression
+gzip compressed data, was "async_poe_client-0.2.1.tar", max compression
```

## Comparing `async_poe_client-0.2.0.tar` & `async_poe_client-0.2.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0       32 2023-07-22 14:46:24.800780 async_poe_client-0.2.0/async_poe_client/__init__.py
--rw-r--r--   0        0        0    48782 2023-07-25 06:32:25.199349 async_poe_client-0.2.0/async_poe_client/client.py
--rw-r--r--   0        0        0     1145 2023-07-19 06:18:30.461961 async_poe_client-0.2.0/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql
--rw-r--r--   0        0        0      536 2023-07-19 06:18:30.461961 async_poe_client-0.2.0/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql
--rw-r--r--   0        0        0      187 2023-07-19 06:18:30.461961 async_poe_client-0.2.0/async_poe_client/poe_graphql/AutoSubscriptionMutation.graphql
--rw-r--r--   0        0        0      701 2023-07-22 07:43:55.501987 async_poe_client-0.2.0/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql
--rw-r--r--   0        0        0      105 2023-07-19 06:18:30.461961 async_poe_client-0.2.0/async_poe_client/poe_graphql/BioFragment.graphql
--rw-r--r--   0        0        0      169 2023-07-22 05:55:18.261809 async_poe_client-0.2.0/async_poe_client/poe_graphql/BotDeletionButton_poeBotDelete_Mutation.graphql
--rw-r--r--   0        0        0       78 2023-07-19 06:18:30.462960 async_poe_client-0.2.0/async_poe_client/poe_graphql/ChatAddedSubscription.graphql
--rw-r--r--   0        0        0      106 2023-07-19 06:18:30.462960 async_poe_client-0.2.0/async_poe_client/poe_graphql/ChatFragment.graphql
--rw-r--r--   0        0        0    12084 2023-07-19 06:18:30.462960 async_poe_client-0.2.0/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql
--rw-r--r--   0        0        0      712 2023-07-19 06:18:30.462960 async_poe_client-0.2.0/async_poe_client/poe_graphql/ChatPaginationQuery.graphql
--rw-r--r--   0        0        0      162 2023-07-19 06:18:30.462960 async_poe_client-0.2.0/async_poe_client/poe_graphql/ChatViewQuery.graphql
--rw-r--r--   0        0        0      167 2023-07-19 06:18:30.463987 async_poe_client-0.2.0/async_poe_client/poe_graphql/DeleteHumanMessagesMutation.graphql
--rw-r--r--   0        0        0      129 2023-07-19 06:18:30.463987 async_poe_client-0.2.0/async_poe_client/poe_graphql/DeleteMessageMutation.graphql
--rw-r--r--   0        0        0      154 2023-07-19 06:18:30.463987 async_poe_client-0.2.0/async_poe_client/poe_graphql/DeleteUserMessagesMutation.graphql
--rw-r--r--   0        0        0     1148 2023-07-19 06:18:30.463987 async_poe_client-0.2.0/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql
--rw-r--r--   0        0        0      111 2023-07-19 06:18:30.463987 async_poe_client-0.2.0/async_poe_client/poe_graphql/HandleFragment.graphql
--rw-r--r--   0        0        0      319 2023-07-19 06:18:30.464960 async_poe_client-0.2.0/async_poe_client/poe_graphql/LoginWithVerificationCodeMutation.graphql
--rw-r--r--   0        0        0     1985 2023-07-19 06:18:30.464960 async_poe_client-0.2.0/async_poe_client/poe_graphql/MessageAddedSubscription.graphql
--rw-r--r--   0        0        0      141 2023-07-19 06:18:30.464960 async_poe_client-0.2.0/async_poe_client/poe_graphql/MessageDeletedSubscription.graphql
--rw-r--r--   0        0        0      207 2023-07-19 06:18:30.464960 async_poe_client-0.2.0/async_poe_client/poe_graphql/MessageFragment.graphql
--rw-r--r--   0        0        0      152 2023-07-19 06:18:30.464960 async_poe_client-0.2.0/async_poe_client/poe_graphql/MessageRemoveVoteMutation.graphql
--rw-r--r--   0        0        0      223 2023-07-19 06:18:30.465959 async_poe_client-0.2.0/async_poe_client/poe_graphql/MessageSetVoteMutation.graphql
--rw-r--r--   0        0        0     1832 2023-07-19 06:18:30.465959 async_poe_client-0.2.0/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql
--rw-r--r--   0        0        0      968 2023-07-19 06:18:30.465959 async_poe_client-0.2.0/async_poe_client/poe_graphql/PoeBotEditMutation.graphql
--rw-r--r--   0        0        0      963 2023-07-19 06:18:30.465959 async_poe_client-0.2.0/async_poe_client/poe_graphql/SendMessageMutation.graphql
--rw-r--r--   0        0        0      275 2023-07-19 06:18:30.465959 async_poe_client-0.2.0/async_poe_client/poe_graphql/SendVerificationCodeForLoginMutation.graphql
--rw-r--r--   0        0        0      222 2023-07-19 06:18:30.465959 async_poe_client-0.2.0/async_poe_client/poe_graphql/ShareMessagesMutation.graphql
--rw-r--r--   0        0        0      321 2023-07-19 06:18:30.466959 async_poe_client-0.2.0/async_poe_client/poe_graphql/SignupWithVerificationCodeMutation.graphql
--rw-r--r--   0        0        0      166 2023-07-19 06:18:30.466959 async_poe_client-0.2.0/async_poe_client/poe_graphql/StaleChatUpdateMutation.graphql
--rw-r--r--   0        0        0      170 2023-07-19 06:18:30.466959 async_poe_client-0.2.0/async_poe_client/poe_graphql/SubscriptionsMutation.graphql
--rw-r--r--   0        0        0       98 2023-07-19 06:18:30.466959 async_poe_client-0.2.0/async_poe_client/poe_graphql/SummarizePlainPostQuery.graphql
--rw-r--r--   0        0        0      150 2023-07-19 06:18:30.466959 async_poe_client-0.2.0/async_poe_client/poe_graphql/SummarizeQuotePostQuery.graphql
--rw-r--r--   0        0        0      183 2023-07-19 06:18:30.466959 async_poe_client-0.2.0/async_poe_client/poe_graphql/SummarizeSharePostQuery.graphql
--rw-r--r--   0        0        0      382 2023-07-19 06:18:30.467959 async_poe_client-0.2.0/async_poe_client/poe_graphql/UserSnippetFragment.graphql
--rw-r--r--   0        0        0      421 2023-07-19 06:18:30.467959 async_poe_client-0.2.0/async_poe_client/poe_graphql/ViewerInfoQuery.graphql
--rw-r--r--   0        0        0     1068 2023-07-19 06:18:30.467959 async_poe_client-0.2.0/async_poe_client/poe_graphql/ViewerStateFragment.graphql
--rw-r--r--   0        0        0      700 2023-07-19 06:18:30.467959 async_poe_client-0.2.0/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql
--rw-r--r--   0        0        0       53 2023-07-23 07:11:13.271223 async_poe_client-0.2.0/async_poe_client/requirements.txt
--rw-r--r--   0        0        0     2459 2023-07-25 06:17:58.542713 async_poe_client-0.2.0/async_poe_client/util.py
--rw-r--r--   0        0        0      467 2023-07-25 06:40:16.211595 async_poe_client-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    17252 2023-07-25 06:41:01.974440 async_poe_client-0.2.0/README.md
--rw-r--r--   0        0        0    17538 1970-01-01 00:00:00.000000 async_poe_client-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       32 2023-07-22 14:46:24.800780 async_poe_client-0.2.1/async_poe_client/__init__.py
+-rw-r--r--   0        0        0    48379 2023-07-26 00:46:30.166874 async_poe_client-0.2.1/async_poe_client/client.py
+-rw-r--r--   0        0        0     1145 2023-07-19 06:18:30.461961 async_poe_client-0.2.1/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql
+-rw-r--r--   0        0        0      536 2023-07-19 06:18:30.461961 async_poe_client-0.2.1/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql
+-rw-r--r--   0        0        0      187 2023-07-19 06:18:30.461961 async_poe_client-0.2.1/async_poe_client/poe_graphql/AutoSubscriptionMutation.graphql
+-rw-r--r--   0        0        0      701 2023-07-22 07:43:55.501987 async_poe_client-0.2.1/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql
+-rw-r--r--   0        0        0      105 2023-07-19 06:18:30.461961 async_poe_client-0.2.1/async_poe_client/poe_graphql/BioFragment.graphql
+-rw-r--r--   0        0        0      169 2023-07-22 05:55:18.261809 async_poe_client-0.2.1/async_poe_client/poe_graphql/BotDeletionButton_poeBotDelete_Mutation.graphql
+-rw-r--r--   0        0        0       78 2023-07-19 06:18:30.462960 async_poe_client-0.2.1/async_poe_client/poe_graphql/ChatAddedSubscription.graphql
+-rw-r--r--   0        0        0      106 2023-07-19 06:18:30.462960 async_poe_client-0.2.1/async_poe_client/poe_graphql/ChatFragment.graphql
+-rw-r--r--   0        0        0    12084 2023-07-19 06:18:30.462960 async_poe_client-0.2.1/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql
+-rw-r--r--   0        0        0      712 2023-07-19 06:18:30.462960 async_poe_client-0.2.1/async_poe_client/poe_graphql/ChatPaginationQuery.graphql
+-rw-r--r--   0        0        0      162 2023-07-19 06:18:30.462960 async_poe_client-0.2.1/async_poe_client/poe_graphql/ChatViewQuery.graphql
+-rw-r--r--   0        0        0      167 2023-07-19 06:18:30.463987 async_poe_client-0.2.1/async_poe_client/poe_graphql/DeleteHumanMessagesMutation.graphql
+-rw-r--r--   0        0        0      129 2023-07-19 06:18:30.463987 async_poe_client-0.2.1/async_poe_client/poe_graphql/DeleteMessageMutation.graphql
+-rw-r--r--   0        0        0      154 2023-07-19 06:18:30.463987 async_poe_client-0.2.1/async_poe_client/poe_graphql/DeleteUserMessagesMutation.graphql
+-rw-r--r--   0        0        0     1148 2023-07-19 06:18:30.463987 async_poe_client-0.2.1/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql
+-rw-r--r--   0        0        0      111 2023-07-19 06:18:30.463987 async_poe_client-0.2.1/async_poe_client/poe_graphql/HandleFragment.graphql
+-rw-r--r--   0        0        0      319 2023-07-19 06:18:30.464960 async_poe_client-0.2.1/async_poe_client/poe_graphql/LoginWithVerificationCodeMutation.graphql
+-rw-r--r--   0        0        0     1985 2023-07-19 06:18:30.464960 async_poe_client-0.2.1/async_poe_client/poe_graphql/MessageAddedSubscription.graphql
+-rw-r--r--   0        0        0      141 2023-07-19 06:18:30.464960 async_poe_client-0.2.1/async_poe_client/poe_graphql/MessageDeletedSubscription.graphql
+-rw-r--r--   0        0        0      207 2023-07-19 06:18:30.464960 async_poe_client-0.2.1/async_poe_client/poe_graphql/MessageFragment.graphql
+-rw-r--r--   0        0        0      152 2023-07-19 06:18:30.464960 async_poe_client-0.2.1/async_poe_client/poe_graphql/MessageRemoveVoteMutation.graphql
+-rw-r--r--   0        0        0      223 2023-07-19 06:18:30.465959 async_poe_client-0.2.1/async_poe_client/poe_graphql/MessageSetVoteMutation.graphql
+-rw-r--r--   0        0        0     1832 2023-07-19 06:18:30.465959 async_poe_client-0.2.1/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql
+-rw-r--r--   0        0        0      968 2023-07-19 06:18:30.465959 async_poe_client-0.2.1/async_poe_client/poe_graphql/PoeBotEditMutation.graphql
+-rw-r--r--   0        0        0      963 2023-07-19 06:18:30.465959 async_poe_client-0.2.1/async_poe_client/poe_graphql/SendMessageMutation.graphql
+-rw-r--r--   0        0        0      275 2023-07-19 06:18:30.465959 async_poe_client-0.2.1/async_poe_client/poe_graphql/SendVerificationCodeForLoginMutation.graphql
+-rw-r--r--   0        0        0      222 2023-07-19 06:18:30.465959 async_poe_client-0.2.1/async_poe_client/poe_graphql/ShareMessagesMutation.graphql
+-rw-r--r--   0        0        0      321 2023-07-19 06:18:30.466959 async_poe_client-0.2.1/async_poe_client/poe_graphql/SignupWithVerificationCodeMutation.graphql
+-rw-r--r--   0        0        0      166 2023-07-19 06:18:30.466959 async_poe_client-0.2.1/async_poe_client/poe_graphql/StaleChatUpdateMutation.graphql
+-rw-r--r--   0        0        0      170 2023-07-19 06:18:30.466959 async_poe_client-0.2.1/async_poe_client/poe_graphql/SubscriptionsMutation.graphql
+-rw-r--r--   0        0        0       98 2023-07-19 06:18:30.466959 async_poe_client-0.2.1/async_poe_client/poe_graphql/SummarizePlainPostQuery.graphql
+-rw-r--r--   0        0        0      150 2023-07-19 06:18:30.466959 async_poe_client-0.2.1/async_poe_client/poe_graphql/SummarizeQuotePostQuery.graphql
+-rw-r--r--   0        0        0      183 2023-07-19 06:18:30.466959 async_poe_client-0.2.1/async_poe_client/poe_graphql/SummarizeSharePostQuery.graphql
+-rw-r--r--   0        0        0      382 2023-07-19 06:18:30.467959 async_poe_client-0.2.1/async_poe_client/poe_graphql/UserSnippetFragment.graphql
+-rw-r--r--   0        0        0      421 2023-07-19 06:18:30.467959 async_poe_client-0.2.1/async_poe_client/poe_graphql/ViewerInfoQuery.graphql
+-rw-r--r--   0        0        0     1068 2023-07-19 06:18:30.467959 async_poe_client-0.2.1/async_poe_client/poe_graphql/ViewerStateFragment.graphql
+-rw-r--r--   0        0        0      700 2023-07-19 06:18:30.467959 async_poe_client-0.2.1/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql
+-rw-r--r--   0        0        0       53 2023-07-23 07:11:13.271223 async_poe_client-0.2.1/async_poe_client/requirements.txt
+-rw-r--r--   0        0        0     2459 2023-07-25 06:17:58.542713 async_poe_client-0.2.1/async_poe_client/util.py
+-rw-r--r--   0        0        0      467 2023-07-25 06:53:59.884106 async_poe_client-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    17721 2023-07-25 06:52:50.946100 async_poe_client-0.2.1/README.md
+-rw-r--r--   0        0        0    18004 1970-01-01 00:00:00.000000 async_poe_client-0.2.1/PKG-INFO
```

### Comparing `async_poe_client-0.2.0/async_poe_client/client.py` & `async_poe_client-0.2.1/async_poe_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,18 +72,19 @@
 
         Raises:
             Raises an Exception if it fails to get the base data.
             Raises a ValueError if it fails to extract 'next_data', 'viewer', 'user_id', or 'formkey' from the response.
         """
         try:
             async with aiohttp.ClientSession(**self.session_args) as client:
-                response = await client.get(HOME_URL)
+                response = await client.get(HOME_URL,timeout=8)
                 text = await response.text()
         except Exception as e:
             raise Exception("Failed to get basedata from home.") from e
+        """extract next_data from html"""
         try:
             """get next_data"""
             json_regex = (
                 r'<script id="__NEXT_DATA__" type="application\/json">(.+?)</script>'
             )
             json_text = re.search(json_regex, text).group(1)
             self.next_data = json.loads(json_text)
@@ -170,20 +171,20 @@
 
         Raises:
             Raises a ValueError exception if it fails to get the chat data.
         """
         url = (
             f'https://poe.com/_next/data/{self.next_data["buildId"]}/{url_botname}.json'
         )
-        retry = 6
+        retry = 3
         error = Exception("Unknown error")
         while retry > 0:
             try:
                 async with aiohttp.ClientSession(**self.session_args) as client:
-                    response = await client.get(url, timeout=3)
+                    response = await client.get(url, timeout=8)
                     data = await response.text()  # noqa: E501
                     json_data = json.loads(data)
                     chat_data = json_data["pageProps"]["data"]["chatOfBotHandle"]
                     return chat_data
             except Exception as e:
                 error = e
                 retry -= 1
@@ -766,15 +767,15 @@
                 url_botname, question, with_chat_break
             )
             last_text = ""
             yield_header = False
             suggestion_list = []
             self.bots[url_botname]["Suggestion"] = []
             retry = 5
-            suggestion_lost = 5
+            suggestion_lost = 10
             while retry >= 0:
                 try:
                     response = await client.get(self.channel_url)
                     raw_data = await response.json()
                     if "messages" not in raw_data:
                         retry -= 1
                         if retry == 0:
@@ -789,55 +790,49 @@
                         plain_text = message["text"][len(last_text) :]
                         last_text = message["text"]
                         if (
                             self.bots[url_botname]["defaultBotObject"][
                                 "hasSuggestedReplies"
                             ]
                             and suggest_able
-                            and message["state"] == "complete"
                         ):
-                            if len(message["suggestedReplies"]) == 0:
-                                suggestion_lost -= 1
-                                if suggestion_lost <= 0:
-                                    logger.error(
-                                        "Failed to get suggestions:Poe didn't send suggestions"
-                                    )
-                                    break
-                            if 0 < len(message["suggestedReplies"]) < 3:
-                                if len(message["suggestedReplies"]) == len(
-                                    suggestion_list
-                                ):
+                            if plain_text:
+                                yield plain_text
+                            else:
+                                if len(message["suggestedReplies"]) == 0:
                                     suggestion_lost -= 1
                                     if suggestion_lost <= 0:
                                         logger.error(
-                                            "Failed to get suggestions:Poe didn't send enough suggestions"
+                                            "Failed to get suggestions:Poe didn't send suggestions"
                                         )
                                         break
-                                if not yield_header:
-                                    yield_header = True
-                                    yield "\n\nSuggested Reply:"
-                                for suggest in message["suggestedReplies"]:
-                                    if suggest not in suggestion_list:
-                                        suggestion_list.append(
-                                            message["suggestedReplies"][-1]
-                                        )
-                                        yield f"\n{str(len(message['suggestedReplies']))}:{message['suggestedReplies'][-1]}"  # noqa: E501
-                            elif len(message["suggestedReplies"]) >= 3:
-                                suggestion_list.append(message["suggestedReplies"][-1])
-                                self.bots[url_botname]["Suggestion"] = suggestion_list
-                                yield f"\n{str(len(message['suggestedReplies']))}:{message['suggestedReplies'][-1]}"
-                                break
-                            else:
-                                yield plain_text
+                                else:
+                                    if len(message["suggestedReplies"]) == len(
+                                        suggestion_list
+                                    ):
+                                        suggestion_lost -= 1
+                                        if suggestion_lost <= 0:
+                                            logger.error(
+                                                "Failed to get enough suggestions:Poe didn't send suggestions"
+                                            )
+                                            break
+                                    if not yield_header:
+                                        yield_header = True
+                                        yield "\n\nSuggested Reply:"
+                                    for suggest in message["suggestedReplies"]:
+                                        if suggest not in suggestion_list:
+                                            yield f"\n{str(len(suggestion_list)+1)}:{suggest}"
+                                            suggestion_list.append(suggest)
+                                    if len(suggestion_list) >= 3:
+                                        break
                         else:
-                            if message["state"] == "complete":
+                            if plain_text:
                                 yield plain_text
+                            if message["state"] == "complete":
                                 break
-                            else:
-                                yield plain_text
                     else:
                         retry -= 1
                         if retry == 0:
                             if retry == 0:
                                 raise Exception(
                                     "Failed to get answer form poe too many times."
                                 )
```

### Comparing `async_poe_client-0.2.0/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql` & `async_poe_client-0.2.1/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.2.0/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql` & `async_poe_client-0.2.1/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.2.0/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql` & `async_poe_client-0.2.1/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.2.0/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql` & `async_poe_client-0.2.1/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.2.0/async_poe_client/poe_graphql/ChatPaginationQuery.graphql` & `async_poe_client-0.2.1/async_poe_client/poe_graphql/ChatPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.2.0/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql` & `async_poe_client-0.2.1/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.2.0/async_poe_client/poe_graphql/MessageAddedSubscription.graphql` & `async_poe_client-0.2.1/async_poe_client/poe_graphql/MessageAddedSubscription.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.2.0/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql` & `async_poe_client-0.2.1/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.2.0/async_poe_client/poe_graphql/PoeBotEditMutation.graphql` & `async_poe_client-0.2.1/async_poe_client/poe_graphql/PoeBotEditMutation.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.2.0/async_poe_client/poe_graphql/SendMessageMutation.graphql` & `async_poe_client-0.2.1/async_poe_client/poe_graphql/SendMessageMutation.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.2.0/async_poe_client/poe_graphql/ViewerStateFragment.graphql` & `async_poe_client-0.2.1/async_poe_client/poe_graphql/ViewerStateFragment.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.2.0/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql` & `async_poe_client-0.2.1/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.2.0/async_poe_client/util.py` & `async_poe_client-0.2.1/async_poe_client/util.py`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.2.0/README.md` & `async_poe_client-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # User Guide
-
-[中文版本](README_zh_CN.md)
+latest version:0.1.9  
+[中文使用指南](README_zh_CN.md)
 
 This is a guide on how to use the `async-poe-Client` library. Before starting, make sure you've installed this library.
 
 ```
 pip install async-poe-client
 ```
 
@@ -36,14 +36,17 @@
   The relationship between this url_botname and other names can be understood as:  
     1. For the system's built-in bots, the name of the bot you see on the poe web page and the url_botname are always
        equal (but neither equals the handle).
     2. For bots you create, url_botname = handle. If display_name is set, the name you see on the web page is display_name;
        if not set, you see url_botname (handle).
        However, there are special cases where the handle does not follow the above rules, such as the handle of all bots
        obtained using get_available_bots always equals url_botname.
+- 2.How to obtain p_b and formkey? ->  
+    1. To obtain p_b: Open poe.com, press F12 to open the debugging tool, then select the application. You can find the value of p_b in the cookies.  
+    2. To obtain formkey: Open poe.com, press F12 to open the debugging tool, then select Network. After chatting with a bot, you can see the gqlpost network request. Within the request headers, there is a separate key-value pair for the formkey.
 
 ## Step 1: Import the library and create a Poe_Client object
 
 If you don't formkey to the Poe_Client, you need to install node.js for generate form key.
 Here is the download link.[node.js](https://nodejs.org/en)
 
 Before you can use any functionality of the `Poe_Client` library, you first need to import the library and create
```

### Comparing `async_poe_client-0.2.0/PKG-INFO` & `async_poe_client-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-poe-client
-Version: 0.2.0
+Version: 0.2.1
 Summary: A stable, fast and convenient async client for poe.com
 Author: canxin
 Author-email: 1969730106@qq.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -14,16 +14,16 @@
 Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
 Requires-Dist: aiohttp-socks (>=0.8.0,<0.9.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: pyexecjs2 (>=1.6.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # User Guide
-
-[中文版本](README_zh_CN.md)
+latest version:0.1.9  
+[中文使用指南](README_zh_CN.md)
 
 This is a guide on how to use the `async-poe-Client` library. Before starting, make sure you've installed this library.
 
 ```
 pip install async-poe-client
 ```
 
@@ -55,14 +55,17 @@
   The relationship between this url_botname and other names can be understood as:  
     1. For the system's built-in bots, the name of the bot you see on the poe web page and the url_botname are always
        equal (but neither equals the handle).
     2. For bots you create, url_botname = handle. If display_name is set, the name you see on the web page is display_name;
        if not set, you see url_botname (handle).
        However, there are special cases where the handle does not follow the above rules, such as the handle of all bots
        obtained using get_available_bots always equals url_botname.
+- 2.How to obtain p_b and formkey? ->  
+    1. To obtain p_b: Open poe.com, press F12 to open the debugging tool, then select the application. You can find the value of p_b in the cookies.  
+    2. To obtain formkey: Open poe.com, press F12 to open the debugging tool, then select Network. After chatting with a bot, you can see the gqlpost network request. Within the request headers, there is a separate key-value pair for the formkey.
 
 ## Step 1: Import the library and create a Poe_Client object
 
 If you don't formkey to the Poe_Client, you need to install node.js for generate form key.
 Here is the download link.[node.js](https://nodejs.org/en)
 
 Before you can use any functionality of the `Poe_Client` library, you first need to import the library and create
```

