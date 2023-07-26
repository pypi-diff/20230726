# Comparing `tmp/playgroundrl-0.0.8.tar.gz` & `tmp/playgroundrl-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playgroundrl-0.0.8.tar", last modified: Tue Apr 11 19:54:28 2023, max compression
+gzip compressed data, was "playgroundrl-0.1.0.tar", last modified: Wed Jul 26 19:07:17 2023, max compression
```

## Comparing `playgroundrl-0.0.8.tar` & `playgroundrl-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-04-11 19:54:28.830499 playgroundrl-0.0.8/
--rw-r--r--   0 langston   (501) staff       (20)      170 2023-04-11 19:54:28.830595 playgroundrl-0.0.8/PKG-INFO
--rw-r--r--   0 langston   (501) staff       (20)      162 2023-04-08 20:30:44.000000 playgroundrl-0.0.8/README.md
--rw-r--r--   0 langston   (501) staff       (20)       38 2023-04-11 19:54:28.830778 playgroundrl-0.0.8/setup.cfg
--rw-r--r--   0 langston   (501) staff       (20)      443 2023-04-11 19:53:51.000000 playgroundrl-0.0.8/setup.py
-drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-04-11 19:54:28.827894 playgroundrl-0.0.8/src/
-drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-04-11 19:54:28.829229 playgroundrl-0.0.8/src/playgroundrl/
--rw-r--r--   0 langston   (501) staff       (20)        0 2023-04-08 20:30:44.000000 playgroundrl-0.0.8/src/playgroundrl/__init__.py
--rw-r--r--   0 langston   (501) staff       (20)     8938 2023-04-11 19:53:08.000000 playgroundrl-0.0.8/src/playgroundrl/client.py
--rw-r--r--   0 langston   (501) staff       (20)     5104 2023-04-08 21:07:04.000000 playgroundrl-0.0.8/src/playgroundrl/state.py
-drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-04-11 19:54:28.830335 playgroundrl-0.0.8/src/playgroundrl.egg-info/
--rw-r--r--   0 langston   (501) staff       (20)      170 2023-04-11 19:54:28.000000 playgroundrl-0.0.8/src/playgroundrl.egg-info/PKG-INFO
--rw-r--r--   0 langston   (501) staff       (20)      309 2023-04-11 19:54:28.000000 playgroundrl-0.0.8/src/playgroundrl.egg-info/SOURCES.txt
--rw-r--r--   0 langston   (501) staff       (20)        1 2023-04-11 19:54:28.000000 playgroundrl-0.0.8/src/playgroundrl.egg-info/dependency_links.txt
--rw-r--r--   0 langston   (501) staff       (20)       52 2023-04-11 19:54:28.000000 playgroundrl-0.0.8/src/playgroundrl.egg-info/requires.txt
--rw-r--r--   0 langston   (501) staff       (20)       13 2023-04-11 19:54:28.000000 playgroundrl-0.0.8/src/playgroundrl.egg-info/top_level.txt
+drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-07-26 19:07:17.092923 playgroundrl-0.1.0/
+-rw-r--r--   0 rayan      (501) staff       (20)      170 2023-07-26 19:07:17.092966 playgroundrl-0.1.0/PKG-INFO
+-rw-r--r--   0 rayan      (501) staff       (20)      452 2023-07-25 01:29:43.000000 playgroundrl-0.1.0/README.md
+-rw-r--r--   0 rayan      (501) staff       (20)       38 2023-07-26 19:07:17.093125 playgroundrl-0.1.0/setup.cfg
+-rw-r--r--   0 rayan      (501) staff       (20)      456 2023-07-26 19:07:01.000000 playgroundrl-0.1.0/setup.py
+drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-07-26 19:07:17.090927 playgroundrl-0.1.0/src/
+drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-07-26 19:07:17.092157 playgroundrl-0.1.0/src/playgroundrl/
+-rw-r--r--   0 rayan      (501) staff       (20)        0 2023-02-27 07:47:18.000000 playgroundrl-0.1.0/src/playgroundrl/__init__.py
+-rw-r--r--   0 rayan      (501) staff       (20)     1313 2023-07-25 01:29:43.000000 playgroundrl-0.1.0/src/playgroundrl/actions.py
+-rw-r--r--   0 rayan      (501) staff       (20)    13029 2023-07-26 19:03:20.000000 playgroundrl-0.1.0/src/playgroundrl/client.py
+-rw-r--r--   0 rayan      (501) staff       (20)     5421 2023-07-25 01:29:43.000000 playgroundrl-0.1.0/src/playgroundrl/state.py
+-rw-r--r--   0 rayan      (501) staff       (20)      418 2023-06-29 23:39:57.000000 playgroundrl-0.1.0/src/playgroundrl/util.py
+drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-07-26 19:07:17.092830 playgroundrl-0.1.0/src/playgroundrl.egg-info/
+-rw-r--r--   0 rayan      (501) staff       (20)      170 2023-07-26 19:07:17.000000 playgroundrl-0.1.0/src/playgroundrl.egg-info/PKG-INFO
+-rw-r--r--   0 rayan      (501) staff       (20)      362 2023-07-26 19:07:17.000000 playgroundrl-0.1.0/src/playgroundrl.egg-info/SOURCES.txt
+-rw-r--r--   0 rayan      (501) staff       (20)        1 2023-07-26 19:07:17.000000 playgroundrl-0.1.0/src/playgroundrl.egg-info/dependency_links.txt
+-rw-r--r--   0 rayan      (501) staff       (20)       52 2023-07-26 19:07:17.000000 playgroundrl-0.1.0/src/playgroundrl.egg-info/requires.txt
+-rw-r--r--   0 rayan      (501) staff       (20)       13 2023-07-26 19:07:17.000000 playgroundrl-0.1.0/src/playgroundrl.egg-info/top_level.txt
```

### Comparing `playgroundrl-0.0.8/src/playgroundrl/state.py` & `playgroundrl-0.1.0/src/playgroundrl/state.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,52 @@
-import attrs 
+import attrs
 from typing import List, Dict
+
 """
 Module with various game state representations
 """
 
+
 @attrs.define
-class GameState():
+class GameState:
     player_moving: str
     """user_id of player who's current turn it is"""
 
     model_name: str
     """name of model who's turn it is next"""
 
     player_moving_id: int
     """Player id of the player / model who's turn it is next"""
 
+
 @attrs.define
 class ChessState(GameState):
-    fen: str 
+    fen: str
     """FEN representation of current board state"""
 
 
 @attrs.define
 class SnakeState(GameState):
     apple: List[int]
     """(x, y) of apple"""
 
     snake: List[List[int]]
     """[(x1, y1), (x2, y2), ... of snake's coordinates]"""
 
 
 @attrs.define
+class MiningDecarbonizationState(GameState):
+    mined_resources: List[List[float]]
+    """2D array with values from 0 to 1 indicating the resources mined in the last turn for each tile"""
+
+    emissions: List[List[float]]
+    """2D array with values from 0 to 1 indicating the emissions produced in the last turn for each tile"""
+
+
+@attrs.define
 class TicTacToeState(GameState):
     board: List[List[int]]
     """Current tic tac toe board"""
 
     # player_id: int
 
 
@@ -81,63 +93,62 @@
 
     longest_roads_by_player: Dict[str, int]
     """length of the longest roads for each player"""
 
     winning_color: str
     """null if the game is not over, or a player color if someone has won"""
 
+
 # Card is represented as suit (s, c, h, d)
-# concatenated with two 
+# concatenated with two
 # digit rank (2 - 14)
 Card = str
 PokerHand = List[Card]
 PlayerId = int
 
 
 @attrs.define
-class RoundOutcome():
+class RoundOutcome:
     hands: Dict[PlayerId, PokerHand]
     """Mapping of player id to hand in last round"""
 
     winnings: Dict[PlayerId, int]
     """Mapping of player id to total amount won in last round"""
 
+
 @attrs.define
 class PokerState(GameState):
-
     communal_cards: List[Card]
     """Board cards"""
 
     chip_counts = Dict[PlayerId, int]
     """Chip counts for all players"""
 
     amounts_bet = Dict[PlayerId, int]
     """Amount the player has bet for current round of betting"""
 
     user_ids = Dict[PlayerId, str]
     """User IDs of each player, useful for utility printing"""
-    
+
     can_raise: bool
     """In certain unique situations, raising is disabled"""
 
     hand_number: int
     """Which hand we're on (starts at 0, strictly increases)"""
 
     players_left_in_hand: int
     """How many players that have not folded"""
 
     status: str
     """(player specific) -- status of current player (IN, OUT, TO_CALL, ALL_IN, )"""
 
-
     pot_size: str
     """(player specific) Size of the pot this player is eligible for (always the global pot, 
         except in certain all-in cases)"""
 
-
     chips_to_call: int
     """How many chips the player needs to put in to call the next bet (only applicable of state is TO_CALL)"""
 
     hole_cards: PokerHand
     """Player's secret cards"""
 
     position: int
@@ -163,38 +174,38 @@
 class CodenamesState(GameState):
     color: str
     """Color of player receiving state"""
 
     role: str
     """Role of player receiving state (giver / guesser)"""
 
-    words: List[List[str]]
+    words: List[str]
     """
     5x5 array of words representing board
     """
 
-    guessed: List[List[str]]
+    guessed: List[str]
     """
     Colors revealed already through guesses.
     BLUE / RED / INNOCENT / ASSASSIN / UNKNOWN
     """
 
-    actual: List[List[str]]
+    actual: List[str]
     """
     For giver, the actual values for each tile
     For guesser, the same as guessed. 
     """
 
     clue: str
     """
     Most recently given clue (one word)
     """
-    
+
     count: int
     """
     Count for most recent clue
     """
 
     scores: Dict[str, int]
     """
     Color to score mapping
-    """
+    """
```

