# Comparing `tmp/PlexTraktSync-0.26.8.tar.gz` & `tmp/PlexTraktSync-0.26.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/PlexTraktSync/PlexTraktSync/dist/.tmp-w2462gqq/PlexTraktSync-0.26.8.tar", last modified: Wed Jun 28 19:11:34 2023, max compression
+gzip compressed data, was "/home/runner/work/PlexTraktSync/PlexTraktSync/dist/.tmp-obe_p52z/PlexTraktSync-0.26.9.tar", last modified: Wed Jul 26 12:57:34 2023, max compression
```

## Comparing `PlexTraktSync-0.26.8.tar` & `PlexTraktSync-0.26.9.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 19:11:34.000000 PlexTraktSync-0.26.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19069 2023-06-28 19:11:34.000000 PlexTraktSync-0.26.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 19:11:34.000000 PlexTraktSync-0.26.8/PlexTraktSync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19069 2023-06-28 19:11:34.000000 PlexTraktSync-0.26.8/PlexTraktSync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-06-28 19:11:34.000000 PlexTraktSync-0.26.8/PlexTraktSync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 19:11:34.000000 PlexTraktSync-0.26.8/PlexTraktSync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-28 19:11:34.000000 PlexTraktSync-0.26.8/PlexTraktSync.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-28 19:11:34.000000 PlexTraktSync-0.26.8/PlexTraktSync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-28 19:11:34.000000 PlexTraktSync-0.26.8/PlexTraktSync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18219 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 19:11:34.000000 PlexTraktSync-0.26.8/plextraktsync/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-28 19:11:23.000000 PlexTraktSync-0.26.8/plextraktsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 19:11:34.000000 PlexTraktSync-0.26.8/plextraktsync/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/commands/bug_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/commands/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/commands/clear_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/commands/imdb_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/commands/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/commands/plex_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/commands/self_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/commands/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/commands/trakt_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/commands/unmatched.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/commands/watch.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/commands/watched_shows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 19:11:34.000000 PlexTraktSync-0.26.8/plextraktsync/config/
--rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/config/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/config/ConfigLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/config/ConfigMergeMixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/config/HttpCacheConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/config/PlexServerConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/config/RunConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/config/ServerConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/config/SyncConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/config.default.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 19:11:34.000000 PlexTraktSync-0.26.8/plextraktsync/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/decorators/cached_property.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/decorators/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/decorators/http_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/decorators/measure_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/decorators/memoize.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/decorators/nocache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/decorators/rate_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/decorators/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/decorators/time_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 19:11:34.000000 PlexTraktSync-0.26.8/plextraktsync/logger/
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/logger/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/media.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 19:11:34.000000 PlexTraktSync-0.26.8/plextraktsync/mixin/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/mixin/ChangeNotifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 19:11:34.000000 PlexTraktSync-0.26.8/plextraktsync/plex/
--rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/plex/PlexApi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/plex/PlexAudioCodec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/plex/PlexGuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/plex/PlexLibraryItem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/plex/PlexLibrarySection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/plex/PlexRatings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/plex/PlexServerConnection.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/plex/PlexWatchList.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/plex/SessionCollection.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/plex/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/pytrakt_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 19:11:34.000000 PlexTraktSync-0.26.8/plextraktsync/queue/
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/queue/BackgroundTask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/queue/Queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/queue/TraktBatchWorker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/queue/TraktMarkWatchedWorker.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/rich_addons.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/servers.default.yml
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/style.py
--rw-r--r--   0 runner    (1001) docker     (123)    11131 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 19:11:34.000000 PlexTraktSync-0.26.8/plextraktsync/trakt/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/trakt/PartialTraktMedia.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/trakt/ScrobblerCollection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/trakt/ScrobblerProxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/trakt/TraktApi.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/trakt/TraktItem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/trakt/TraktLookup.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/trakt/TraktRatingCollection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/trakt/TraktWatchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/trakt/trakt_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/trakt/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/trakt_list_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 19:11:34.000000 PlexTraktSync-0.26.8/plextraktsync/util/
--rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/util/Factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/util/Path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/util/Timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/util/Version.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/util/execp.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/util/execx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/util/expand_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/util/git_version_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/util/local_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/util/openurl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/util/packaging.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/util/parse_date.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/util/remove_empty_values.py
--rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/walker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 19:11:34.000000 PlexTraktSync-0.26.8/plextraktsync/watch/
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/watch/EventDispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/watch/EventFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/watch/ProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/watch/WatchStateUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/watch/WebSocketListener.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/plextraktsync/watch/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-28 19:11:28.000000 PlexTraktSync-0.26.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-28 19:11:34.000000 PlexTraktSync-0.26.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 19:11:34.000000 PlexTraktSync-0.26.8/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1923 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/tests/test_collection_metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1443 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/tests/test_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2703 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/tests/test_events.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      299 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/tests/test_logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      977 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/tests/test_new_agent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      442 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/tests/test_plex_search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/tests/test_threading.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1174 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/tests/test_timer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      572 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/tests/test_trakt_progress.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3584 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/tests/test_tv_lookup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1926 2023-06-28 19:11:22.000000 PlexTraktSync-0.26.8/tests/test_walker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:57:34.000000 PlexTraktSync-0.26.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19069 2023-07-26 12:57:34.000000 PlexTraktSync-0.26.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:57:34.000000 PlexTraktSync-0.26.9/PlexTraktSync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19069 2023-07-26 12:57:34.000000 PlexTraktSync-0.26.9/PlexTraktSync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-07-26 12:57:34.000000 PlexTraktSync-0.26.9/PlexTraktSync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:57:34.000000 PlexTraktSync-0.26.9/PlexTraktSync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 12:57:34.000000 PlexTraktSync-0.26.9/PlexTraktSync.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-26 12:57:34.000000 PlexTraktSync-0.26.9/PlexTraktSync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-26 12:57:34.000000 PlexTraktSync-0.26.9/PlexTraktSync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18219 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:57:34.000000 PlexTraktSync-0.26.9/plextraktsync/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:57:34.000000 PlexTraktSync-0.26.9/plextraktsync/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/commands/bug_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/commands/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/commands/clear_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/commands/imdb_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/commands/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/commands/plex_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/commands/self_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/commands/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/commands/trakt_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/commands/unmatched.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/commands/watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/commands/watched_shows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:57:34.000000 PlexTraktSync-0.26.9/plextraktsync/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/config/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/config/ConfigLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/config/ConfigMergeMixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/config/HttpCacheConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/config/PlexServerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/config/RunConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/config/ServerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/config/SyncConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/config.default.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:57:34.000000 PlexTraktSync-0.26.9/plextraktsync/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/decorators/cached_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/decorators/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/decorators/http_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/decorators/measure_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/decorators/memoize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/decorators/nocache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/decorators/rate_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/decorators/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/decorators/time_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:57:34.000000 PlexTraktSync-0.26.9/plextraktsync/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/logger/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/media.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:57:34.000000 PlexTraktSync-0.26.9/plextraktsync/mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/mixin/ChangeNotifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:57:34.000000 PlexTraktSync-0.26.9/plextraktsync/plex/
+-rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/plex/PlexApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/plex/PlexAudioCodec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/plex/PlexGuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/plex/PlexLibraryItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/plex/PlexLibrarySection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/plex/PlexRatings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/plex/PlexServerConnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/plex/PlexWatchList.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/plex/SessionCollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/plex/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/pytrakt_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:57:34.000000 PlexTraktSync-0.26.9/plextraktsync/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/queue/BackgroundTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/queue/Queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/queue/TraktBatchWorker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/queue/TraktMarkWatchedWorker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/rich_addons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/servers.default.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11131 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:57:34.000000 PlexTraktSync-0.26.9/plextraktsync/trakt/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/trakt/PartialTraktMedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/trakt/ScrobblerCollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/trakt/ScrobblerProxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/trakt/TraktApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/trakt/TraktItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/trakt/TraktLookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/trakt/TraktRatingCollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/trakt/TraktWatchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/trakt/trakt_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/trakt/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/trakt_list_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:57:34.000000 PlexTraktSync-0.26.9/plextraktsync/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/util/Factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/util/Path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/util/Timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/util/Version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/util/execp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/util/execx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/util/expand_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/util/git_version_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/util/local_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/util/openurl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/util/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/util/parse_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/util/remove_empty_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/walker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:57:34.000000 PlexTraktSync-0.26.9/plextraktsync/watch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/watch/EventDispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/watch/EventFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/watch/ProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/watch/WatchStateUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/watch/WebSocketListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/plextraktsync/watch/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-26 12:57:27.000000 PlexTraktSync-0.26.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-26 12:57:34.000000 PlexTraktSync-0.26.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:57:34.000000 PlexTraktSync-0.26.9/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1923 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/tests/test_collection_metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1443 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/tests/test_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2703 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/tests/test_events.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      299 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/tests/test_logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      977 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/tests/test_new_agent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      442 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/tests/test_plex_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/tests/test_threading.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1174 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/tests/test_timer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      572 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/tests/test_trakt_progress.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3584 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/tests/test_tv_lookup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1926 2023-07-26 12:57:21.000000 PlexTraktSync-0.26.9/tests/test_walker.py
```

### Comparing `PlexTraktSync-0.26.8/LICENSE` & `PlexTraktSync-0.26.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/PKG-INFO` & `PlexTraktSync-0.26.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexTraktSync
-Version: 0.26.8
+Version: 0.26.9
 Summary: Plex-Trakt-Sync is a two-way-sync between trakt.tv and Plex Media Server
 Home-page: https://github.com/Taxel/PlexTraktSync
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Taxel/PlexTraktSync/issues
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PlexTraktSync-0.26.8/PlexTraktSync.egg-info/PKG-INFO` & `PlexTraktSync-0.26.9/PlexTraktSync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexTraktSync
-Version: 0.26.8
+Version: 0.26.9
 Summary: Plex-Trakt-Sync is a two-way-sync between trakt.tv and Plex Media Server
 Home-page: https://github.com/Taxel/PlexTraktSync
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Taxel/PlexTraktSync/issues
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PlexTraktSync-0.26.8/PlexTraktSync.egg-info/SOURCES.txt` & `PlexTraktSync-0.26.9/PlexTraktSync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/PlexTraktSync.egg-info/requires.txt` & `PlexTraktSync-0.26.9/PlexTraktSync.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 attrs==23.1.0
 certifi==2023.5.7
-charset-normalizer==3.1.0
-click==8.1.3
+charset-normalizer==3.2.0
+click==8.1.4
 deprecated==1.2.14
 inquirerpy==0.3.4
 oauthlib==3.2.2
 plexapi==4.14.0
-prompt-toolkit==3.0.38
+prompt-toolkit==3.0.39
 pygments==2.15.1
 python-dotenv==0.21.1
 python-git-info==0.8.3
 pytimeparse==1.1.8
 pytrakt==3.4.23
-pyyaml==6.0
+pyyaml==6.0.1
 requests-cache==1.0.0b1
 requests==2.31.0
 rich==13.4.2
 tqdm==4.65.0
 urllib3==2.0.3
 wcwidth==0.2.6
 websocket-client==1.6.1
@@ -35,11 +35,11 @@
 [:python_version >= "3.6"]
 url-normalize==1.4.3
 
 [:python_version >= "3.7"]
 cattrs==23.1.2
 markdown-it-py==2.2.0
 mdurl==0.1.2
-platformdirs==3.8.0
+platformdirs==3.9.1
 
 [:python_version >= "3.7" and python_version < "4.0"]
 pfzy==0.3.4
```

### Comparing `PlexTraktSync-0.26.8/README.md` & `PlexTraktSync-0.26.9/README.md`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/cli.py` & `PlexTraktSync-0.26.9/plextraktsync/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from functools import wraps
 from os import environ
 
 import click
+from click import ClickException
 
 from plextraktsync.factory import factory
 
 
 def command():
     """
     Wrapper to lazy load commands when commands being executed only
@@ -19,19 +20,21 @@
 
             name = fn.__name__
             module = importlib.import_module(f".commands.{name}", package=__package__)
             cmd = getattr(module, name)
 
             try:
                 cmd(*args, **kwargs)
+            except ClickException as e:
+                from plextraktsync.factory import logger
+                logger.fatal(f"Error running {name} command: {str(e)}")
             except Exception as e:
                 from plextraktsync.factory import logger
                 logger.exception(e)
 
-                from click import ClickException
                 raise ClickException(f"Error running {name} command: {str(e)}")
 
         return wrap
 
     return decorator
```

### Comparing `PlexTraktSync-0.26.8/plextraktsync/commands/bug_report.py` & `PlexTraktSync-0.26.9/plextraktsync/commands/bug_report.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/commands/cache.py` & `PlexTraktSync-0.26.9/plextraktsync/commands/cache.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/commands/clear_collections.py` & `PlexTraktSync-0.26.9/plextraktsync/commands/clear_collections.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/commands/config.py` & `PlexTraktSync-0.26.9/plextraktsync/commands/config.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/commands/download.py` & `PlexTraktSync-0.26.9/plextraktsync/commands/download.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/commands/imdb_import.py` & `PlexTraktSync-0.26.9/plextraktsync/commands/imdb_import.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/commands/info.py` & `PlexTraktSync-0.26.9/plextraktsync/commands/info.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/commands/inspect.py` & `PlexTraktSync-0.26.9/plextraktsync/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/commands/login.py` & `PlexTraktSync-0.26.9/plextraktsync/commands/login.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/commands/plex_login.py` & `PlexTraktSync-0.26.9/plextraktsync/commands/plex_login.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/commands/self_update.py` & `PlexTraktSync-0.26.9/plextraktsync/commands/self_update.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/commands/sync.py` & `PlexTraktSync-0.26.9/plextraktsync/commands/sync.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/commands/trakt_login.py` & `PlexTraktSync-0.26.9/plextraktsync/commands/trakt_login.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/commands/unmatched.py` & `PlexTraktSync-0.26.9/plextraktsync/commands/unmatched.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/commands/watch.py` & `PlexTraktSync-0.26.9/plextraktsync/commands/watch.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/commands/watched_shows.py` & `PlexTraktSync-0.26.9/plextraktsync/commands/watched_shows.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/config/Config.py` & `PlexTraktSync-0.26.9/plextraktsync/config/Config.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/config/ConfigLoader.py` & `PlexTraktSync-0.26.9/plextraktsync/config/ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/config/HttpCacheConfig.py` & `PlexTraktSync-0.26.9/plextraktsync/config/HttpCacheConfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         "*/library/sections/*/collections": DO_NOT_CACHE,
         # library_sections
         "*/library/sections": DO_NOT_CACHE,
 
         # reloads
         "*/library/metadata/*?*include*": DO_NOT_CACHE,
         # episodes
-        "*/library/metadata/*/allLeaves": DO_NOT_CACHE,
+        "*/library/sections/*/all?includeGuids=1&type=4*": DO_NOT_CACHE,
         # find_by_id
         "*/library/metadata/*": DO_NOT_CACHE,
         # mark played, mark unplayed
         "*/:/scrobble?key=*&identifier=com.plexapp.plugins.library": DO_NOT_CACHE,
         "*/:/unscrobble?key=&&identifier=com.plexapp.plugins.library": DO_NOT_CACHE,
         # playlists
         "*/playlists?title=": DO_NOT_CACHE,
```

### Comparing `PlexTraktSync-0.26.8/plextraktsync/config/ServerConfig.py` & `PlexTraktSync-0.26.9/plextraktsync/config/ServerConfig.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/config/SyncConfig.py` & `PlexTraktSync-0.26.9/plextraktsync/config/SyncConfig.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/config.default.yml` & `PlexTraktSync-0.26.9/plextraktsync/config.default.yml`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/decorators/rate_limit.py` & `PlexTraktSync-0.26.9/plextraktsync/decorators/rate_limit.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/decorators/retry.py` & `PlexTraktSync-0.26.9/plextraktsync/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/logger/filter.py` & `PlexTraktSync-0.26.9/plextraktsync/logger/filter.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/logging.py` & `PlexTraktSync-0.26.9/plextraktsync/logging.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/media.py` & `PlexTraktSync-0.26.9/plextraktsync/media.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/mixin/ChangeNotifier.py` & `PlexTraktSync-0.26.9/plextraktsync/mixin/ChangeNotifier.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/plex/PlexApi.py` & `PlexTraktSync-0.26.9/plextraktsync/plex/PlexApi.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/plex/PlexAudioCodec.py` & `PlexTraktSync-0.26.9/plextraktsync/plex/PlexAudioCodec.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/plex/PlexGuid.py` & `PlexTraktSync-0.26.9/plextraktsync/plex/PlexGuid.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/plex/PlexLibraryItem.py` & `PlexTraktSync-0.26.9/plextraktsync/plex/PlexLibraryItem.py`

 * *Files 2% similar despite different names*

```diff
@@ -279,15 +279,15 @@
 
     def episodes(self):
         for ep in self._get_episodes():
             yield PlexLibraryItem(ep, plex=self.plex)
 
     @retry()
     def _get_episodes(self):
-        return self.item.episodes()
+        return self.library.search(libtype='episode', filters={'show.id': self.item.ratingKey})
 
     @cached_property
     def season_number(self):
         return self.item.seasonNumber
 
     @cached_property
     def episode_number(self):
```

### Comparing `PlexTraktSync-0.26.8/plextraktsync/plex/PlexLibrarySection.py` & `PlexTraktSync-0.26.9/plextraktsync/plex/PlexLibrarySection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/plex/PlexRatings.py` & `PlexTraktSync-0.26.9/plextraktsync/plex/PlexRatings.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/plex/PlexServerConnection.py` & `PlexTraktSync-0.26.9/plextraktsync/plex/PlexServerConnection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/plex/PlexWatchList.py` & `PlexTraktSync-0.26.9/plextraktsync/plex/PlexWatchList.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/plex/SessionCollection.py` & `PlexTraktSync-0.26.9/plextraktsync/plex/SessionCollection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/pytrakt_extensions.py` & `PlexTraktSync-0.26.9/plextraktsync/pytrakt_extensions.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/queue/BackgroundTask.py` & `PlexTraktSync-0.26.9/plextraktsync/queue/BackgroundTask.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/queue/Queue.py` & `PlexTraktSync-0.26.9/plextraktsync/queue/Queue.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/queue/TraktBatchWorker.py` & `PlexTraktSync-0.26.9/plextraktsync/queue/TraktBatchWorker.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/queue/TraktMarkWatchedWorker.py` & `PlexTraktSync-0.26.9/plextraktsync/queue/TraktMarkWatchedWorker.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/rich_addons.py` & `PlexTraktSync-0.26.9/plextraktsync/rich_addons.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/sync.py` & `PlexTraktSync-0.26.9/plextraktsync/sync.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/trakt/ScrobblerCollection.py` & `PlexTraktSync-0.26.9/plextraktsync/trakt/ScrobblerCollection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/trakt/ScrobblerProxy.py` & `PlexTraktSync-0.26.9/plextraktsync/trakt/ScrobblerProxy.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/trakt/TraktApi.py` & `PlexTraktSync-0.26.9/plextraktsync/trakt/TraktApi.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,16 +48,15 @@
     @cached_property
     @rate_limit()
     @retry()
     def me(self):
         try:
             return trakt.users.User("me")
         except (OAuthException, ForbiddenException) as e:
-            logger.fatal(f"Trakt authentication error: {str(e)}")
-            raise ClickException(e)
+            raise ClickException(f"Trakt authentication error: {str(e)}")
 
     @cached_property
     @rate_limit()
     @retry()
     @flatten_list
     def liked_lists(self):
         for item in self.me.get_liked_lists("lists", limit=1000):
```

### Comparing `PlexTraktSync-0.26.8/plextraktsync/trakt/TraktItem.py` & `PlexTraktSync-0.26.9/plextraktsync/trakt/TraktItem.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/trakt/TraktLookup.py` & `PlexTraktSync-0.26.9/plextraktsync/trakt/TraktLookup.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/trakt/TraktRatingCollection.py` & `PlexTraktSync-0.26.9/plextraktsync/trakt/TraktRatingCollection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/trakt/TraktWatchlist.py` & `PlexTraktSync-0.26.9/plextraktsync/trakt/TraktWatchlist.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/trakt_list_util.py` & `PlexTraktSync-0.26.9/plextraktsync/trakt_list_util.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/util/Factory.py` & `PlexTraktSync-0.26.9/plextraktsync/util/Factory.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/util/Path.py` & `PlexTraktSync-0.26.9/plextraktsync/util/Path.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/util/Timer.py` & `PlexTraktSync-0.26.9/plextraktsync/util/Timer.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/util/Version.py` & `PlexTraktSync-0.26.9/plextraktsync/util/Version.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/util/expand_id.py` & `PlexTraktSync-0.26.9/plextraktsync/util/expand_id.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/util/local_url.py` & `PlexTraktSync-0.26.9/plextraktsync/util/local_url.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/util/openurl.py` & `PlexTraktSync-0.26.9/plextraktsync/util/openurl.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/util/packaging.py` & `PlexTraktSync-0.26.9/plextraktsync/util/packaging.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/util/remove_empty_values.py` & `PlexTraktSync-0.26.9/plextraktsync/util/remove_empty_values.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/walker.py` & `PlexTraktSync-0.26.9/plextraktsync/walker.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     def add_movie(self, movie):
         self.movie.append(movie)
 
     @property
     def is_partial(self):
         """
         Returns true if partial library walk is performed.
-        Due the way watchlist is filled, watchlists should only be updated on full walk.
+        Due to the way watchlist is filled, watchlists should only be updated on full walk.
         """
         # Single item provided
         if self.library or self.movie or self.show or self.id:
             return True
 
         # Must sync both movies and shows to be full sync
         return not self.walk_movies or not self.walk_shows
```

### Comparing `PlexTraktSync-0.26.8/plextraktsync/watch/EventDispatcher.py` & `PlexTraktSync-0.26.9/plextraktsync/watch/EventDispatcher.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/watch/EventFactory.py` & `PlexTraktSync-0.26.9/plextraktsync/watch/EventFactory.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/watch/ProgressBar.py` & `PlexTraktSync-0.26.9/plextraktsync/watch/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/watch/WatchStateUpdater.py` & `PlexTraktSync-0.26.9/plextraktsync/watch/WatchStateUpdater.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/watch/WebSocketListener.py` & `PlexTraktSync-0.26.9/plextraktsync/watch/WebSocketListener.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/plextraktsync/watch/events.py` & `PlexTraktSync-0.26.9/plextraktsync/watch/events.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/requirements.txt` & `PlexTraktSync-0.26.9/requirements.txt`

 * *Files 9% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 #    pipenv lock --requirements
 #
 
 attrs==23.1.0
 backports.cached-property==1.0.2; python_version <= '3.7'
 cattrs==23.1.2; python_version >= '3.7'
 certifi==2023.5.7
-charset-normalizer==3.1.0
-click==8.1.3
+charset-normalizer==3.2.0
+click==8.1.4
 deprecated==1.2.14
 idna==3.4; python_version >= '3.5'
 inquirerpy==0.3.4
 markdown-it-py==2.2.0; python_version >= '3.7'
 mdurl==0.1.2; python_version >= '3.7'
 oauthlib==3.2.2
 pfzy==0.3.4; python_version >= '3.7' and python_version < '4.0'
-platformdirs==3.8.0; python_version >= '3.7'
+platformdirs==3.9.1; python_version >= '3.7'
 plexapi==4.14.0
-prompt-toolkit==3.0.38
+prompt-toolkit==3.0.39
 pygments==2.15.1
 python-dotenv==0.21.1
 python-git-info==0.8.3
 pytimeparse==1.1.8
 pytrakt==3.4.23
-pyyaml==6.0
+pyyaml==6.0.1
 requests-cache==1.0.0b1
 requests-oauthlib==1.3.1; python_version >= '3.4'
 requests==2.31.0
 rich==13.4.2
 six==1.16.0; python_version >= '3.4'
 tqdm==4.65.0
 url-normalize==1.4.3; python_version >= '3.6'
```

### Comparing `PlexTraktSync-0.26.8/setup.cfg` & `PlexTraktSync-0.26.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/tests/test_collection_metadata.py` & `PlexTraktSync-0.26.9/tests/test_collection_metadata.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/tests/test_config.py` & `PlexTraktSync-0.26.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/tests/test_events.py` & `PlexTraktSync-0.26.9/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/tests/test_new_agent.py` & `PlexTraktSync-0.26.9/tests/test_new_agent.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/tests/test_timer.py` & `PlexTraktSync-0.26.9/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/tests/test_trakt_progress.py` & `PlexTraktSync-0.26.9/tests/test_trakt_progress.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/tests/test_tv_lookup.py` & `PlexTraktSync-0.26.9/tests/test_tv_lookup.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.8/tests/test_walker.py` & `PlexTraktSync-0.26.9/tests/test_walker.py`

 * *Files identical despite different names*

