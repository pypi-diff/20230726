# Comparing `tmp/atriumsports_sdk-1.3.2.tar.gz` & `tmp/atriumsports_sdk-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atriumsports_sdk-1.3.2.tar", last modified: Mon Jul 10 10:51:03 2023, max compression
+gzip compressed data, was "atriumsports_sdk-1.4.0.tar", last modified: Wed Jul 26 16:44:04 2023, max compression
```

## Comparing `atriumsports_sdk-1.3.2.tar` & `atriumsports_sdk-1.4.0.tar`

### file list

```diff
@@ -1,436 +1,438 @@
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-10 10:51:03.930160 atriumsports_sdk-1.3.2/
--rw-r--r--   0 k.kieda    (502) staff       (20)     1074 2023-03-17 13:13:15.000000 atriumsports_sdk-1.3.2/LICENSE
--rw-r--r--   0 k.kieda    (502) staff       (20)     5380 2023-07-10 10:51:03.929678 atriumsports_sdk-1.3.2/PKG-INFO
--rw-r--r--   0 k.kieda    (502) staff       (20)     4963 2023-06-16 15:49:48.000000 atriumsports_sdk-1.3.2/README.md
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-10 10:51:03.626665 atriumsports_sdk-1.3.2/atriumsports/
--rw-r--r--   0 k.kieda    (502) staff       (20)     1096 2023-03-17 13:13:15.000000 atriumsports_sdk-1.3.2/atriumsports/__init__.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4294 2023-04-24 10:52:41.000000 atriumsports_sdk-1.3.2/atriumsports/atrium_response.py
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-10 10:51:03.628432 atriumsports_sdk-1.3.2/atriumsports/datacore/
--rw-r--r--   0 k.kieda    (502) staff       (20)        0 2022-11-21 11:07:25.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/__init__.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6660 2023-04-24 10:52:41.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/datacore.py
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-10 10:51:03.633136 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/
--rw-r--r--   0 k.kieda    (502) staff       (20)    54651 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/__init__.py
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-10 10:51:03.682530 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/
--rw-r--r--   0 k.kieda    (502) staff       (20)     4630 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/__init__.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   121018 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/awards_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    59847 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/career_statistics_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    18925 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/change_log_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    97107 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/competition_statistics_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   127164 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/competitions_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    78128 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/conduct_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   137833 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/conferences_divisions_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    66311 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/download_video_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    91278 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/entities_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    21039 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/entity_fixture_history_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   127554 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/entity_fixture_statistics_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    70185 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/entity_groups_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    59444 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixture_entities_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11205 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixture_live_summary_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    59323 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixture_persons_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    77945 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixture_playbyplay_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    72387 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixture_profiles_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    76686 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixture_progressions_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    89352 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixture_roster_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   407884 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixtures_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   252466 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/images_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    70633 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/leader_criteria_sets_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    73398 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/leader_qualifiers_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    70024 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/leagues_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    73817 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/local_video_endpoints_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    70215 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/merge_records_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    66029 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/organizations_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    36028 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/partner_apis_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    23558 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/person_fixture_history_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   134432 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/person_fixture_statistics_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    91522 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/persons_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   107461 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/rankings_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   150045 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/roles_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    77289 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_entities_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    49629 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_entity_base_statistics_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    71603 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_entity_placings_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    44646 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_leaders_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    50867 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_person_base_statistics_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    71598 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_person_placings_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    77803 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_persons_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    97800 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_roster_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    90287 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_series_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   177700 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_statistics_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   120275 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/seasons_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    68423 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/sites_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   229910 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/stages_pools_rounds_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    76768 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/standing_adjustments_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    71710 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/standing_configurations_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   137275 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/standings_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    71111 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/transfers_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   100928 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/venues_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    73928 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/video_stream_inputs_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    76269 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/video_stream_subscriptions_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    72341 2023-07-10 10:50:22.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/video_streams_available_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    28316 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api_client.py
--rw-r--r--   0 k.kieda    (502) staff       (20)      779 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    14860 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/configuration.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5022 2023-07-10 10:50:15.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/exceptions.py
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-10 10:51:03.926386 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/
--rw-r--r--   0 k.kieda    (502) staff       (20)    35789 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/__init__.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6094 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/award_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5926 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/award_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    10475 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/awards_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2330 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/awards_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3495 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/awards_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3057 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/blank_model_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5041 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/career_person_season_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2530 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/career_person_season_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3762 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/career_person_season_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3531 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/career_person_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2481 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/career_person_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3689 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/career_person_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4448 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/change_log_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2354 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/change_log_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3532 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/change_log_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4405 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_entity_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2521 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_entity_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3749 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_entity_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4302 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_historical_name.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4401 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_person_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2521 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_person_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3749 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_person_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9341 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9112 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11710 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2316 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_model_league.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2376 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3567 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11966 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_season_status_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2436 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_season_status_model_league.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2496 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_season_status_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3713 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_season_status_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    23827 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conduct_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2337 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conduct_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2938 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conduct_penalty_result.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    18995 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conduct_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    18856 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conduct_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3507 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conduct_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5693 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conference_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5174 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conference_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7587 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conferences_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2368 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conferences_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3555 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conferences_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3114 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/contact_details.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6109 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/division_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5676 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/division_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     8546 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/divisions_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2352 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/divisions_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3531 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/divisions_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    18029 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entities_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2336 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entities_model_entity_group.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2343 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entities_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3519 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entities_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2496 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_additional_details.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5227 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_address.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5268 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_group_address.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4876 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_group_historical_name.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11288 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_group_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4222 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_group_post_body_additional_names.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3406 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_group_post_body_colors.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11119 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_group_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    13235 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_groups_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2377 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_groups_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3568 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_groups_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4836 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_historical_name.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    15522 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4158 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_post_body_additional_names.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3348 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_post_body_colors.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    15400 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     1929 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/environmental_details.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2849 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/error_list_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2825 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/error_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6046 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_competitor.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    12585 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entities_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2356 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entities_model_conference.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2336 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entities_model_division.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2318 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entities_model_entity.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2424 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entities_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9137 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entities_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3604 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entities_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2747 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_period_statistics_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4700 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2489 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5193 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2545 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3795 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2244 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_statistics_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3701 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2703 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_live_summary_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3641 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_live_summary_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5527 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_participant.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    10059 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_pbp_event_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2425 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_pbp_event_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3605 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_pbp_event_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4486 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_pbp_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2362 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_pbp_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2660 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_pbp_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3544 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_pbp_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7624 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2489 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6090 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2546 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3138 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3795 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4767 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3701 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9886 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_persons_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2416 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_persons_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2309 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_persons_model_person.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6942 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_persons_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3592 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_persons_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    22216 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3960 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_profiles_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2424 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_profiles_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2650 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_profiles_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2393 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_profiles_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3604 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_profiles_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3546 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_progression_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3225 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_progression_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5970 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_progressions_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2364 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_progressions_model_fixture.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2457 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_progressions_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2354 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_progressions_model_season.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3652 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_progressions_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    22088 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6724 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_roster_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2386 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_roster_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3884 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_roster_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3580 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_roster_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3201 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_videosteam_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    28618 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_by_entity_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3617 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_by_entity_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    28554 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2359 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_model_fixture_profile.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2344 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2292 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_model_round.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2305 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_model_series.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2274 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_model_venue.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3519 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4979 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/game_log_entity_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2387 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/game_log_entity_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3581 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/game_log_entity_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7681 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/game_log_person_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2387 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/game_log_person_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3581 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/game_log_person_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     1897 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/head_to_head_identification.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2049 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/head_to_head_identification_for_subsequent_checks.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2363 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/head_to_head_resolution.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2499 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/head_to_head_resolution_for_extra_depth_h2h_s.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9444 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/images_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2329 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/images_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     1757 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/images_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2461 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/images_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3495 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/images_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     1876 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/included_data.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3200 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_criteria_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2415 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_criteria_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2085 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_criteria_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     1837 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_criteria_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3592 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_criteria_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3810 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_qualifier_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3635 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_qualifier_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5867 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_qualifiers_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2444 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_qualifiers_model_leaders_criteria.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2430 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_qualifiers_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3616 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_qualifiers_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2728 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_summary_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3580 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_summary_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6652 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/league_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6530 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/league_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     8593 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leagues_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2336 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leagues_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3507 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leagues_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5994 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/organization_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5784 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/organization_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7119 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/organizations_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3579 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/organizations_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5672 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/person_additional_details.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5833 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/person_historical_name.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2556 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/person_list_default_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    13370 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/person_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5720 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/person_post_body_additional_names_value.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    13315 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/person_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    15343 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/persons_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2336 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/persons_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3507 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/persons_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6103 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/pool_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5679 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/pool_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5564 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/ranking_rows_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4618 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/ranking_rows_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4458 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/ranking_rows_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3556 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/ranking_rows_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2200 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/response_links.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3437 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/response_meta_data.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11638 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/role_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11517 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/role_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    15525 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/roles_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2320 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/roles_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3483 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/roles_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7057 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/round_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6627 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/round_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     8848 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entities_list_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2444 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entities_list_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3641 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entities_list_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9018 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entities_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5624 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entities_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3592 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entities_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6248 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_base_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2514 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_base_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3713 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_base_statistics_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3738 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_base_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4059 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_placings_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3665 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_placings_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5241 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2481 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3689 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6222 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2526 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2442 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_pool.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2452 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_stage.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3772 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6931 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_base_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2514 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_base_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3893 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_base_statistics_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3738 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_base_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4059 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_placings_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3665 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_placings_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5731 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2481 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6195 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_statistics_periods_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3783 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_statistics_periods_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3689 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5105 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_total_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2522 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_total_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3750 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_total_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6836 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_persons_list_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2436 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_persons_list_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3629 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_persons_list_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7006 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_persons_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4072 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_persons_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3580 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_persons_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     8501 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_pools_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2362 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_pools_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3556 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_pools_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    18148 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    18363 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    10457 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_roster_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2378 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_roster_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5981 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_roster_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3568 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_roster_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9996 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_rounds_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2370 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_rounds_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3568 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_rounds_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4466 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_series_competitor.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    16333 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_series_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2371 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_series_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3568 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_series_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5733 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_stage_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5248 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_stage_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7537 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_stages_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2377 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_stages_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3568 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_stages_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5288 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2542 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3796 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5276 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_venues_address.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11002 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_venues_list_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2428 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_venues_list_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2326 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_venues_list_model_site.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3617 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_venues_list_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3543 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasonentity_placings_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3354 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasonentity_placings_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3543 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasonperson_placings_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3354 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasonperson_placings_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3957 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasonroster_configuration.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    22249 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasons_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2326 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasons_model_competition.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2351 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasons_model_fixture_profile.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2336 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasons_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2452 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasons_model_standing_configuration.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3507 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasons_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    12210 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/series_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11915 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/series_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5211 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/site_address.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6538 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/site_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6354 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/site_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7786 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/sites_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2320 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/sites_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3483 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/sites_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3245 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/social_media.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2237 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/sorting.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    12332 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_adjustment_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    12243 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_adjustment_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    17425 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_adjustments_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2457 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_adjustments_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3652 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_adjustments_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4994 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_building.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    13200 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_configuration.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6222 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_configurations_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2482 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_configurations_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4849 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_configurations_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4563 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_configurations_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3688 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_configurations_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    12098 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    18313 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_post_body_calculated_value.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4442 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_post_body_points_value.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    12099 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    18136 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standings_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2352 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standings_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3531 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standings_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     1778 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/success_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3507 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/success_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2624 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/transfer_component.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7246 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/transfer_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7087 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/transfer_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9588 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/transfers_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2354 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/transfers_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3531 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/transfers_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5219 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venue_address.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5326 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venue_historical_name.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    10631 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venue_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    10463 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venue_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    12568 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venues_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2328 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venues_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2248 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venues_model_site.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3495 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venues_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9562 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_file_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2163 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_files_download_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3641 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_files_download_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11486 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_files_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2361 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_files_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3544 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_files_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11747 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_inputs_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2441 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_inputs_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3629 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_inputs_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5343 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_local_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2433 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_local_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3473 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_local_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3312 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_local_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3617 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_local_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9468 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_outputs_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2449 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_outputs_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3641 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_outputs_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11463 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_subscription_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11577 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_subscription_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    13664 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_subscriptions_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2447 2023-07-10 10:50:20.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_subscriptions_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3640 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_subscriptions_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    12617 2023-07-10 10:50:19.000000 atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/rest.py
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-10 10:51:03.927172 atriumsports_sdk-1.3.2/atriumsports/datacore_stream/
--rw-r--r--   0 k.kieda    (502) staff       (20)        0 2023-03-17 13:13:17.000000 atriumsports_sdk-1.3.2/atriumsports/datacore_stream/__init__.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6124 2023-04-24 10:52:46.000000 atriumsports_sdk-1.3.2/atriumsports/datacore_stream/datacore_stream.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     1942 2023-07-03 16:04:32.000000 atriumsports_sdk-1.3.2/atriumsports/endpoints.py
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-10 10:51:03.929208 atriumsports_sdk-1.3.2/atriumsports_sdk.egg-info/
--rw-r--r--   0 k.kieda    (502) staff       (20)     5380 2023-07-10 10:51:03.000000 atriumsports_sdk-1.3.2/atriumsports_sdk.egg-info/PKG-INFO
--rw-r--r--   0 k.kieda    (502) staff       (20)    27301 2023-07-10 10:51:03.000000 atriumsports_sdk-1.3.2/atriumsports_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 k.kieda    (502) staff       (20)        1 2023-07-10 10:51:03.000000 atriumsports_sdk-1.3.2/atriumsports_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 k.kieda    (502) staff       (20)      115 2023-07-10 10:51:03.000000 atriumsports_sdk-1.3.2/atriumsports_sdk.egg-info/requires.txt
--rw-r--r--   0 k.kieda    (502) staff       (20)       13 2023-07-10 10:51:03.000000 atriumsports_sdk-1.3.2/atriumsports_sdk.egg-info/top_level.txt
--rw-r--r--   0 k.kieda    (502) staff       (20)       80 2023-04-24 10:51:20.000000 atriumsports_sdk-1.3.2/pyproject.toml
--rw-r--r--   0 k.kieda    (502) staff       (20)       38 2023-07-10 10:51:03.930240 atriumsports_sdk-1.3.2/setup.cfg
--rw-r--r--   0 k.kieda    (502) staff       (20)      954 2023-07-10 10:49:42.000000 atriumsports_sdk-1.3.2/setup.py
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-26 16:44:04.114103 atriumsports_sdk-1.4.0/
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1074 2023-03-17 13:13:15.000000 atriumsports_sdk-1.4.0/LICENSE
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5380 2023-07-26 16:44:04.113822 atriumsports_sdk-1.4.0/PKG-INFO
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4963 2023-06-16 15:49:48.000000 atriumsports_sdk-1.4.0/README.md
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-26 16:44:02.227688 atriumsports_sdk-1.4.0/atriumsports/
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1096 2023-03-17 13:13:15.000000 atriumsports_sdk-1.4.0/atriumsports/__init__.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4294 2023-04-24 10:52:41.000000 atriumsports_sdk-1.4.0/atriumsports/atrium_response.py
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-26 16:44:02.230824 atriumsports_sdk-1.4.0/atriumsports/datacore/
+-rw-r--r--   0 k.kieda    (502) staff       (20)        0 2022-11-21 11:07:25.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/__init__.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6660 2023-04-24 10:52:41.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/datacore.py
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-26 16:44:02.258344 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/
+-rw-r--r--   0 k.kieda    (502) staff       (20)    54869 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/__init__.py
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-26 16:44:02.589750 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4630 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/__init__.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   121018 2023-07-26 16:40:21.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/awards_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    59847 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/career_statistics_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    18925 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/change_log_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    97107 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/competition_statistics_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   127164 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/competitions_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    78180 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/conduct_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   137833 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/conferences_divisions_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    66311 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/download_video_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    91278 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/entities_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    21039 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/entity_fixture_history_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   127554 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/entity_fixture_statistics_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    70185 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/entity_groups_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    59444 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/fixture_entities_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11205 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/fixture_live_summary_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    59323 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/fixture_persons_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    77945 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/fixture_playbyplay_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    72387 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/fixture_profiles_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    76686 2023-07-26 16:40:21.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/fixture_progressions_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    89352 2023-07-26 16:40:21.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/fixture_roster_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   442257 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/fixtures_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   252466 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/images_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    70633 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/leader_criteria_sets_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    73398 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/leader_qualifiers_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    70024 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/leagues_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    73817 2023-07-26 16:40:21.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/local_video_endpoints_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    70215 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/merge_records_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    66029 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/organizations_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    36028 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/partner_apis_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    23558 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/person_fixture_history_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   134432 2023-07-26 16:40:21.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/person_fixture_statistics_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    91522 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/persons_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   107461 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/rankings_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   150045 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/roles_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    77289 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/season_entities_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    49629 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/season_entity_base_statistics_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    71603 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/season_entity_placings_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    44646 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/season_leaders_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    50867 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/season_person_base_statistics_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    71598 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/season_person_placings_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    77803 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/season_persons_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    97800 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/season_roster_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    90287 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/season_series_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   177700 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/season_statistics_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   120275 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/seasons_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    68423 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/sites_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   229910 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/stages_pools_rounds_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    76768 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/standing_adjustments_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    71710 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/standing_configurations_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   137275 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/standings_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    71111 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/transfers_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   102802 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/venues_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    73928 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/video_stream_inputs_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    76269 2023-07-26 16:40:21.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/video_stream_subscriptions_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    72341 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/video_streams_available_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    28317 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api_client.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)      779 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    14860 2023-07-26 16:40:18.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/configuration.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5022 2023-07-26 16:40:14.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/exceptions.py
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-26 16:44:04.106412 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/
+-rw-r--r--   0 k.kieda    (502) staff       (20)    36007 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/__init__.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6094 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/award_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5926 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/award_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    10475 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/awards_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2330 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/awards_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3495 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/awards_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3057 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/blank_model_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5041 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/career_person_season_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2530 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/career_person_season_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3762 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/career_person_season_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3531 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/career_person_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2481 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/career_person_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3689 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/career_person_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4448 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/change_log_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2354 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/change_log_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3532 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/change_log_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4405 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competition_entity_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2521 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competition_entity_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3749 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competition_entity_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4302 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competition_historical_name.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4401 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competition_person_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2521 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competition_person_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3749 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competition_person_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9596 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competition_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9367 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competition_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11965 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competitions_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2316 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competitions_model_league.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2376 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competitions_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3567 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competitions_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12221 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competitions_season_status_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2436 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competitions_season_status_model_league.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2496 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competitions_season_status_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3713 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competitions_season_status_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    24236 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/conduct_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2337 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/conduct_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2938 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/conduct_penalty_result.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    19404 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/conduct_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    19265 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/conduct_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3507 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/conduct_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5693 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/conference_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5174 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/conference_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7587 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/conferences_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2368 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/conferences_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3555 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/conferences_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3114 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/contact_details.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6109 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/division_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5676 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/division_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     8546 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/divisions_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2352 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/divisions_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3531 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/divisions_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    18768 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entities_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2336 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entities_model_entity_group.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2343 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entities_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3519 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entities_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2496 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_additional_details.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5227 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_address.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5268 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_group_address.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4876 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_group_historical_name.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11288 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_group_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4222 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_group_post_body_additional_names.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3406 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_group_post_body_colors.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11119 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_group_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    13235 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_groups_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2377 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_groups_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3568 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_groups_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4836 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_historical_name.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    16261 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4158 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_post_body_additional_names.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3348 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_post_body_colors.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    16139 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1929 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/environmental_details.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2849 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/error_list_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2825 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/error_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6046 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_competitor.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12585 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_entities_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2356 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_entities_model_conference.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2336 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_entities_model_division.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2318 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_entities_model_entity.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2424 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_entities_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9137 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_entities_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3604 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_entities_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2747 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_entity_period_statistics_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4700 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2489 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5193 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2545 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3795 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2244 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3701 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2703 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_live_summary_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3641 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_live_summary_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5527 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_participant.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    10059 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_pbp_event_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2425 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_pbp_event_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3605 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_pbp_event_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4486 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_pbp_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2362 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_pbp_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2660 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_pbp_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3544 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_pbp_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7624 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_person_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2489 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_person_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6090 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2546 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3138 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3795 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4767 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_person_statistics_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3701 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_person_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9886 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_persons_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2416 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_persons_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2309 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_persons_model_person.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6942 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_persons_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3592 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_persons_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    22546 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3960 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_profiles_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2424 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_profiles_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2650 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_profiles_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2393 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_profiles_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3604 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_profiles_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3546 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_progression_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3225 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_progression_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5970 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_progressions_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2364 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_progressions_model_fixture.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2457 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_progressions_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2354 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_progressions_model_season.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3652 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_progressions_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    22418 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6724 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_roster_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2386 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_roster_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3884 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_roster_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3580 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_roster_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3201 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_videosteam_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    28988 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixtures_by_competition_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3677 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixtures_by_competition_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    28948 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixtures_by_entity_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3617 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixtures_by_entity_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    28884 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixtures_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2359 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixtures_model_fixture_profile.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2344 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixtures_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2292 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixtures_model_round.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2305 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixtures_model_series.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2274 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixtures_model_venue.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3519 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixtures_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4979 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/game_log_entity_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2387 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/game_log_entity_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3581 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/game_log_entity_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7681 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/game_log_person_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2387 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/game_log_person_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3581 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/game_log_person_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1897 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/head_to_head_identification.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2049 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/head_to_head_identification_for_subsequent_checks.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2363 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/head_to_head_resolution.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2499 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/head_to_head_resolution_for_extra_depth_h2h_s.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9707 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/images_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2329 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/images_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1757 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/images_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2461 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/images_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3495 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/images_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1876 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/included_data.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3200 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leader_criteria_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2415 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leader_criteria_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2085 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leader_criteria_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1837 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leader_criteria_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3592 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leader_criteria_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3810 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leader_qualifier_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3635 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leader_qualifier_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5867 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leader_qualifiers_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2444 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leader_qualifiers_model_leaders_criteria.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2430 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leader_qualifiers_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3616 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leader_qualifiers_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2728 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leader_summary_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3580 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leader_summary_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6652 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/league_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6530 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/league_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     8593 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leagues_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2336 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leagues_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3507 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leagues_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5994 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/organization_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5784 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/organization_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7119 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/organizations_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3579 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/organizations_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5672 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/person_additional_details.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5833 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/person_historical_name.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2556 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/person_list_default_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    13370 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/person_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5720 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/person_post_body_additional_names_value.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    13315 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/person_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    15343 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/persons_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2336 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/persons_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3507 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/persons_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6103 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/pool_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5679 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/pool_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5564 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/ranking_rows_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4618 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/ranking_rows_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4458 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/ranking_rows_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3556 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/ranking_rows_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2200 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/response_links.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3437 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/response_meta_data.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11638 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/role_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11517 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/role_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    15525 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/roles_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2320 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/roles_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3483 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/roles_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7057 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/round_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6627 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/round_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     8848 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_entities_list_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2444 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_entities_list_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3641 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_entities_list_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9018 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_entities_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5624 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_entities_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3592 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_entities_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6248 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2514 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3713 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3738 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4059 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_entity_placings_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3665 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_entity_placings_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5241 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_entity_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2481 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_entity_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3689 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_entity_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6222 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2526 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2442 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_pool.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2452 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_stage.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3772 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6931 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_person_base_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2514 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_person_base_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3893 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_person_base_statistics_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3738 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_person_base_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4059 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_person_placings_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3665 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_person_placings_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5731 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_person_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2481 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_person_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6195 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_person_statistics_periods_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3783 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_person_statistics_periods_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3689 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_person_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5105 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_person_total_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2522 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_person_total_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3750 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_person_total_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6836 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_persons_list_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2436 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_persons_list_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3629 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_persons_list_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7006 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_persons_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4072 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_persons_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3580 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_persons_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     8501 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_pools_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2362 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_pools_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3556 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_pools_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    18148 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    18363 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    10457 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_roster_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2378 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_roster_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5981 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_roster_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3568 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_roster_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9996 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_rounds_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2370 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_rounds_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3568 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_rounds_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4466 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_series_competitor.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    16333 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_series_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2371 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_series_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3568 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_series_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5733 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_stage_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5248 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_stage_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7537 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_stages_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2377 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_stages_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3568 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_stages_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5288 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2542 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3796 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5276 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_venues_address.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11002 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_venues_list_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2428 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_venues_list_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2326 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_venues_list_model_site.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3617 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_venues_list_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3543 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/seasonentity_placings_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3354 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/seasonentity_placings_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3543 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/seasonperson_placings_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3354 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/seasonperson_placings_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3957 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/seasonroster_configuration.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    22249 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/seasons_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2326 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/seasons_model_competition.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2351 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/seasons_model_fixture_profile.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2336 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/seasons_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2452 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/seasons_model_standing_configuration.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3507 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/seasons_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12210 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/series_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11915 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/series_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5211 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/site_address.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6538 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/site_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6354 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/site_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7786 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/sites_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2320 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/sites_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3483 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/sites_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3245 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/social_media.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2237 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/sorting.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12269 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_adjustment_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12243 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_adjustment_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    17425 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_adjustments_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2457 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_adjustments_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3652 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_adjustments_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4994 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_building.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    13200 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_configuration.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6222 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_configurations_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2482 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_configurations_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4849 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_configurations_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4563 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_configurations_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3688 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_configurations_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12098 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    18313 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_post_body_calculated_value.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4442 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_post_body_points_value.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12099 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    18136 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standings_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2352 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standings_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3531 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standings_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1778 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/success_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3507 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/success_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2624 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/transfer_component.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7487 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/transfer_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7328 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/transfer_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9829 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/transfers_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2354 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/transfers_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3531 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/transfers_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5219 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/venue_address.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5326 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/venue_historical_name.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    10631 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/venue_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    10463 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/venue_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12568 2023-07-26 16:40:20.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/venues_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2328 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/venues_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2248 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/venues_model_site.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3495 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/venues_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    10297 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_file_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2163 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_files_download_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3641 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_files_download_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12221 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_files_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2361 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_files_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3544 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_files_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11747 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_stream_inputs_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2441 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_stream_inputs_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3629 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_stream_inputs_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5343 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_stream_local_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2433 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_stream_local_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3473 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_stream_local_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3312 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_stream_local_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3617 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_stream_local_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9468 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_stream_outputs_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2449 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_stream_outputs_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3641 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_stream_outputs_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11463 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_subscription_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11577 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_subscription_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    13664 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_subscriptions_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2447 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_subscriptions_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3640 2023-07-26 16:40:19.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_subscriptions_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12618 2023-07-26 16:40:18.000000 atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/rest.py
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-26 16:44:04.110832 atriumsports_sdk-1.4.0/atriumsports/datacore_stream/
+-rw-r--r--   0 k.kieda    (502) staff       (20)        0 2023-03-17 13:13:17.000000 atriumsports_sdk-1.4.0/atriumsports/datacore_stream/__init__.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6124 2023-04-24 10:52:46.000000 atriumsports_sdk-1.4.0/atriumsports/datacore_stream/datacore_stream.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1942 2023-07-03 16:04:32.000000 atriumsports_sdk-1.4.0/atriumsports/endpoints.py
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2023-07-26 16:44:04.113394 atriumsports_sdk-1.4.0/atriumsports_sdk.egg-info/
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5380 2023-07-26 16:44:02.000000 atriumsports_sdk-1.4.0/atriumsports_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 k.kieda    (502) staff       (20)    27444 2023-07-26 16:44:02.000000 atriumsports_sdk-1.4.0/atriumsports_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 k.kieda    (502) staff       (20)        1 2023-07-26 16:44:02.000000 atriumsports_sdk-1.4.0/atriumsports_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 k.kieda    (502) staff       (20)      115 2023-07-26 16:44:02.000000 atriumsports_sdk-1.4.0/atriumsports_sdk.egg-info/requires.txt
+-rw-r--r--   0 k.kieda    (502) staff       (20)       13 2023-07-26 16:44:02.000000 atriumsports_sdk-1.4.0/atriumsports_sdk.egg-info/top_level.txt
+-rw-r--r--   0 k.kieda    (502) staff       (20)       80 2023-04-24 10:51:20.000000 atriumsports_sdk-1.4.0/pyproject.toml
+-rw-r--r--   0 k.kieda    (502) staff       (20)       38 2023-07-26 16:44:04.114161 atriumsports_sdk-1.4.0/setup.cfg
+-rw-r--r--   0 k.kieda    (502) staff       (20)      954 2023-07-26 13:26:00.000000 atriumsports_sdk-1.4.0/setup.py
```

### Comparing `atriumsports_sdk-1.3.2/LICENSE` & `atriumsports_sdk-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/PKG-INFO` & `atriumsports_sdk-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atriumsports_sdk
-Version: 1.3.2
+Version: 1.4.0
 Summary: Python module for integration to Atrium Sports APIs
 Author: Atrium Sports
 Author-email: python_dev@atriumsports.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `atriumsports_sdk-1.3.2/README.md` & `atriumsports_sdk-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/__init__.py` & `atriumsports_sdk-1.4.0/atriumsports/__init__.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/atrium_response.py` & `atriumsports_sdk-1.4.0/atriumsports/atrium_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/datacore.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/datacore.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/__init__.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,15 +237,15 @@
 
 This **access token** must then be sent in the `Authorization` header for each subsequent API call.  Access tokens have a finite life and will expire. When the token expires you will need to create a new token to make more API calls.  Creation of tokens is rate-limited, so you should use the existing token as long as possible.
 
 <!-- ReDoc-Inject: <security-definitions> -->
   # noqa: E501
 """
 
-__version__ = "1.3.2"
+__version__ = "1.4.0"
 
 # import apis into sdk package
 from atriumsports.datacore.openapi.api.awards_api import AwardsApi
 from atriumsports.datacore.openapi.api.career_statistics_api import CareerStatisticsApi
 from atriumsports.datacore.openapi.api.change_log_api import ChangeLogApi
 from atriumsports.datacore.openapi.api.competition_statistics_api import CompetitionStatisticsApi
 from atriumsports.datacore.openapi.api.competitions_api import CompetitionsApi
@@ -481,14 +481,16 @@
 from atriumsports.datacore.openapi.models.fixture_progressions_response import FixtureProgressionsResponse
 from atriumsports.datacore.openapi.models.fixture_put_body import FixturePutBody
 from atriumsports.datacore.openapi.models.fixture_roster_model import FixtureRosterModel
 from atriumsports.datacore.openapi.models.fixture_roster_model_organization import FixtureRosterModelOrganization
 from atriumsports.datacore.openapi.models.fixture_roster_post_body import FixtureRosterPostBody
 from atriumsports.datacore.openapi.models.fixture_roster_response import FixtureRosterResponse
 from atriumsports.datacore.openapi.models.fixture_videosteam_post_body import FixtureVideosteamPostBody
+from atriumsports.datacore.openapi.models.fixtures_by_competition_model import FixturesByCompetitionModel
+from atriumsports.datacore.openapi.models.fixtures_by_competition_response import FixturesByCompetitionResponse
 from atriumsports.datacore.openapi.models.fixtures_by_entity_model import FixturesByEntityModel
 from atriumsports.datacore.openapi.models.fixtures_by_entity_response import FixturesByEntityResponse
 from atriumsports.datacore.openapi.models.fixtures_model import FixturesModel
 from atriumsports.datacore.openapi.models.fixtures_model_fixture_profile import FixturesModelFixtureProfile
 from atriumsports.datacore.openapi.models.fixtures_model_organization import FixturesModelOrganization
 from atriumsports.datacore.openapi.models.fixtures_model_round import FixturesModelRound
 from atriumsports.datacore.openapi.models.fixtures_model_series import FixturesModelSeries
```

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/__init__.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/__init__.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/awards_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/awards_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/career_statistics_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/career_statistics_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/change_log_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/change_log_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/competition_statistics_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/competition_statistics_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/competitions_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/competitions_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/conduct_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/conduct_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -872,15 +872,15 @@
         ] = None,
         competition_id: Annotated[
             Optional[StrictStr], Field(description="The unique identifier of the competition")
         ] = None,
         conduct_status: Annotated[
             Optional[constr(strict=True, max_length=200)],
             Field(
-                description="Conduct status. Multiple allowed (comma-delimited). >- `ACTIVE` Active >- `CLOSED` Closed >- `COMPLETE` Complete >- `INACTIVE` Inactive >- `PENDING` Pending "
+                description="Conduct status. Multiple allowed (comma-delimited). >- None None >- `ACTIVE` Active >- `CLOSED` Closed >- `COMPLETE` Complete >- `INACTIVE` Inactive >- `PENDING` Pending "
             ),
         ] = None,
         conduct_type: Annotated[
             Optional[StrictStr],
             Field(
                 description="Conduct type. Multiple allowed (comma-delimited). >- `CITATION` Citation >- `CONCUSSION` Concussion >- `CORRUPTION` Corruption >- `DOPING` Doping >- `MATCH_FIXING` Match Fixing >- `SWEARING` Swearing >- `TOUCHLINE_SUSPENSION` Touchline Suspension >- `UNSPORTSMANLIKE_CONDUCT` Unsportsmanlike Conduct >- `VIOLET_CONDUCT` Violent Conduct "
             ),
@@ -949,15 +949,15 @@
         :type organization_id: str
         :param sport: Sport name (required)
         :type sport: str
         :param added: Record was added after this date/time. In UTC.
         :type added: datetime
         :param competition_id: The unique identifier of the competition
         :type competition_id: str
-        :param conduct_status: Conduct status. Multiple allowed (comma-delimited). >- `ACTIVE` Active >- `CLOSED` Closed >- `COMPLETE` Complete >- `INACTIVE` Inactive >- `PENDING` Pending
+        :param conduct_status: Conduct status. Multiple allowed (comma-delimited). >- None None >- `ACTIVE` Active >- `CLOSED` Closed >- `COMPLETE` Complete >- `INACTIVE` Inactive >- `PENDING` Pending
         :type conduct_status: str
         :param conduct_type: Conduct type. Multiple allowed (comma-delimited). >- `CITATION` Citation >- `CONCUSSION` Concussion >- `CORRUPTION` Corruption >- `DOPING` Doping >- `MATCH_FIXING` Match Fixing >- `SWEARING` Swearing >- `TOUCHLINE_SUSPENSION` Touchline Suspension >- `UNSPORTSMANLIKE_CONDUCT` Unsportsmanlike Conduct >- `VIOLET_CONDUCT` Violent Conduct
         :type conduct_type: str
         :param date_offence_local_end: Where dateOffenceLocal is before this value
         :type date_offence_local_end: datetime
         :param date_offence_local_start: Where dateOffenceLocal is after this value
         :type date_offence_local_start: datetime
@@ -1042,15 +1042,15 @@
         ] = None,
         competition_id: Annotated[
             Optional[StrictStr], Field(description="The unique identifier of the competition")
         ] = None,
         conduct_status: Annotated[
             Optional[constr(strict=True, max_length=200)],
             Field(
-                description="Conduct status. Multiple allowed (comma-delimited). >- `ACTIVE` Active >- `CLOSED` Closed >- `COMPLETE` Complete >- `INACTIVE` Inactive >- `PENDING` Pending "
+                description="Conduct status. Multiple allowed (comma-delimited). >- None None >- `ACTIVE` Active >- `CLOSED` Closed >- `COMPLETE` Complete >- `INACTIVE` Inactive >- `PENDING` Pending "
             ),
         ] = None,
         conduct_type: Annotated[
             Optional[StrictStr],
             Field(
                 description="Conduct type. Multiple allowed (comma-delimited). >- `CITATION` Citation >- `CONCUSSION` Concussion >- `CORRUPTION` Corruption >- `DOPING` Doping >- `MATCH_FIXING` Match Fixing >- `SWEARING` Swearing >- `TOUCHLINE_SUSPENSION` Touchline Suspension >- `UNSPORTSMANLIKE_CONDUCT` Unsportsmanlike Conduct >- `VIOLET_CONDUCT` Violent Conduct "
             ),
@@ -1119,15 +1119,15 @@
         :type organization_id: str
         :param sport: Sport name (required)
         :type sport: str
         :param added: Record was added after this date/time. In UTC.
         :type added: datetime
         :param competition_id: The unique identifier of the competition
         :type competition_id: str
-        :param conduct_status: Conduct status. Multiple allowed (comma-delimited). >- `ACTIVE` Active >- `CLOSED` Closed >- `COMPLETE` Complete >- `INACTIVE` Inactive >- `PENDING` Pending
+        :param conduct_status: Conduct status. Multiple allowed (comma-delimited). >- None None >- `ACTIVE` Active >- `CLOSED` Closed >- `COMPLETE` Complete >- `INACTIVE` Inactive >- `PENDING` Pending
         :type conduct_status: str
         :param conduct_type: Conduct type. Multiple allowed (comma-delimited). >- `CITATION` Citation >- `CONCUSSION` Concussion >- `CORRUPTION` Corruption >- `DOPING` Doping >- `MATCH_FIXING` Match Fixing >- `SWEARING` Swearing >- `TOUCHLINE_SUSPENSION` Touchline Suspension >- `UNSPORTSMANLIKE_CONDUCT` Unsportsmanlike Conduct >- `VIOLET_CONDUCT` Violent Conduct
         :type conduct_type: str
         :param date_offence_local_end: Where dateOffenceLocal is before this value
         :type date_offence_local_end: datetime
         :param date_offence_local_start: Where dateOffenceLocal is after this value
         :type date_offence_local_start: datetime
```

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/conferences_divisions_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/conferences_divisions_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/download_video_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/download_video_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/entities_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/entities_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/entity_fixture_history_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/entity_fixture_history_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/entity_fixture_statistics_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/entity_fixture_statistics_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/entity_groups_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/entity_groups_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixture_entities_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/fixture_entities_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixture_live_summary_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/fixture_live_summary_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixture_persons_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/fixture_persons_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixture_playbyplay_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/fixture_playbyplay_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixture_profiles_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/fixture_profiles_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixture_progressions_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/fixture_progressions_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixture_roster_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/fixture_roster_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/fixtures_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/fixtures_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 from atriumsports.datacore.openapi.api_client import ApiClient
 from atriumsports.datacore.openapi.api_response import ApiResponse
 from atriumsports.datacore.openapi.exceptions import ApiTypeError, ApiValueError  # noqa: F401
 from atriumsports.datacore.openapi.models.fixture_post_body import FixturePostBody
 from atriumsports.datacore.openapi.models.fixture_put_body import FixturePutBody
 from atriumsports.datacore.openapi.models.fixture_videosteam_post_body import FixtureVideosteamPostBody
+from atriumsports.datacore.openapi.models.fixtures_by_competition_response import FixturesByCompetitionResponse
 from atriumsports.datacore.openapi.models.fixtures_by_entity_response import FixturesByEntityResponse
 from atriumsports.datacore.openapi.models.fixtures_response import FixturesResponse
 from atriumsports.datacore.openapi.models.season_fixture_stages_pools_list_response import (
     SeasonFixtureStagesPoolsListResponse,
 )
 from atriumsports.datacore.openapi.models.success_response import SuccessResponse
 
@@ -47,14 +48,661 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
+    def fixture_by_competition_list(
+        self,
+        competition_id: Annotated[StrictStr, Field(..., description="The unique identifier of the competition")],
+        organization_id: Annotated[
+            constr(strict=True, max_length=5, min_length=5),
+            Field(..., description="The unique identifier of the organization"),
+        ],
+        sport: Annotated[StrictStr, Field(..., description="Sport name")],
+        added: Annotated[
+            Optional[datetime], Field(description="Record was added after this date/time. In UTC.")
+        ] = None,
+        competitor_type: Annotated[
+            Optional[StrictStr],
+            Field(description="The type of competitors in this fixture >- `ENTITY` Entity >- `PERSON` Person "),
+        ] = None,
+        external: Annotated[
+            Optional[StrictStr],
+            Field(
+                description="A comma separated list of fields that will instead be interpreted as an externalId. See [External Ids](#section/Introduction/External-Ids) for more information."
+            ),
+        ] = None,
+        fields: Annotated[
+            Optional[StrictStr],
+            Field(
+                description="A comma separated list of fields to display.  The response will only display these fields. See [Partial Response](#section/Partial-Response) section for more information."
+            ),
+        ] = None,
+        fixture_id: Annotated[Optional[StrictStr], Field(description="The unique identifier of the fixture")] = None,
+        fixture_type: Annotated[
+            Optional[constr(strict=True, max_length=50)],
+            Field(
+                description="Type of Fixture >- `ALL_STAR` All Star >- `DEMONSTRATION` Demonstration >- `FINAL` Final >- `FRIENDLY` Friendly >- `PLAYOFF` Playoff >- `PRESEASON` Pre Season >- `REGULAR` Regular "
+            ),
+        ] = None,
+        from_time_local: Annotated[
+            Optional[datetime], Field(description="Where fixture start time (in local time) >= this value")
+        ] = None,
+        from_time_utc: Annotated[
+            Optional[datetime], Field(description="Where fixture start time (in UTC) >= this value")
+        ] = None,
+        hide_null: Annotated[
+            Optional[StrictBool], Field(description="Don't display data fields with null values or empty structures")
+        ] = None,
+        include: Annotated[
+            Optional[StrictStr],
+            Field(
+                description="A comma separated list of resource types to include. See [Resource Inclusion](#section/Introduction/Resource-Inclusion) for more information."
+            ),
+        ] = None,
+        limit: Annotated[
+            Optional[conint(strict=True, le=1000, ge=1)],
+            Field(
+                description="The maximum number of records to return. See [Pagination](#section/Introduction/Pagination) for more information."
+            ),
+        ] = None,
+        live_data_available: Annotated[Optional[StrictBool], Field(description="Is live data available?")] = None,
+        live_video_available: Annotated[Optional[StrictBool], Field(description="Is live video available ?")] = None,
+        locked: Annotated[
+            Optional[StrictBool], Field(description="Is the fixture locked (to prevent editing)?")
+        ] = None,
+        offset: Annotated[
+            Optional[StrictInt],
+            Field(
+                description="The offset of the records. See [Pagination](#section/Introduction/Pagination) for more information."
+            ),
+        ] = None,
+        pool_code: Annotated[
+            Optional[constr(strict=True, max_length=30)], Field(description="The pool identifier within a season")
+        ] = None,
+        round_code: Annotated[
+            Optional[constr(strict=True, max_length=30)], Field(description="The round identifier within a season")
+        ] = None,
+        round_number: Annotated[Optional[constr(strict=True, max_length=30)], Field(description="Round number")] = None,
+        season_id: Annotated[Optional[StrictStr], Field(description="The unique identifier of the season")] = None,
+        sort_by: Annotated[
+            Optional[StrictStr],
+            Field(
+                description="Comma-delimited list of one or more fields to sort by, each field can have '-' as prefix to sort in descending order, and '+' (or no prefix) to sort in ascending order."
+            ),
+        ] = None,
+        stage_code: Annotated[
+            Optional[constr(strict=True, max_length=30)], Field(description="The stage identifier within a season")
+        ] = None,
+        status: Annotated[
+            Optional[constr(strict=True, max_length=200)],
+            Field(
+                description="Fixture status. Can specify multiple, delimited by comma. >- `ABANDONED` Abandoned >- `BYE` Bye >- `CANCELLED` Cancelled >- `CONFIRMED` Confirmed >- `FINISHED` Finished >- `IF_NEEDED` If Needed >- `IN_PROGRESS` In Progress >- `PENDING` Pending >- `POSTPONED` Postponed >- `SCHEDULED` Scheduled "
+            ),
+        ] = None,
+        times_unconfirmed: Annotated[
+            Optional[StrictBool], Field(description="Is the fixture time yet to be confirmed ?")
+        ] = None,
+        to_time_local: Annotated[
+            Optional[datetime], Field(description="Where fixture start time (in local time) <= this value")
+        ] = None,
+        to_time_utc: Annotated[
+            Optional[datetime], Field(description="Where fixture start time (in UTC) <= this value")
+        ] = None,
+        updated: Annotated[
+            Optional[datetime], Field(description="Record was modified after this date/time. In UTC.")
+        ] = None,
+        venue_id: Annotated[Optional[StrictStr], Field(description="The unique identifier of the venue")] = None,
+        **kwargs
+    ) -> FixturesByCompetitionResponse:  # noqa: E501
+        """Get a list of fixtures for a Competition  # noqa: E501
+
+        Return a list of fixtures, for a specific Competition  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.fixture_by_competition_list(competition_id, organization_id, sport, added, competitor_type, external, fields, fixture_id, fixture_type, from_time_local, from_time_utc, hide_null, include, limit, live_data_available, live_video_available, locked, offset, pool_code, round_code, round_number, season_id, sort_by, stage_code, status, times_unconfirmed, to_time_local, to_time_utc, updated, venue_id, async_req=True)
+        >>> result = thread.get()
+
+        :param competition_id: The unique identifier of the competition (required)
+        :type competition_id: str
+        :param organization_id: The unique identifier of the organization (required)
+        :type organization_id: str
+        :param sport: Sport name (required)
+        :type sport: str
+        :param added: Record was added after this date/time. In UTC.
+        :type added: datetime
+        :param competitor_type: The type of competitors in this fixture >- `ENTITY` Entity >- `PERSON` Person
+        :type competitor_type: str
+        :param external: A comma separated list of fields that will instead be interpreted as an externalId. See [External Ids](#section/Introduction/External-Ids) for more information.
+        :type external: str
+        :param fields: A comma separated list of fields to display.  The response will only display these fields. See [Partial Response](#section/Partial-Response) section for more information.
+        :type fields: str
+        :param fixture_id: The unique identifier of the fixture
+        :type fixture_id: str
+        :param fixture_type: Type of Fixture >- `ALL_STAR` All Star >- `DEMONSTRATION` Demonstration >- `FINAL` Final >- `FRIENDLY` Friendly >- `PLAYOFF` Playoff >- `PRESEASON` Pre Season >- `REGULAR` Regular
+        :type fixture_type: str
+        :param from_time_local: Where fixture start time (in local time) >= this value
+        :type from_time_local: datetime
+        :param from_time_utc: Where fixture start time (in UTC) >= this value
+        :type from_time_utc: datetime
+        :param hide_null: Don't display data fields with null values or empty structures
+        :type hide_null: bool
+        :param include: A comma separated list of resource types to include. See [Resource Inclusion](#section/Introduction/Resource-Inclusion) for more information.
+        :type include: str
+        :param limit: The maximum number of records to return. See [Pagination](#section/Introduction/Pagination) for more information.
+        :type limit: int
+        :param live_data_available: Is live data available?
+        :type live_data_available: bool
+        :param live_video_available: Is live video available ?
+        :type live_video_available: bool
+        :param locked: Is the fixture locked (to prevent editing)?
+        :type locked: bool
+        :param offset: The offset of the records. See [Pagination](#section/Introduction/Pagination) for more information.
+        :type offset: int
+        :param pool_code: The pool identifier within a season
+        :type pool_code: str
+        :param round_code: The round identifier within a season
+        :type round_code: str
+        :param round_number: Round number
+        :type round_number: str
+        :param season_id: The unique identifier of the season
+        :type season_id: str
+        :param sort_by: Comma-delimited list of one or more fields to sort by, each field can have '-' as prefix to sort in descending order, and '+' (or no prefix) to sort in ascending order.
+        :type sort_by: str
+        :param stage_code: The stage identifier within a season
+        :type stage_code: str
+        :param status: Fixture status. Can specify multiple, delimited by comma. >- `ABANDONED` Abandoned >- `BYE` Bye >- `CANCELLED` Cancelled >- `CONFIRMED` Confirmed >- `FINISHED` Finished >- `IF_NEEDED` If Needed >- `IN_PROGRESS` In Progress >- `PENDING` Pending >- `POSTPONED` Postponed >- `SCHEDULED` Scheduled
+        :type status: str
+        :param times_unconfirmed: Is the fixture time yet to be confirmed ?
+        :type times_unconfirmed: bool
+        :param to_time_local: Where fixture start time (in local time) <= this value
+        :type to_time_local: datetime
+        :param to_time_utc: Where fixture start time (in UTC) <= this value
+        :type to_time_utc: datetime
+        :param updated: Record was modified after this date/time. In UTC.
+        :type updated: datetime
+        :param venue_id: The unique identifier of the venue
+        :type venue_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: FixturesByCompetitionResponse
+        """
+        kwargs["_return_http_data_only"] = True
+        if "_preload_content" in kwargs:
+            raise ValueError(
+                "Error! Please call the fixture_by_competition_list_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"
+            )
+        try:
+            return self.fixture_by_competition_list_with_http_info(
+                competition_id,
+                organization_id,
+                sport,
+                added,
+                competitor_type,
+                external,
+                fields,
+                fixture_id,
+                fixture_type,
+                from_time_local,
+                from_time_utc,
+                hide_null,
+                include,
+                limit,
+                live_data_available,
+                live_video_available,
+                locked,
+                offset,
+                pool_code,
+                round_code,
+                round_number,
+                season_id,
+                sort_by,
+                stage_code,
+                status,
+                times_unconfirmed,
+                to_time_local,
+                to_time_utc,
+                updated,
+                venue_id,
+                **kwargs
+            )  # noqa: E501
+        except Exception as e:
+            logger.error("Exception when calling FixturesApi->fixture_by_competition_list: %s\n" % e)
+            raise
+
+    @validate_arguments
+    def fixture_by_competition_list_with_http_info(
+        self,
+        competition_id: Annotated[StrictStr, Field(..., description="The unique identifier of the competition")],
+        organization_id: Annotated[
+            constr(strict=True, max_length=5, min_length=5),
+            Field(..., description="The unique identifier of the organization"),
+        ],
+        sport: Annotated[StrictStr, Field(..., description="Sport name")],
+        added: Annotated[
+            Optional[datetime], Field(description="Record was added after this date/time. In UTC.")
+        ] = None,
+        competitor_type: Annotated[
+            Optional[StrictStr],
+            Field(description="The type of competitors in this fixture >- `ENTITY` Entity >- `PERSON` Person "),
+        ] = None,
+        external: Annotated[
+            Optional[StrictStr],
+            Field(
+                description="A comma separated list of fields that will instead be interpreted as an externalId. See [External Ids](#section/Introduction/External-Ids) for more information."
+            ),
+        ] = None,
+        fields: Annotated[
+            Optional[StrictStr],
+            Field(
+                description="A comma separated list of fields to display.  The response will only display these fields. See [Partial Response](#section/Partial-Response) section for more information."
+            ),
+        ] = None,
+        fixture_id: Annotated[Optional[StrictStr], Field(description="The unique identifier of the fixture")] = None,
+        fixture_type: Annotated[
+            Optional[constr(strict=True, max_length=50)],
+            Field(
+                description="Type of Fixture >- `ALL_STAR` All Star >- `DEMONSTRATION` Demonstration >- `FINAL` Final >- `FRIENDLY` Friendly >- `PLAYOFF` Playoff >- `PRESEASON` Pre Season >- `REGULAR` Regular "
+            ),
+        ] = None,
+        from_time_local: Annotated[
+            Optional[datetime], Field(description="Where fixture start time (in local time) >= this value")
+        ] = None,
+        from_time_utc: Annotated[
+            Optional[datetime], Field(description="Where fixture start time (in UTC) >= this value")
+        ] = None,
+        hide_null: Annotated[
+            Optional[StrictBool], Field(description="Don't display data fields with null values or empty structures")
+        ] = None,
+        include: Annotated[
+            Optional[StrictStr],
+            Field(
+                description="A comma separated list of resource types to include. See [Resource Inclusion](#section/Introduction/Resource-Inclusion) for more information."
+            ),
+        ] = None,
+        limit: Annotated[
+            Optional[conint(strict=True, le=1000, ge=1)],
+            Field(
+                description="The maximum number of records to return. See [Pagination](#section/Introduction/Pagination) for more information."
+            ),
+        ] = None,
+        live_data_available: Annotated[Optional[StrictBool], Field(description="Is live data available?")] = None,
+        live_video_available: Annotated[Optional[StrictBool], Field(description="Is live video available ?")] = None,
+        locked: Annotated[
+            Optional[StrictBool], Field(description="Is the fixture locked (to prevent editing)?")
+        ] = None,
+        offset: Annotated[
+            Optional[StrictInt],
+            Field(
+                description="The offset of the records. See [Pagination](#section/Introduction/Pagination) for more information."
+            ),
+        ] = None,
+        pool_code: Annotated[
+            Optional[constr(strict=True, max_length=30)], Field(description="The pool identifier within a season")
+        ] = None,
+        round_code: Annotated[
+            Optional[constr(strict=True, max_length=30)], Field(description="The round identifier within a season")
+        ] = None,
+        round_number: Annotated[Optional[constr(strict=True, max_length=30)], Field(description="Round number")] = None,
+        season_id: Annotated[Optional[StrictStr], Field(description="The unique identifier of the season")] = None,
+        sort_by: Annotated[
+            Optional[StrictStr],
+            Field(
+                description="Comma-delimited list of one or more fields to sort by, each field can have '-' as prefix to sort in descending order, and '+' (or no prefix) to sort in ascending order."
+            ),
+        ] = None,
+        stage_code: Annotated[
+            Optional[constr(strict=True, max_length=30)], Field(description="The stage identifier within a season")
+        ] = None,
+        status: Annotated[
+            Optional[constr(strict=True, max_length=200)],
+            Field(
+                description="Fixture status. Can specify multiple, delimited by comma. >- `ABANDONED` Abandoned >- `BYE` Bye >- `CANCELLED` Cancelled >- `CONFIRMED` Confirmed >- `FINISHED` Finished >- `IF_NEEDED` If Needed >- `IN_PROGRESS` In Progress >- `PENDING` Pending >- `POSTPONED` Postponed >- `SCHEDULED` Scheduled "
+            ),
+        ] = None,
+        times_unconfirmed: Annotated[
+            Optional[StrictBool], Field(description="Is the fixture time yet to be confirmed ?")
+        ] = None,
+        to_time_local: Annotated[
+            Optional[datetime], Field(description="Where fixture start time (in local time) <= this value")
+        ] = None,
+        to_time_utc: Annotated[
+            Optional[datetime], Field(description="Where fixture start time (in UTC) <= this value")
+        ] = None,
+        updated: Annotated[
+            Optional[datetime], Field(description="Record was modified after this date/time. In UTC.")
+        ] = None,
+        venue_id: Annotated[Optional[StrictStr], Field(description="The unique identifier of the venue")] = None,
+        **kwargs
+    ) -> ApiResponse:  # noqa: E501
+        """Get a list of fixtures for a Competition  # noqa: E501
+
+        Return a list of fixtures, for a specific Competition  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.fixture_by_competition_list_with_http_info(competition_id, organization_id, sport, added, competitor_type, external, fields, fixture_id, fixture_type, from_time_local, from_time_utc, hide_null, include, limit, live_data_available, live_video_available, locked, offset, pool_code, round_code, round_number, season_id, sort_by, stage_code, status, times_unconfirmed, to_time_local, to_time_utc, updated, venue_id, async_req=True)
+        >>> result = thread.get()
+
+        :param competition_id: The unique identifier of the competition (required)
+        :type competition_id: str
+        :param organization_id: The unique identifier of the organization (required)
+        :type organization_id: str
+        :param sport: Sport name (required)
+        :type sport: str
+        :param added: Record was added after this date/time. In UTC.
+        :type added: datetime
+        :param competitor_type: The type of competitors in this fixture >- `ENTITY` Entity >- `PERSON` Person
+        :type competitor_type: str
+        :param external: A comma separated list of fields that will instead be interpreted as an externalId. See [External Ids](#section/Introduction/External-Ids) for more information.
+        :type external: str
+        :param fields: A comma separated list of fields to display.  The response will only display these fields. See [Partial Response](#section/Partial-Response) section for more information.
+        :type fields: str
+        :param fixture_id: The unique identifier of the fixture
+        :type fixture_id: str
+        :param fixture_type: Type of Fixture >- `ALL_STAR` All Star >- `DEMONSTRATION` Demonstration >- `FINAL` Final >- `FRIENDLY` Friendly >- `PLAYOFF` Playoff >- `PRESEASON` Pre Season >- `REGULAR` Regular
+        :type fixture_type: str
+        :param from_time_local: Where fixture start time (in local time) >= this value
+        :type from_time_local: datetime
+        :param from_time_utc: Where fixture start time (in UTC) >= this value
+        :type from_time_utc: datetime
+        :param hide_null: Don't display data fields with null values or empty structures
+        :type hide_null: bool
+        :param include: A comma separated list of resource types to include. See [Resource Inclusion](#section/Introduction/Resource-Inclusion) for more information.
+        :type include: str
+        :param limit: The maximum number of records to return. See [Pagination](#section/Introduction/Pagination) for more information.
+        :type limit: int
+        :param live_data_available: Is live data available?
+        :type live_data_available: bool
+        :param live_video_available: Is live video available ?
+        :type live_video_available: bool
+        :param locked: Is the fixture locked (to prevent editing)?
+        :type locked: bool
+        :param offset: The offset of the records. See [Pagination](#section/Introduction/Pagination) for more information.
+        :type offset: int
+        :param pool_code: The pool identifier within a season
+        :type pool_code: str
+        :param round_code: The round identifier within a season
+        :type round_code: str
+        :param round_number: Round number
+        :type round_number: str
+        :param season_id: The unique identifier of the season
+        :type season_id: str
+        :param sort_by: Comma-delimited list of one or more fields to sort by, each field can have '-' as prefix to sort in descending order, and '+' (or no prefix) to sort in ascending order.
+        :type sort_by: str
+        :param stage_code: The stage identifier within a season
+        :type stage_code: str
+        :param status: Fixture status. Can specify multiple, delimited by comma. >- `ABANDONED` Abandoned >- `BYE` Bye >- `CANCELLED` Cancelled >- `CONFIRMED` Confirmed >- `FINISHED` Finished >- `IF_NEEDED` If Needed >- `IN_PROGRESS` In Progress >- `PENDING` Pending >- `POSTPONED` Postponed >- `SCHEDULED` Scheduled
+        :type status: str
+        :param times_unconfirmed: Is the fixture time yet to be confirmed ?
+        :type times_unconfirmed: bool
+        :param to_time_local: Where fixture start time (in local time) <= this value
+        :type to_time_local: datetime
+        :param to_time_utc: Where fixture start time (in UTC) <= this value
+        :type to_time_utc: datetime
+        :param updated: Record was modified after this date/time. In UTC.
+        :type updated: datetime
+        :param venue_id: The unique identifier of the venue
+        :type venue_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(FixturesByCompetitionResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            "competition_id",
+            "organization_id",
+            "sport",
+            "added",
+            "competitor_type",
+            "external",
+            "fields",
+            "fixture_id",
+            "fixture_type",
+            "from_time_local",
+            "from_time_utc",
+            "hide_null",
+            "include",
+            "limit",
+            "live_data_available",
+            "live_video_available",
+            "locked",
+            "offset",
+            "pool_code",
+            "round_code",
+            "round_number",
+            "season_id",
+            "sort_by",
+            "stage_code",
+            "status",
+            "times_unconfirmed",
+            "to_time_local",
+            "to_time_utc",
+            "updated",
+            "venue_id",
+        ]
+        _all_params.extend(
+            [
+                "async_req",
+                "_return_http_data_only",
+                "_preload_content",
+                "_request_timeout",
+                "_request_auth",
+                "_content_type",
+                "_headers",
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params["kwargs"].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'" " to method fixture_by_competition_list" % _key
+                )
+            _params[_key] = _val
+        del _params["kwargs"]
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params["competition_id"]:
+            _path_params["competitionId"] = _params["competition_id"]
+
+        if _params["organization_id"]:
+            _path_params["organizationId"] = _params["organization_id"]
+
+        if _params["sport"]:
+            _path_params["sport"] = _params["sport"]
+
+        # process the query parameters
+        _query_params = []
+        if _params.get("added") is not None:  # noqa: E501
+            if isinstance(_params["added"], datetime):
+                _query_params.append(
+                    ("added", _params["added"].strftime(self.api_client.configuration.datetime_format))
+                )
+            else:
+                _query_params.append(("added", _params["added"]))
+
+        if _params.get("competitor_type") is not None:  # noqa: E501
+            _query_params.append(("competitorType", _params["competitor_type"].value))
+
+        if _params.get("external") is not None:  # noqa: E501
+            _query_params.append(("external", _params["external"]))
+
+        if _params.get("fields") is not None:  # noqa: E501
+            _query_params.append(("fields", _params["fields"]))
+
+        if _params.get("fixture_id") is not None:  # noqa: E501
+            _query_params.append(("fixtureId", _params["fixture_id"]))
+
+        if _params.get("fixture_type") is not None:  # noqa: E501
+            _query_params.append(("fixtureType", _params["fixture_type"].value))
+
+        if _params.get("from_time_local") is not None:  # noqa: E501
+            if isinstance(_params["from_time_local"], datetime):
+                _query_params.append(
+                    (
+                        "fromTimeLocal",
+                        _params["from_time_local"].strftime(self.api_client.configuration.datetime_format),
+                    )
+                )
+            else:
+                _query_params.append(("fromTimeLocal", _params["from_time_local"]))
+
+        if _params.get("from_time_utc") is not None:  # noqa: E501
+            if isinstance(_params["from_time_utc"], datetime):
+                _query_params.append(
+                    ("fromTimeUTC", _params["from_time_utc"].strftime(self.api_client.configuration.datetime_format))
+                )
+            else:
+                _query_params.append(("fromTimeUTC", _params["from_time_utc"]))
+
+        if _params.get("hide_null") is not None:  # noqa: E501
+            _query_params.append(("hideNull", _params["hide_null"]))
+
+        if _params.get("include") is not None:  # noqa: E501
+            _query_params.append(("include", _params["include"]))
+
+        if _params.get("limit") is not None:  # noqa: E501
+            _query_params.append(("limit", _params["limit"]))
+
+        if _params.get("live_data_available") is not None:  # noqa: E501
+            _query_params.append(("liveDataAvailable", _params["live_data_available"]))
+
+        if _params.get("live_video_available") is not None:  # noqa: E501
+            _query_params.append(("liveVideoAvailable", _params["live_video_available"]))
+
+        if _params.get("locked") is not None:  # noqa: E501
+            _query_params.append(("locked", _params["locked"]))
+
+        if _params.get("offset") is not None:  # noqa: E501
+            _query_params.append(("offset", _params["offset"]))
+
+        if _params.get("pool_code") is not None:  # noqa: E501
+            _query_params.append(("poolCode", _params["pool_code"]))
+
+        if _params.get("round_code") is not None:  # noqa: E501
+            _query_params.append(("roundCode", _params["round_code"]))
+
+        if _params.get("round_number") is not None:  # noqa: E501
+            _query_params.append(("roundNumber", _params["round_number"]))
+
+        if _params.get("season_id") is not None:  # noqa: E501
+            _query_params.append(("seasonId", _params["season_id"]))
+
+        if _params.get("sort_by") is not None:  # noqa: E501
+            _query_params.append(("sortBy", _params["sort_by"]))
+
+        if _params.get("stage_code") is not None:  # noqa: E501
+            _query_params.append(("stageCode", _params["stage_code"]))
+
+        if _params.get("status") is not None:  # noqa: E501
+            _query_params.append(("status", _params["status"].value))
+
+        if _params.get("times_unconfirmed") is not None:  # noqa: E501
+            _query_params.append(("timesUnconfirmed", _params["times_unconfirmed"]))
+
+        if _params.get("to_time_local") is not None:  # noqa: E501
+            if isinstance(_params["to_time_local"], datetime):
+                _query_params.append(
+                    ("toTimeLocal", _params["to_time_local"].strftime(self.api_client.configuration.datetime_format))
+                )
+            else:
+                _query_params.append(("toTimeLocal", _params["to_time_local"]))
+
+        if _params.get("to_time_utc") is not None:  # noqa: E501
+            if isinstance(_params["to_time_utc"], datetime):
+                _query_params.append(
+                    ("toTimeUTC", _params["to_time_utc"].strftime(self.api_client.configuration.datetime_format))
+                )
+            else:
+                _query_params.append(("toTimeUTC", _params["to_time_utc"]))
+
+        if _params.get("updated") is not None:  # noqa: E501
+            if isinstance(_params["updated"], datetime):
+                _query_params.append(
+                    ("updated", _params["updated"].strftime(self.api_client.configuration.datetime_format))
+                )
+            else:
+                _query_params.append(("updated", _params["updated"]))
+
+        if _params.get("venue_id") is not None:  # noqa: E501
+            _query_params.append(("venueId", _params["venue_id"]))
+
+        # process the header parameters
+        _header_params = dict(_params.get("_headers", {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        # set the HTTP header `Accept`
+        _header_params["Accept"] = self.api_client.select_header_accept(["application/json"])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ["OAuth2"]  # noqa: E501
+
+        _response_types_map = {
+            "200": "FixturesByCompetitionResponse",
+        }
+
+        return self.api_client.call_api(
+            "/{sport}/o/{organizationId}/competitions/{competitionId}/fixtures",
+            "GET",
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get("async_req"),
+            _return_http_data_only=_params.get("_return_http_data_only"),  # noqa: E501
+            _preload_content=_params.get("_preload_content", True),
+            _request_timeout=_params.get("_request_timeout"),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get("_request_auth"),
+        )
+
+    @validate_arguments
     def fixture_by_entity_all_seasons_list(
         self,
         entity_id: Annotated[StrictStr, Field(..., description="The unique identifier of the entity")],
         organization_id: Annotated[
             constr(strict=True, max_length=5, min_length=5),
             Field(..., description="The unique identifier of the organization"),
         ],
@@ -747,14 +1395,17 @@
         pool_code: Annotated[
             Optional[constr(strict=True, max_length=30)], Field(description="The pool identifier within a season")
         ] = None,
         round_code: Annotated[
             Optional[constr(strict=True, max_length=30)], Field(description="The round identifier within a season")
         ] = None,
         round_number: Annotated[Optional[constr(strict=True, max_length=30)], Field(description="Round number")] = None,
+        series_code: Annotated[
+            Optional[constr(strict=True, max_length=30)], Field(description="The series identifier within a season")
+        ] = None,
         sort_by: Annotated[
             Optional[StrictStr],
             Field(
                 description="Comma-delimited list of one or more fields to sort by, each field can have '-' as prefix to sort in descending order, and '+' (or no prefix) to sort in ascending order."
             ),
         ] = None,
         stage_code: Annotated[
@@ -783,15 +1434,15 @@
     ) -> FixturesByEntityResponse:  # noqa: E501
         """Get a list of fixtures for an Entity  # noqa: E501
 
         Return a list of fixtures, within ~seasonprefix~ season, for a specific Entity  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.fixture_by_entity_list(entity_id, organization_id, season_id, sport, added, competitor_type, external, fields, fixture_type, from_time_local, from_time_utc, hide_null, include, is_home, limit, live_data_available, live_video_available, locked, offset, pool_code, round_code, round_number, sort_by, stage_code, status, times_unconfirmed, to_time_local, to_time_utc, updated, venue_id, async_req=True)
+        >>> thread = api.fixture_by_entity_list(entity_id, organization_id, season_id, sport, added, competitor_type, external, fields, fixture_type, from_time_local, from_time_utc, hide_null, include, is_home, limit, live_data_available, live_video_available, locked, offset, pool_code, round_code, round_number, series_code, sort_by, stage_code, status, times_unconfirmed, to_time_local, to_time_utc, updated, venue_id, async_req=True)
         >>> result = thread.get()
 
         :param entity_id: The unique identifier of the entity (required)
         :type entity_id: str
         :param organization_id: The unique identifier of the organization (required)
         :type organization_id: str
         :param season_id: The unique identifier of the season (required)
@@ -830,14 +1481,16 @@
         :type offset: int
         :param pool_code: The pool identifier within a season
         :type pool_code: str
         :param round_code: The round identifier within a season
         :type round_code: str
         :param round_number: Round number
         :type round_number: str
+        :param series_code: The series identifier within a season
+        :type series_code: str
         :param sort_by: Comma-delimited list of one or more fields to sort by, each field can have '-' as prefix to sort in descending order, and '+' (or no prefix) to sort in ascending order.
         :type sort_by: str
         :param stage_code: The stage identifier within a season
         :type stage_code: str
         :param status: Fixture status. Can specify multiple, delimited by comma. >- `ABANDONED` Abandoned >- `BYE` Bye >- `CANCELLED` Cancelled >- `CONFIRMED` Confirmed >- `FINISHED` Finished >- `IF_NEEDED` If Needed >- `IN_PROGRESS` In Progress >- `PENDING` Pending >- `POSTPONED` Postponed >- `SCHEDULED` Scheduled
         :type status: str
         :param times_unconfirmed: Is the fixture time yet to be confirmed ?
@@ -886,14 +1539,15 @@
                 live_data_available,
                 live_video_available,
                 locked,
                 offset,
                 pool_code,
                 round_code,
                 round_number,
+                series_code,
                 sort_by,
                 stage_code,
                 status,
                 times_unconfirmed,
                 to_time_local,
                 to_time_utc,
                 updated,
@@ -975,14 +1629,17 @@
         pool_code: Annotated[
             Optional[constr(strict=True, max_length=30)], Field(description="The pool identifier within a season")
         ] = None,
         round_code: Annotated[
             Optional[constr(strict=True, max_length=30)], Field(description="The round identifier within a season")
         ] = None,
         round_number: Annotated[Optional[constr(strict=True, max_length=30)], Field(description="Round number")] = None,
+        series_code: Annotated[
+            Optional[constr(strict=True, max_length=30)], Field(description="The series identifier within a season")
+        ] = None,
         sort_by: Annotated[
             Optional[StrictStr],
             Field(
                 description="Comma-delimited list of one or more fields to sort by, each field can have '-' as prefix to sort in descending order, and '+' (or no prefix) to sort in ascending order."
             ),
         ] = None,
         stage_code: Annotated[
@@ -1011,15 +1668,15 @@
     ) -> ApiResponse:  # noqa: E501
         """Get a list of fixtures for an Entity  # noqa: E501
 
         Return a list of fixtures, within ~seasonprefix~ season, for a specific Entity  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.fixture_by_entity_list_with_http_info(entity_id, organization_id, season_id, sport, added, competitor_type, external, fields, fixture_type, from_time_local, from_time_utc, hide_null, include, is_home, limit, live_data_available, live_video_available, locked, offset, pool_code, round_code, round_number, sort_by, stage_code, status, times_unconfirmed, to_time_local, to_time_utc, updated, venue_id, async_req=True)
+        >>> thread = api.fixture_by_entity_list_with_http_info(entity_id, organization_id, season_id, sport, added, competitor_type, external, fields, fixture_type, from_time_local, from_time_utc, hide_null, include, is_home, limit, live_data_available, live_video_available, locked, offset, pool_code, round_code, round_number, series_code, sort_by, stage_code, status, times_unconfirmed, to_time_local, to_time_utc, updated, venue_id, async_req=True)
         >>> result = thread.get()
 
         :param entity_id: The unique identifier of the entity (required)
         :type entity_id: str
         :param organization_id: The unique identifier of the organization (required)
         :type organization_id: str
         :param season_id: The unique identifier of the season (required)
@@ -1058,14 +1715,16 @@
         :type offset: int
         :param pool_code: The pool identifier within a season
         :type pool_code: str
         :param round_code: The round identifier within a season
         :type round_code: str
         :param round_number: Round number
         :type round_number: str
+        :param series_code: The series identifier within a season
+        :type series_code: str
         :param sort_by: Comma-delimited list of one or more fields to sort by, each field can have '-' as prefix to sort in descending order, and '+' (or no prefix) to sort in ascending order.
         :type sort_by: str
         :param stage_code: The stage identifier within a season
         :type stage_code: str
         :param status: Fixture status. Can specify multiple, delimited by comma. >- `ABANDONED` Abandoned >- `BYE` Bye >- `CANCELLED` Cancelled >- `CONFIRMED` Confirmed >- `FINISHED` Finished >- `IF_NEEDED` If Needed >- `IN_PROGRESS` In Progress >- `PENDING` Pending >- `POSTPONED` Postponed >- `SCHEDULED` Scheduled
         :type status: str
         :param times_unconfirmed: Is the fixture time yet to be confirmed ?
@@ -1124,14 +1783,15 @@
             "live_data_available",
             "live_video_available",
             "locked",
             "offset",
             "pool_code",
             "round_code",
             "round_number",
+            "series_code",
             "sort_by",
             "stage_code",
             "status",
             "times_unconfirmed",
             "to_time_local",
             "to_time_utc",
             "updated",
@@ -1242,14 +1902,17 @@
 
         if _params.get("round_code") is not None:  # noqa: E501
             _query_params.append(("roundCode", _params["round_code"]))
 
         if _params.get("round_number") is not None:  # noqa: E501
             _query_params.append(("roundNumber", _params["round_number"]))
 
+        if _params.get("series_code") is not None:  # noqa: E501
+            _query_params.append(("seriesCode", _params["series_code"]))
+
         if _params.get("sort_by") is not None:  # noqa: E501
             _query_params.append(("sortBy", _params["sort_by"]))
 
         if _params.get("stage_code") is not None:  # noqa: E501
             _query_params.append(("stageCode", _params["stage_code"]))
 
         if _params.get("status") is not None:  # noqa: E501
```

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/images_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/images_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/leader_criteria_sets_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/leader_criteria_sets_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/leader_qualifiers_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/leader_qualifiers_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/leagues_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/leagues_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/local_video_endpoints_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/local_video_endpoints_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/merge_records_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/merge_records_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/organizations_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/organizations_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/partner_apis_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/partner_apis_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/person_fixture_history_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/person_fixture_history_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/person_fixture_statistics_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/person_fixture_statistics_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/persons_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/persons_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/rankings_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/rankings_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/roles_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/roles_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_entities_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/season_entities_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_entity_base_statistics_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/season_entity_base_statistics_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_entity_placings_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/season_entity_placings_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_leaders_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/season_leaders_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_person_base_statistics_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/season_person_base_statistics_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_person_placings_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/season_person_placings_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_persons_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/season_persons_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_roster_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/season_roster_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_series_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/season_series_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/season_statistics_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/season_statistics_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/seasons_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/seasons_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/sites_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/sites_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/stages_pools_rounds_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/stages_pools_rounds_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/standing_adjustments_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/standing_adjustments_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/standing_configurations_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/standing_configurations_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/standings_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/standings_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/transfers_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/transfers_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/venues_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/venues_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1189,14 +1189,20 @@
         ] = None,
         limit: Annotated[
             Optional[conint(strict=True, le=1000, ge=1)],
             Field(
                 description="The maximum number of records to return. See [Pagination](#section/Introduction/Pagination) for more information."
             ),
         ] = None,
+        name_local_contains: Annotated[
+            Optional[constr(strict=True, max_length=50, min_length=2)],
+            Field(
+                description="Fields that allow a 'Contains' query string parameter search for words separated by a space, matching characters left to right. Example: nameLocal=David Johnson nameLocalContains=Dav will match nameLocalContains=John will match nameLocalContains=son will not match"
+            ),
+        ] = None,
         offset: Annotated[
             Optional[StrictInt],
             Field(
                 description="The offset of the records. See [Pagination](#section/Introduction/Pagination) for more information."
             ),
         ] = None,
         status: Annotated[
@@ -1210,15 +1216,15 @@
     ) -> VenuesResponse:  # noqa: E501
         """Get a list of venues  # noqa: E501
 
         Return a list of available venues  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.venue_list(organization_id, sport, added, country_code, external, fields, hide_null, include, limit, offset, status, updated, async_req=True)
+        >>> thread = api.venue_list(organization_id, sport, added, country_code, external, fields, hide_null, include, limit, name_local_contains, offset, status, updated, async_req=True)
         >>> result = thread.get()
 
         :param organization_id: The unique identifier of the organization (required)
         :type organization_id: str
         :param sport: Sport name (required)
         :type sport: str
         :param added: Record was added after this date/time. In UTC.
@@ -1231,14 +1237,16 @@
         :type fields: str
         :param hide_null: Don't display data fields with null values or empty structures
         :type hide_null: bool
         :param include: A comma separated list of resource types to include. See [Resource Inclusion](#section/Introduction/Resource-Inclusion) for more information.
         :type include: str
         :param limit: The maximum number of records to return. See [Pagination](#section/Introduction/Pagination) for more information.
         :type limit: int
+        :param name_local_contains: Fields that allow a 'Contains' query string parameter search for words separated by a space, matching characters left to right. Example: nameLocal=David Johnson nameLocalContains=Dav will match nameLocalContains=John will match nameLocalContains=son will not match
+        :type name_local_contains: str
         :param offset: The offset of the records. See [Pagination](#section/Introduction/Pagination) for more information.
         :type offset: int
         :param status: Status >- `ACTIVE` Active >- `INACTIVE` Inactive >- `PENDING` Pending
         :type status: str
         :param updated: Record was modified after this date/time. In UTC.
         :type updated: datetime
         :param async_req: Whether to execute the request asynchronously.
@@ -1264,14 +1272,15 @@
                 added,
                 country_code,
                 external,
                 fields,
                 hide_null,
                 include,
                 limit,
+                name_local_contains,
                 offset,
                 status,
                 updated,
                 **kwargs
             )  # noqa: E501
         except Exception as e:
             logger.error("Exception when calling VenuesApi->venue_list: %s\n" % e)
@@ -1314,14 +1323,20 @@
         ] = None,
         limit: Annotated[
             Optional[conint(strict=True, le=1000, ge=1)],
             Field(
                 description="The maximum number of records to return. See [Pagination](#section/Introduction/Pagination) for more information."
             ),
         ] = None,
+        name_local_contains: Annotated[
+            Optional[constr(strict=True, max_length=50, min_length=2)],
+            Field(
+                description="Fields that allow a 'Contains' query string parameter search for words separated by a space, matching characters left to right. Example: nameLocal=David Johnson nameLocalContains=Dav will match nameLocalContains=John will match nameLocalContains=son will not match"
+            ),
+        ] = None,
         offset: Annotated[
             Optional[StrictInt],
             Field(
                 description="The offset of the records. See [Pagination](#section/Introduction/Pagination) for more information."
             ),
         ] = None,
         status: Annotated[
@@ -1335,15 +1350,15 @@
     ) -> ApiResponse:  # noqa: E501
         """Get a list of venues  # noqa: E501
 
         Return a list of available venues  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.venue_list_with_http_info(organization_id, sport, added, country_code, external, fields, hide_null, include, limit, offset, status, updated, async_req=True)
+        >>> thread = api.venue_list_with_http_info(organization_id, sport, added, country_code, external, fields, hide_null, include, limit, name_local_contains, offset, status, updated, async_req=True)
         >>> result = thread.get()
 
         :param organization_id: The unique identifier of the organization (required)
         :type organization_id: str
         :param sport: Sport name (required)
         :type sport: str
         :param added: Record was added after this date/time. In UTC.
@@ -1356,14 +1371,16 @@
         :type fields: str
         :param hide_null: Don't display data fields with null values or empty structures
         :type hide_null: bool
         :param include: A comma separated list of resource types to include. See [Resource Inclusion](#section/Introduction/Resource-Inclusion) for more information.
         :type include: str
         :param limit: The maximum number of records to return. See [Pagination](#section/Introduction/Pagination) for more information.
         :type limit: int
+        :param name_local_contains: Fields that allow a 'Contains' query string parameter search for words separated by a space, matching characters left to right. Example: nameLocal=David Johnson nameLocalContains=Dav will match nameLocalContains=John will match nameLocalContains=son will not match
+        :type name_local_contains: str
         :param offset: The offset of the records. See [Pagination](#section/Introduction/Pagination) for more information.
         :type offset: int
         :param status: Status >- `ACTIVE` Active >- `INACTIVE` Inactive >- `PENDING` Pending
         :type status: str
         :param updated: Record was modified after this date/time. In UTC.
         :type updated: datetime
         :param async_req: Whether to execute the request asynchronously.
@@ -1399,14 +1416,15 @@
             "added",
             "country_code",
             "external",
             "fields",
             "hide_null",
             "include",
             "limit",
+            "name_local_contains",
             "offset",
             "status",
             "updated",
         ]
         _all_params.extend(
             [
                 "async_req",
@@ -1460,14 +1478,17 @@
 
         if _params.get("include") is not None:  # noqa: E501
             _query_params.append(("include", _params["include"]))
 
         if _params.get("limit") is not None:  # noqa: E501
             _query_params.append(("limit", _params["limit"]))
 
+        if _params.get("name_local_contains") is not None:  # noqa: E501
+            _query_params.append(("nameLocalContains", _params["name_local_contains"]))
+
         if _params.get("offset") is not None:  # noqa: E501
             _query_params.append(("offset", _params["offset"]))
 
         if _params.get("status") is not None:  # noqa: E501
             _query_params.append(("status", _params["status"].value))
 
         if _params.get("updated") is not None:  # noqa: E501
```

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/video_stream_inputs_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/video_stream_inputs_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/video_stream_subscriptions_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/video_stream_subscriptions_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api/video_streams_available_api.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api/video_streams_available_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api_client.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = "AtriumSportsSDK/1.3.2"
+        self.user_agent = "AtriumSportsSDK/1.4.0"
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
@@ -154,14 +154,15 @@
         _return_http_data_only=None,
         collection_formats=None,
         _preload_content=True,
         _request_timeout=None,
         _host=None,
         _request_auth=None,
     ):
+
         config = self.configuration
 
         # header parameters
         header_params = header_params or {}
         header_params.update(self.default_headers)
         if self.cookie:
             header_params["Cookie"] = self.cookie
```

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/api_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/api_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/configuration.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,15 +388,15 @@
         :return: The report for debugging.
         """
         return (
             "Python SDK Debug Report:\n"
             "OS: {env}\n"
             "Python Version: {pyversion}\n"
             "Version of the API: v1\n"
-            "SDK Package Version: 1.3.2".format(env=sys.platform, pyversion=sys.version)
+            "SDK Package Version: 1.4.0".format(env=sys.platform, pyversion=sys.version)
         )
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/exceptions.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/__init__.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,14 +182,16 @@
 from atriumsports.datacore.openapi.models.fixture_progressions_response import FixtureProgressionsResponse
 from atriumsports.datacore.openapi.models.fixture_put_body import FixturePutBody
 from atriumsports.datacore.openapi.models.fixture_roster_model import FixtureRosterModel
 from atriumsports.datacore.openapi.models.fixture_roster_model_organization import FixtureRosterModelOrganization
 from atriumsports.datacore.openapi.models.fixture_roster_post_body import FixtureRosterPostBody
 from atriumsports.datacore.openapi.models.fixture_roster_response import FixtureRosterResponse
 from atriumsports.datacore.openapi.models.fixture_videosteam_post_body import FixtureVideosteamPostBody
+from atriumsports.datacore.openapi.models.fixtures_by_competition_model import FixturesByCompetitionModel
+from atriumsports.datacore.openapi.models.fixtures_by_competition_response import FixturesByCompetitionResponse
 from atriumsports.datacore.openapi.models.fixtures_by_entity_model import FixturesByEntityModel
 from atriumsports.datacore.openapi.models.fixtures_by_entity_response import FixturesByEntityResponse
 from atriumsports.datacore.openapi.models.fixtures_model import FixturesModel
 from atriumsports.datacore.openapi.models.fixtures_model_fixture_profile import FixturesModelFixtureProfile
 from atriumsports.datacore.openapi.models.fixtures_model_organization import FixturesModelOrganization
 from atriumsports.datacore.openapi.models.fixtures_model_round import FixturesModelRound
 from atriumsports.datacore.openapi.models.fixtures_model_series import FixturesModelSeries
```

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/award_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/award_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/award_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/award_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/awards_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/awards_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/awards_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/awards_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/awards_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/awards_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/blank_model_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/blank_model_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/career_person_season_statistics_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/career_person_season_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/career_person_season_statistics_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/career_person_season_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/career_person_season_statistics_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/career_person_season_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/career_person_statistics_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/career_person_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/career_person_statistics_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/career_person_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/career_person_statistics_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/career_person_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/change_log_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/change_log_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/change_log_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/change_log_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/change_log_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/change_log_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_entity_statistics_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competition_entity_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_entity_statistics_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competition_entity_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_entity_statistics_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competition_entity_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_historical_name.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competition_historical_name.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_person_statistics_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competition_person_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_person_statistics_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competition_person_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_person_statistics_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competition_person_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competition_post_body.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     )
     historical_names: Optional[conlist(CompetitionHistoricalName)] = Field(
         None, alias="historicalNames", description="Array of competition historical names"
     )
     age_group: Optional[constr(strict=True, max_length=50)] = Field(
         None,
         alias="ageGroup",
-        description="The age group of the competition >- `JUNIOR` Junior >- `MASTERS` Masters >- `SENIOR` Senior >- `UNDER_15` Under 15 >- `UNDER_16` Under 16 >- `UNDER_17` Under 17 >- `UNDER_18` Under 18 >- `UNDER_19` Under 19 >- `UNDER_20` Under 20 >- `UNDER_21` Under 21 >- `UNDER_22` Under 22 >- `UNDER_23` Under 23 >- `YOUTH` Youth ",
+        description="The age group of the competition >- None None >- `JUNIOR` Junior >- `MASTERS` Masters >- `SENIOR` Senior >- `UNDER_15` Under 15 >- `UNDER_16` Under 16 >- `UNDER_17` Under 17 >- `UNDER_18` Under 18 >- `UNDER_19` Under 19 >- `UNDER_20` Under 20 >- `UNDER_21` Under 21 >- `UNDER_22` Under 22 >- `UNDER_23` Under 23 >- `YOUTH` Youth ",
     )
     __properties = [
         "competitionId",
         "leagueId",
         "internationalReference",
         "abbreviationLocal",
         "nameLocal",
@@ -127,17 +127,18 @@
             "UNDER_19",
             "UNDER_20",
             "UNDER_21",
             "UNDER_22",
             "UNDER_23",
             "SENIOR",
             "MASTERS",
+            "null",
         ):
             raise ValueError(
-                "must be one of enum values ('JUNIOR', 'YOUTH', 'UNDER_15', 'UNDER_16', 'UNDER_17', 'UNDER_18', 'UNDER_19', 'UNDER_20', 'UNDER_21', 'UNDER_22', 'UNDER_23', 'SENIOR', 'MASTERS')"
+                "must be one of enum values ('JUNIOR', 'YOUTH', 'UNDER_15', 'UNDER_16', 'UNDER_17', 'UNDER_18', 'UNDER_19', 'UNDER_20', 'UNDER_21', 'UNDER_22', 'UNDER_23', 'SENIOR', 'MASTERS', 'null')"
             )
         return value
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
@@ -200,14 +201,19 @@
             _dict["externalId"] = None
 
         # set to None if historical_names (nullable) is None
         # and __fields_set__ contains the field
         if self.historical_names is None and "historical_names" in self.__fields_set__:
             _dict["historicalNames"] = None
 
+        # set to None if age_group (nullable) is None
+        # and __fields_set__ contains the field
+        if self.age_group is None and "age_group" in self.__fields_set__:
+            _dict["ageGroup"] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> CompetitionPostBody:
         """Create an instance of CompetitionPostBody from a dict"""
         if obj is None:
             return None
```

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competition_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competition_put_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     )
     historical_names: Optional[conlist(CompetitionHistoricalName)] = Field(
         None, alias="historicalNames", description="Array of competition historical names"
     )
     age_group: Optional[constr(strict=True, max_length=50)] = Field(
         None,
         alias="ageGroup",
-        description="The age group of the competition >- `JUNIOR` Junior >- `MASTERS` Masters >- `SENIOR` Senior >- `UNDER_15` Under 15 >- `UNDER_16` Under 16 >- `UNDER_17` Under 17 >- `UNDER_18` Under 18 >- `UNDER_19` Under 19 >- `UNDER_20` Under 20 >- `UNDER_21` Under 21 >- `UNDER_22` Under 22 >- `UNDER_23` Under 23 >- `YOUTH` Youth ",
+        description="The age group of the competition >- None None >- `JUNIOR` Junior >- `MASTERS` Masters >- `SENIOR` Senior >- `UNDER_15` Under 15 >- `UNDER_16` Under 16 >- `UNDER_17` Under 17 >- `UNDER_18` Under 18 >- `UNDER_19` Under 19 >- `UNDER_20` Under 20 >- `UNDER_21` Under 21 >- `UNDER_22` Under 22 >- `UNDER_23` Under 23 >- `YOUTH` Youth ",
     )
     __properties = [
         "leagueId",
         "internationalReference",
         "abbreviationLocal",
         "nameLocal",
         "eventType",
@@ -123,17 +123,18 @@
             "UNDER_19",
             "UNDER_20",
             "UNDER_21",
             "UNDER_22",
             "UNDER_23",
             "SENIOR",
             "MASTERS",
+            "null",
         ):
             raise ValueError(
-                "must be one of enum values ('JUNIOR', 'YOUTH', 'UNDER_15', 'UNDER_16', 'UNDER_17', 'UNDER_18', 'UNDER_19', 'UNDER_20', 'UNDER_21', 'UNDER_22', 'UNDER_23', 'SENIOR', 'MASTERS')"
+                "must be one of enum values ('JUNIOR', 'YOUTH', 'UNDER_15', 'UNDER_16', 'UNDER_17', 'UNDER_18', 'UNDER_19', 'UNDER_20', 'UNDER_21', 'UNDER_22', 'UNDER_23', 'SENIOR', 'MASTERS', 'null')"
             )
         return value
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
@@ -196,14 +197,19 @@
             _dict["externalId"] = None
 
         # set to None if historical_names (nullable) is None
         # and __fields_set__ contains the field
         if self.historical_names is None and "historical_names" in self.__fields_set__:
             _dict["historicalNames"] = None
 
+        # set to None if age_group (nullable) is None
+        # and __fields_set__ contains the field
+        if self.age_group is None and "age_group" in self.__fields_set__:
+            _dict["ageGroup"] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> CompetitionPutBody:
         """Create an instance of CompetitionPutBody from a dict"""
         if obj is None:
             return None
```

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competitions_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         None, alias="historicalNames", description="Array of competition historical names"
     )
     updated: Optional[datetime] = Field(None, description="Date/time last modified. In UTC")
     added: Optional[datetime] = Field(None, description="Date/time added. In UTC")
     age_group: Optional[constr(strict=True, max_length=50)] = Field(
         None,
         alias="ageGroup",
-        description="The age group of the competition >- `JUNIOR` Junior >- `MASTERS` Masters >- `SENIOR` Senior >- `UNDER_15` Under 15 >- `UNDER_16` Under 16 >- `UNDER_17` Under 17 >- `UNDER_18` Under 18 >- `UNDER_19` Under 19 >- `UNDER_20` Under 20 >- `UNDER_21` Under 21 >- `UNDER_22` Under 22 >- `UNDER_23` Under 23 >- `YOUTH` Youth ",
+        description="The age group of the competition >- None None >- `JUNIOR` Junior >- `MASTERS` Masters >- `SENIOR` Senior >- `UNDER_15` Under 15 >- `UNDER_16` Under 16 >- `UNDER_17` Under 17 >- `UNDER_18` Under 18 >- `UNDER_19` Under 19 >- `UNDER_20` Under 20 >- `UNDER_21` Under 21 >- `UNDER_22` Under 22 >- `UNDER_23` Under 23 >- `YOUTH` Youth ",
     )
     images: Optional[conlist(ImagesModel)] = None
     __properties = [
         "competitionId",
         "organizationId",
         "organization",
         "leagueId",
@@ -145,17 +145,18 @@
             "UNDER_19",
             "UNDER_20",
             "UNDER_21",
             "UNDER_22",
             "UNDER_23",
             "SENIOR",
             "MASTERS",
+            "null",
         ):
             raise ValueError(
-                "must be one of enum values ('JUNIOR', 'YOUTH', 'UNDER_15', 'UNDER_16', 'UNDER_17', 'UNDER_18', 'UNDER_19', 'UNDER_20', 'UNDER_21', 'UNDER_22', 'UNDER_23', 'SENIOR', 'MASTERS')"
+                "must be one of enum values ('JUNIOR', 'YOUTH', 'UNDER_15', 'UNDER_16', 'UNDER_17', 'UNDER_18', 'UNDER_19', 'UNDER_20', 'UNDER_21', 'UNDER_22', 'UNDER_23', 'SENIOR', 'MASTERS', 'null')"
             )
         return value
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
@@ -239,14 +240,19 @@
             _dict["externalId"] = None
 
         # set to None if historical_names (nullable) is None
         # and __fields_set__ contains the field
         if self.historical_names is None and "historical_names" in self.__fields_set__:
             _dict["historicalNames"] = None
 
+        # set to None if age_group (nullable) is None
+        # and __fields_set__ contains the field
+        if self.age_group is None and "age_group" in self.__fields_set__:
+            _dict["ageGroup"] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> CompetitionsModel:
         """Create an instance of CompetitionsModel from a dict"""
         if obj is None:
             return None
```

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_model_league.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competitions_model_league.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competitions_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competitions_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_season_status_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competitions_season_status_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         None, alias="historicalNames", description="Array of competition historical names"
     )
     updated: Optional[datetime] = Field(None, description="Date/time last modified. In UTC")
     added: Optional[datetime] = Field(None, description="Date/time added. In UTC")
     age_group: Optional[constr(strict=True, max_length=50)] = Field(
         None,
         alias="ageGroup",
-        description="The age group of the competition >- `JUNIOR` Junior >- `MASTERS` Masters >- `SENIOR` Senior >- `UNDER_15` Under 15 >- `UNDER_16` Under 16 >- `UNDER_17` Under 17 >- `UNDER_18` Under 18 >- `UNDER_19` Under 19 >- `UNDER_20` Under 20 >- `UNDER_21` Under 21 >- `UNDER_22` Under 22 >- `UNDER_23` Under 23 >- `YOUTH` Youth ",
+        description="The age group of the competition >- None None >- `JUNIOR` Junior >- `MASTERS` Masters >- `SENIOR` Senior >- `UNDER_15` Under 15 >- `UNDER_16` Under 16 >- `UNDER_17` Under 17 >- `UNDER_18` Under 18 >- `UNDER_19` Under 19 >- `UNDER_20` Under 20 >- `UNDER_21` Under 21 >- `UNDER_22` Under 22 >- `UNDER_23` Under 23 >- `YOUTH` Youth ",
     )
     images: Optional[conlist(ImagesModel)] = None
     __properties = [
         "competitionId",
         "organizationId",
         "organization",
         "leagueId",
@@ -149,17 +149,18 @@
             "UNDER_19",
             "UNDER_20",
             "UNDER_21",
             "UNDER_22",
             "UNDER_23",
             "SENIOR",
             "MASTERS",
+            "null",
         ):
             raise ValueError(
-                "must be one of enum values ('JUNIOR', 'YOUTH', 'UNDER_15', 'UNDER_16', 'UNDER_17', 'UNDER_18', 'UNDER_19', 'UNDER_20', 'UNDER_21', 'UNDER_22', 'UNDER_23', 'SENIOR', 'MASTERS')"
+                "must be one of enum values ('JUNIOR', 'YOUTH', 'UNDER_15', 'UNDER_16', 'UNDER_17', 'UNDER_18', 'UNDER_19', 'UNDER_20', 'UNDER_21', 'UNDER_22', 'UNDER_23', 'SENIOR', 'MASTERS', 'null')"
             )
         return value
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
@@ -243,14 +244,19 @@
             _dict["externalId"] = None
 
         # set to None if historical_names (nullable) is None
         # and __fields_set__ contains the field
         if self.historical_names is None and "historical_names" in self.__fields_set__:
             _dict["historicalNames"] = None
 
+        # set to None if age_group (nullable) is None
+        # and __fields_set__ contains the field
+        if self.age_group is None and "age_group" in self.__fields_set__:
+            _dict["ageGroup"] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> CompetitionsSeasonStatusModel:
         """Create an instance of CompetitionsSeasonStatusModel from a dict"""
         if obj is None:
             return None
```

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_season_status_model_league.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competitions_season_status_model_league.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_season_status_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competitions_season_status_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/competitions_season_status_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/competitions_season_status_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conduct_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/conduct_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,53 +73,55 @@
         None, description="The section of the period (sub-period)"
     )
     fixture_clock: Optional[constr(strict=True, max_length=20)] = Field(
         None, alias="fixtureClock", description="Fixture clock when the incident occurred"
     )
     role: Optional[constr(strict=True, max_length=100)] = Field(
         None,
-        description="The role of person >- `CAPTAIN` Captain >- `CAPTAIN_VICE` Vice Captain >- `CEO` CEO >- `COACH` Coach >- `COACH_ASSISTANT` Assistant Coach >- `COACH_ASSISTANT_HEAD` Assistant Head Coach >- `COACH_ASSOCIATE_HEAD` Associate Head Coach >- `COACH_DEVELOPMENT` Development Coach >- `COACH_HEAD` Head Coach >- `COACH_HEAD_INTERIM` Interim Head Coach >- `COACH_OTHER` Other coaching staff >- `COACH_SC` Strengh and Conditioning Coach >- `COACH_SENIOR` Senior Coach >- `COACH_SPECIALIST` Specialist Coach >- `COMMISSIONER` Commissioner >- `COMMITTEE` Committee >- `CREW_CHIEF` Crew Chief >- `DIRECTOR` Director >- `DOCTOR` Doctor >- `GENERAL` General >- `GROUNDSKEEPER` Groundskeeper >- `JUDGE_SCORING` Scoring Judge (SJ) >- `JUDGE_TIMING` Timing Judge (TJ) >- `MANAGER` Manager >- `MATCH_OFFICIAL` Match Official >- `MEDIA_OFFICER` Media Officer >- `MEDICAL_STAFF` Medical Staff >- `OTHER` Other >- `PHYSIOTHERAPIST` Physiotherapist >- `PRESIDENT` President >- `PRESIDENT_VICE` Vice President >- `REFEREE` Referee >- `REFEREE_ASSISTANT` Referee Assistant >- `REFEREE_ASSISTANT_RESERVE` Reserve Assistant Referee >- `REFEREE_RESERVE` Reserve Referee >- `SCOREKEEPER` Scorekeeper >- `SCOREKEEPER_ASSISTANT` Assistant Scorekeeper >- `SCORER` Scorer >- `SCORER_ASSISTANT` Assistant Scorer >- `SECRETARY` Secretary >- `STATISTICIAN` Statistician >- `TECHNICAL_OFFICIAL` Technical Official (TO) >- `TIMEKEEPER` Timekeeper >- `TIMER` Timer >- `TRAINER` Trainer >- `TRAINER_ASSISTANT` Assitant Trainer >- `TRANSLATOR` Translator >- `TREASURER` Treasurer >- `UMPIRE` Umpire >- `UMPIRE_RESERVE` Reserve Umpire (RU) >- `UMPIRE_VIDEO` Video Umpire (VU) >- `VIDEO_TECHNICIAN` Video Technician (VT) ",
+        description="The role of person >- None None >- `CAPTAIN` Captain >- `CAPTAIN_VICE` Vice Captain >- `CEO` CEO >- `COACH` Coach >- `COACH_ASSISTANT` Assistant Coach >- `COACH_ASSISTANT_HEAD` Assistant Head Coach >- `COACH_ASSOCIATE_HEAD` Associate Head Coach >- `COACH_DEVELOPMENT` Development Coach >- `COACH_HEAD` Head Coach >- `COACH_HEAD_INTERIM` Interim Head Coach >- `COACH_OTHER` Other coaching staff >- `COACH_SC` Strengh and Conditioning Coach >- `COACH_SENIOR` Senior Coach >- `COACH_SPECIALIST` Specialist Coach >- `COMMISSIONER` Commissioner >- `COMMITTEE` Committee >- `CREW_CHIEF` Crew Chief >- `DIRECTOR` Director >- `DOCTOR` Doctor >- `GENERAL` General >- `GROUNDSKEEPER` Groundskeeper >- `JUDGE_SCORING` Scoring Judge (SJ) >- `JUDGE_TIMING` Timing Judge (TJ) >- `MANAGER` Manager >- `MATCH_OFFICIAL` Match Official >- `MEDIA_OFFICER` Media Officer >- `MEDICAL_STAFF` Medical Staff >- `OTHER` Other >- `PHYSIOTHERAPIST` Physiotherapist >- `PRESIDENT` President >- `PRESIDENT_VICE` Vice President >- `REFEREE` Referee >- `REFEREE_ASSISTANT` Referee Assistant >- `REFEREE_ASSISTANT_RESERVE` Reserve Assistant Referee >- `REFEREE_RESERVE` Reserve Referee >- `SCOREKEEPER` Scorekeeper >- `SCOREKEEPER_ASSISTANT` Assistant Scorekeeper >- `SCORER` Scorer >- `SCORER_ASSISTANT` Assistant Scorer >- `SECRETARY` Secretary >- `STATISTICIAN` Statistician >- `TECHNICAL_OFFICIAL` Technical Official (TO) >- `TIMEKEEPER` Timekeeper >- `TIMER` Timer >- `TRAINER` Trainer >- `TRAINER_ASSISTANT` Assitant Trainer >- `TRANSLATOR` Translator >- `TREASURER` Treasurer >- `UMPIRE` Umpire >- `UMPIRE_RESERVE` Reserve Umpire (RU) >- `UMPIRE_VIDEO` Video Umpire (VU) >- `VIDEO_TECHNICIAN` Video Technician (VT) ",
     )
     date_offence_local: Optional[datetime] = Field(
         None, alias="dateOffenceLocal", description="Date & Time of the Offence in the local timezone"
     )
     conduct_type: Optional[conlist(StrictStr, min_items=1)] = Field(None, alias="conductType")
     conduct_notes: Optional[constr(strict=True, max_length=2000)] = Field(
         None, alias="conductNotes", description="Notes of the Conduct incident"
     )
     date_hearing_local: Optional[date] = Field(None, alias="dateHearingLocal", description="Date hearing")
     hearing_notes: Optional[constr(strict=True, max_length=500)] = Field(
         None, alias="hearingNotes", description="Notes from the conduct hearing"
     )
     hearing_status: Optional[StrictStr] = Field(
-        None, alias="hearingStatus", description="Conduct hearing status >- `FINALIZED` Finalized >- `PENDING` Pending "
+        None,
+        alias="hearingStatus",
+        description="Conduct hearing status >- None None >- `FINALIZED` Finalized >- `PENDING` Pending ",
     )
     life_sentence: Optional[StrictBool] = Field(
         None, alias="lifeSentence", description="Was the result of the conduct hearing a life sentence?"
     )
     penalty_results: Optional[conlist(ConductPenaltyResult)] = Field(None, alias="penaltyResults")
     fine_amount: Optional[Union[StrictFloat, StrictInt]] = Field(
         None, alias="fineAmount", description="Conduct fine amount"
     )
     fine_currency: Optional[constr(strict=True, max_length=20)] = Field(
         None, alias="fineCurrency", description="Fine currency"
     )
     fine_status: Optional[StrictStr] = Field(
         None,
         alias="fineStatus",
-        description="Conduct fine due status >- `CANCELLED` Cancelled >- `ISSUED` Issued >- `OTHER` Other >- `PAID` Paid >- `UNPAID` Unpaid ",
+        description="Conduct fine due status >- None None >- `CANCELLED` Cancelled >- `ISSUED` Issued >- `OTHER` Other >- `PAID` Paid >- `UNPAID` Unpaid ",
     )
     date_suspended_to: Optional[date] = Field(None, alias="dateSuspendedTo", description="Date the suspension ended")
     date_suspended_from: Optional[date] = Field(
         None, alias="dateSuspendedFrom", description="Date the suspension started"
     )
     date_fine_paid_local: Optional[date] = Field(None, alias="dateFinePaidLocal", description="Date the fine was paid")
     status: Optional[constr(strict=True, max_length=30)] = Field(
         None,
-        description="Conduct status >- `ACTIVE` Active >- `CLOSED` Closed >- `COMPLETE` Complete >- `INACTIVE` Inactive >- `PENDING` Pending ",
+        description="Conduct status >- None None >- `ACTIVE` Active >- `CLOSED` Closed >- `COMPLETE` Complete >- `INACTIVE` Inactive >- `PENDING` Pending ",
     )
     external_id: Optional[constr(strict=True, max_length=150)] = Field(
         None, alias="externalId", description="The Id of the data as set by the provider of the data"
     )
     updated: Optional[datetime] = Field(None, description="Date/time last modified. In UTC")
     added: Optional[datetime] = Field(None, description="Date/time added. In UTC")
     __properties = [
@@ -222,17 +224,18 @@
             "UMPIRE_VIDEO",
             "JUDGE_SCORING",
             "JUDGE_TIMING",
             "TECHNICAL_OFFICIAL",
             "VIDEO_TECHNICIAN",
             "TRANSLATOR",
             "MEDIA_OFFICER",
+            "null",
         ):
             raise ValueError(
-                "must be one of enum values ('COACH', 'COACH_HEAD', 'COACH_HEAD_INTERIM', 'COACH_ASSISTANT', 'COACH_ASSISTANT_HEAD', 'COACH_ASSOCIATE_HEAD', 'COACH_SC', 'COACH_SENIOR', 'COACH_DEVELOPMENT', 'COACH_SPECIALIST', 'COACH_OTHER', 'CAPTAIN', 'CAPTAIN_VICE', 'DOCTOR', 'PHYSIOTHERAPIST', 'MEDICAL_STAFF', 'TRAINER', 'TRAINER_ASSISTANT', 'MATCH_OFFICIAL', 'COMMISSIONER', 'STATISTICIAN', 'SCOREKEEPER', 'SCOREKEEPER_ASSISTANT', 'TIMEKEEPER', 'SCORER', 'SCORER_ASSISTANT', 'TIMER', 'GROUNDSKEEPER', 'CEO', 'COMMITTEE', 'PRESIDENT', 'DIRECTOR', 'PRESIDENT_VICE', 'SECRETARY', 'TREASURER', 'MANAGER', 'GENERAL', 'OTHER', 'REFEREE', 'UMPIRE', 'REFEREE_ASSISTANT', 'REFEREE_RESERVE', 'REFEREE_ASSISTANT_RESERVE', 'CREW_CHIEF', 'UMPIRE_RESERVE', 'UMPIRE_VIDEO', 'JUDGE_SCORING', 'JUDGE_TIMING', 'TECHNICAL_OFFICIAL', 'VIDEO_TECHNICIAN', 'TRANSLATOR', 'MEDIA_OFFICER')"
+                "must be one of enum values ('COACH', 'COACH_HEAD', 'COACH_HEAD_INTERIM', 'COACH_ASSISTANT', 'COACH_ASSISTANT_HEAD', 'COACH_ASSOCIATE_HEAD', 'COACH_SC', 'COACH_SENIOR', 'COACH_DEVELOPMENT', 'COACH_SPECIALIST', 'COACH_OTHER', 'CAPTAIN', 'CAPTAIN_VICE', 'DOCTOR', 'PHYSIOTHERAPIST', 'MEDICAL_STAFF', 'TRAINER', 'TRAINER_ASSISTANT', 'MATCH_OFFICIAL', 'COMMISSIONER', 'STATISTICIAN', 'SCOREKEEPER', 'SCOREKEEPER_ASSISTANT', 'TIMEKEEPER', 'SCORER', 'SCORER_ASSISTANT', 'TIMER', 'GROUNDSKEEPER', 'CEO', 'COMMITTEE', 'PRESIDENT', 'DIRECTOR', 'PRESIDENT_VICE', 'SECRETARY', 'TREASURER', 'MANAGER', 'GENERAL', 'OTHER', 'REFEREE', 'UMPIRE', 'REFEREE_ASSISTANT', 'REFEREE_RESERVE', 'REFEREE_ASSISTANT_RESERVE', 'CREW_CHIEF', 'UMPIRE_RESERVE', 'UMPIRE_VIDEO', 'JUDGE_SCORING', 'JUDGE_TIMING', 'TECHNICAL_OFFICIAL', 'VIDEO_TECHNICIAN', 'TRANSLATOR', 'MEDIA_OFFICER', 'null')"
             )
         return value
 
     @validator("conduct_type")
     def conduct_type_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
@@ -256,36 +259,38 @@
 
     @validator("hearing_status")
     def hearing_status_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("PENDING", "FINALIZED"):
-            raise ValueError("must be one of enum values ('PENDING', 'FINALIZED')")
+        if value not in ("PENDING", "FINALIZED", "null"):
+            raise ValueError("must be one of enum values ('PENDING', 'FINALIZED', 'null')")
         return value
 
     @validator("fine_status")
     def fine_status_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("ISSUED", "PAID", "UNPAID", "CANCELLED", "OTHER"):
-            raise ValueError("must be one of enum values ('ISSUED', 'PAID', 'UNPAID', 'CANCELLED', 'OTHER')")
+        if value not in ("ISSUED", "PAID", "UNPAID", "CANCELLED", "OTHER", "null"):
+            raise ValueError("must be one of enum values ('ISSUED', 'PAID', 'UNPAID', 'CANCELLED', 'OTHER', 'null')")
         return value
 
     @validator("status")
     def status_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("ACTIVE", "INACTIVE", "PENDING", "COMPLETE", "CLOSED"):
-            raise ValueError("must be one of enum values ('ACTIVE', 'INACTIVE', 'PENDING', 'COMPLETE', 'CLOSED')")
+        if value not in ("ACTIVE", "INACTIVE", "PENDING", "COMPLETE", "CLOSED", "null"):
+            raise ValueError(
+                "must be one of enum values ('ACTIVE', 'INACTIVE', 'PENDING', 'COMPLETE', 'CLOSED', 'null')"
+            )
         return value
 
     @validator("external_id")
     def external_id_validate_regular_expression(cls, value):
         """Validates the regular expression"""
         if value is None:
             return value
@@ -391,14 +396,19 @@
             _dict["dateHearingLocal"] = None
 
         # set to None if hearing_notes (nullable) is None
         # and __fields_set__ contains the field
         if self.hearing_notes is None and "hearing_notes" in self.__fields_set__:
             _dict["hearingNotes"] = None
 
+        # set to None if hearing_status (nullable) is None
+        # and __fields_set__ contains the field
+        if self.hearing_status is None and "hearing_status" in self.__fields_set__:
+            _dict["hearingStatus"] = None
+
         # set to None if fine_currency (nullable) is None
         # and __fields_set__ contains the field
         if self.fine_currency is None and "fine_currency" in self.__fields_set__:
             _dict["fineCurrency"] = None
 
         # set to None if fine_status (nullable) is None
         # and __fields_set__ contains the field
```

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conduct_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/conduct_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conduct_penalty_result.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/conduct_penalty_result.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conduct_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/conduct_post_body.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,53 +54,55 @@
         None, description="The section of the period (sub-period)"
     )
     fixture_clock: Optional[constr(strict=True, max_length=20)] = Field(
         None, alias="fixtureClock", description="Fixture clock when the incident occurred"
     )
     role: Optional[constr(strict=True, max_length=100)] = Field(
         None,
-        description="The role of person >- `CAPTAIN` Captain >- `CAPTAIN_VICE` Vice Captain >- `CEO` CEO >- `COACH` Coach >- `COACH_ASSISTANT` Assistant Coach >- `COACH_ASSISTANT_HEAD` Assistant Head Coach >- `COACH_ASSOCIATE_HEAD` Associate Head Coach >- `COACH_DEVELOPMENT` Development Coach >- `COACH_HEAD` Head Coach >- `COACH_HEAD_INTERIM` Interim Head Coach >- `COACH_OTHER` Other coaching staff >- `COACH_SC` Strengh and Conditioning Coach >- `COACH_SENIOR` Senior Coach >- `COACH_SPECIALIST` Specialist Coach >- `COMMISSIONER` Commissioner >- `COMMITTEE` Committee >- `CREW_CHIEF` Crew Chief >- `DIRECTOR` Director >- `DOCTOR` Doctor >- `GENERAL` General >- `GROUNDSKEEPER` Groundskeeper >- `JUDGE_SCORING` Scoring Judge (SJ) >- `JUDGE_TIMING` Timing Judge (TJ) >- `MANAGER` Manager >- `MATCH_OFFICIAL` Match Official >- `MEDIA_OFFICER` Media Officer >- `MEDICAL_STAFF` Medical Staff >- `OTHER` Other >- `PHYSIOTHERAPIST` Physiotherapist >- `PRESIDENT` President >- `PRESIDENT_VICE` Vice President >- `REFEREE` Referee >- `REFEREE_ASSISTANT` Referee Assistant >- `REFEREE_ASSISTANT_RESERVE` Reserve Assistant Referee >- `REFEREE_RESERVE` Reserve Referee >- `SCOREKEEPER` Scorekeeper >- `SCOREKEEPER_ASSISTANT` Assistant Scorekeeper >- `SCORER` Scorer >- `SCORER_ASSISTANT` Assistant Scorer >- `SECRETARY` Secretary >- `STATISTICIAN` Statistician >- `TECHNICAL_OFFICIAL` Technical Official (TO) >- `TIMEKEEPER` Timekeeper >- `TIMER` Timer >- `TRAINER` Trainer >- `TRAINER_ASSISTANT` Assitant Trainer >- `TRANSLATOR` Translator >- `TREASURER` Treasurer >- `UMPIRE` Umpire >- `UMPIRE_RESERVE` Reserve Umpire (RU) >- `UMPIRE_VIDEO` Video Umpire (VU) >- `VIDEO_TECHNICIAN` Video Technician (VT) ",
+        description="The role of person >- None None >- `CAPTAIN` Captain >- `CAPTAIN_VICE` Vice Captain >- `CEO` CEO >- `COACH` Coach >- `COACH_ASSISTANT` Assistant Coach >- `COACH_ASSISTANT_HEAD` Assistant Head Coach >- `COACH_ASSOCIATE_HEAD` Associate Head Coach >- `COACH_DEVELOPMENT` Development Coach >- `COACH_HEAD` Head Coach >- `COACH_HEAD_INTERIM` Interim Head Coach >- `COACH_OTHER` Other coaching staff >- `COACH_SC` Strengh and Conditioning Coach >- `COACH_SENIOR` Senior Coach >- `COACH_SPECIALIST` Specialist Coach >- `COMMISSIONER` Commissioner >- `COMMITTEE` Committee >- `CREW_CHIEF` Crew Chief >- `DIRECTOR` Director >- `DOCTOR` Doctor >- `GENERAL` General >- `GROUNDSKEEPER` Groundskeeper >- `JUDGE_SCORING` Scoring Judge (SJ) >- `JUDGE_TIMING` Timing Judge (TJ) >- `MANAGER` Manager >- `MATCH_OFFICIAL` Match Official >- `MEDIA_OFFICER` Media Officer >- `MEDICAL_STAFF` Medical Staff >- `OTHER` Other >- `PHYSIOTHERAPIST` Physiotherapist >- `PRESIDENT` President >- `PRESIDENT_VICE` Vice President >- `REFEREE` Referee >- `REFEREE_ASSISTANT` Referee Assistant >- `REFEREE_ASSISTANT_RESERVE` Reserve Assistant Referee >- `REFEREE_RESERVE` Reserve Referee >- `SCOREKEEPER` Scorekeeper >- `SCOREKEEPER_ASSISTANT` Assistant Scorekeeper >- `SCORER` Scorer >- `SCORER_ASSISTANT` Assistant Scorer >- `SECRETARY` Secretary >- `STATISTICIAN` Statistician >- `TECHNICAL_OFFICIAL` Technical Official (TO) >- `TIMEKEEPER` Timekeeper >- `TIMER` Timer >- `TRAINER` Trainer >- `TRAINER_ASSISTANT` Assitant Trainer >- `TRANSLATOR` Translator >- `TREASURER` Treasurer >- `UMPIRE` Umpire >- `UMPIRE_RESERVE` Reserve Umpire (RU) >- `UMPIRE_VIDEO` Video Umpire (VU) >- `VIDEO_TECHNICIAN` Video Technician (VT) ",
     )
     date_offence_local: Optional[datetime] = Field(
         None, alias="dateOffenceLocal", description="Date & Time of the Offence in the local timezone"
     )
     conduct_type: conlist(StrictStr, min_items=1) = Field(..., alias="conductType")
     conduct_notes: Optional[constr(strict=True, max_length=2000)] = Field(
         None, alias="conductNotes", description="Notes of the Conduct incident"
     )
     date_hearing_local: Optional[date] = Field(None, alias="dateHearingLocal", description="Date hearing")
     hearing_notes: Optional[constr(strict=True, max_length=500)] = Field(
         None, alias="hearingNotes", description="Notes from the conduct hearing"
     )
     hearing_status: Optional[StrictStr] = Field(
-        None, alias="hearingStatus", description="Conduct hearing status >- `FINALIZED` Finalized >- `PENDING` Pending "
+        None,
+        alias="hearingStatus",
+        description="Conduct hearing status >- None None >- `FINALIZED` Finalized >- `PENDING` Pending ",
     )
     life_sentence: Optional[StrictBool] = Field(
         None, alias="lifeSentence", description="Was the result of the conduct hearing a life sentence?"
     )
     penalty_results: Optional[conlist(ConductPenaltyResult)] = Field(None, alias="penaltyResults")
     fine_amount: Optional[Union[StrictFloat, StrictInt]] = Field(
         None, alias="fineAmount", description="Conduct fine amount"
     )
     fine_currency: Optional[constr(strict=True, max_length=20)] = Field(
         None, alias="fineCurrency", description="Fine currency"
     )
     fine_status: Optional[StrictStr] = Field(
         None,
         alias="fineStatus",
-        description="Conduct fine due status >- `CANCELLED` Cancelled >- `ISSUED` Issued >- `OTHER` Other >- `PAID` Paid >- `UNPAID` Unpaid ",
+        description="Conduct fine due status >- None None >- `CANCELLED` Cancelled >- `ISSUED` Issued >- `OTHER` Other >- `PAID` Paid >- `UNPAID` Unpaid ",
     )
     date_suspended_to: Optional[date] = Field(None, alias="dateSuspendedTo", description="Date the suspension ended")
     date_suspended_from: Optional[date] = Field(
         None, alias="dateSuspendedFrom", description="Date the suspension started"
     )
     date_fine_paid_local: Optional[date] = Field(None, alias="dateFinePaidLocal", description="Date the fine was paid")
     status: Optional[constr(strict=True, max_length=30)] = Field(
         None,
-        description="Conduct status >- `ACTIVE` Active >- `CLOSED` Closed >- `COMPLETE` Complete >- `INACTIVE` Inactive >- `PENDING` Pending ",
+        description="Conduct status >- None None >- `ACTIVE` Active >- `CLOSED` Closed >- `COMPLETE` Complete >- `INACTIVE` Inactive >- `PENDING` Pending ",
     )
     external_id: Optional[constr(strict=True, max_length=150)] = Field(
         None, alias="externalId", description="The Id of the data as set by the provider of the data"
     )
     __properties = [
         "conductId",
         "personId",
@@ -190,17 +192,18 @@
             "UMPIRE_VIDEO",
             "JUDGE_SCORING",
             "JUDGE_TIMING",
             "TECHNICAL_OFFICIAL",
             "VIDEO_TECHNICIAN",
             "TRANSLATOR",
             "MEDIA_OFFICER",
+            "null",
         ):
             raise ValueError(
-                "must be one of enum values ('COACH', 'COACH_HEAD', 'COACH_HEAD_INTERIM', 'COACH_ASSISTANT', 'COACH_ASSISTANT_HEAD', 'COACH_ASSOCIATE_HEAD', 'COACH_SC', 'COACH_SENIOR', 'COACH_DEVELOPMENT', 'COACH_SPECIALIST', 'COACH_OTHER', 'CAPTAIN', 'CAPTAIN_VICE', 'DOCTOR', 'PHYSIOTHERAPIST', 'MEDICAL_STAFF', 'TRAINER', 'TRAINER_ASSISTANT', 'MATCH_OFFICIAL', 'COMMISSIONER', 'STATISTICIAN', 'SCOREKEEPER', 'SCOREKEEPER_ASSISTANT', 'TIMEKEEPER', 'SCORER', 'SCORER_ASSISTANT', 'TIMER', 'GROUNDSKEEPER', 'CEO', 'COMMITTEE', 'PRESIDENT', 'DIRECTOR', 'PRESIDENT_VICE', 'SECRETARY', 'TREASURER', 'MANAGER', 'GENERAL', 'OTHER', 'REFEREE', 'UMPIRE', 'REFEREE_ASSISTANT', 'REFEREE_RESERVE', 'REFEREE_ASSISTANT_RESERVE', 'CREW_CHIEF', 'UMPIRE_RESERVE', 'UMPIRE_VIDEO', 'JUDGE_SCORING', 'JUDGE_TIMING', 'TECHNICAL_OFFICIAL', 'VIDEO_TECHNICIAN', 'TRANSLATOR', 'MEDIA_OFFICER')"
+                "must be one of enum values ('COACH', 'COACH_HEAD', 'COACH_HEAD_INTERIM', 'COACH_ASSISTANT', 'COACH_ASSISTANT_HEAD', 'COACH_ASSOCIATE_HEAD', 'COACH_SC', 'COACH_SENIOR', 'COACH_DEVELOPMENT', 'COACH_SPECIALIST', 'COACH_OTHER', 'CAPTAIN', 'CAPTAIN_VICE', 'DOCTOR', 'PHYSIOTHERAPIST', 'MEDICAL_STAFF', 'TRAINER', 'TRAINER_ASSISTANT', 'MATCH_OFFICIAL', 'COMMISSIONER', 'STATISTICIAN', 'SCOREKEEPER', 'SCOREKEEPER_ASSISTANT', 'TIMEKEEPER', 'SCORER', 'SCORER_ASSISTANT', 'TIMER', 'GROUNDSKEEPER', 'CEO', 'COMMITTEE', 'PRESIDENT', 'DIRECTOR', 'PRESIDENT_VICE', 'SECRETARY', 'TREASURER', 'MANAGER', 'GENERAL', 'OTHER', 'REFEREE', 'UMPIRE', 'REFEREE_ASSISTANT', 'REFEREE_RESERVE', 'REFEREE_ASSISTANT_RESERVE', 'CREW_CHIEF', 'UMPIRE_RESERVE', 'UMPIRE_VIDEO', 'JUDGE_SCORING', 'JUDGE_TIMING', 'TECHNICAL_OFFICIAL', 'VIDEO_TECHNICIAN', 'TRANSLATOR', 'MEDIA_OFFICER', 'null')"
             )
         return value
 
     @validator("conduct_type")
     def conduct_type_validate_enum(cls, value):
         """Validates the enum"""
         for i in value:
@@ -221,36 +224,38 @@
 
     @validator("hearing_status")
     def hearing_status_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("PENDING", "FINALIZED"):
-            raise ValueError("must be one of enum values ('PENDING', 'FINALIZED')")
+        if value not in ("PENDING", "FINALIZED", "null"):
+            raise ValueError("must be one of enum values ('PENDING', 'FINALIZED', 'null')")
         return value
 
     @validator("fine_status")
     def fine_status_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("ISSUED", "PAID", "UNPAID", "CANCELLED", "OTHER"):
-            raise ValueError("must be one of enum values ('ISSUED', 'PAID', 'UNPAID', 'CANCELLED', 'OTHER')")
+        if value not in ("ISSUED", "PAID", "UNPAID", "CANCELLED", "OTHER", "null"):
+            raise ValueError("must be one of enum values ('ISSUED', 'PAID', 'UNPAID', 'CANCELLED', 'OTHER', 'null')")
         return value
 
     @validator("status")
     def status_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("ACTIVE", "INACTIVE", "PENDING", "COMPLETE", "CLOSED"):
-            raise ValueError("must be one of enum values ('ACTIVE', 'INACTIVE', 'PENDING', 'COMPLETE', 'CLOSED')")
+        if value not in ("ACTIVE", "INACTIVE", "PENDING", "COMPLETE", "CLOSED", "null"):
+            raise ValueError(
+                "must be one of enum values ('ACTIVE', 'INACTIVE', 'PENDING', 'COMPLETE', 'CLOSED', 'null')"
+            )
         return value
 
     @validator("external_id")
     def external_id_validate_regular_expression(cls, value):
         """Validates the regular expression"""
         if value is None:
             return value
@@ -324,14 +329,19 @@
             _dict["dateHearingLocal"] = None
 
         # set to None if hearing_notes (nullable) is None
         # and __fields_set__ contains the field
         if self.hearing_notes is None and "hearing_notes" in self.__fields_set__:
             _dict["hearingNotes"] = None
 
+        # set to None if hearing_status (nullable) is None
+        # and __fields_set__ contains the field
+        if self.hearing_status is None and "hearing_status" in self.__fields_set__:
+            _dict["hearingStatus"] = None
+
         # set to None if fine_currency (nullable) is None
         # and __fields_set__ contains the field
         if self.fine_currency is None and "fine_currency" in self.__fields_set__:
             _dict["fineCurrency"] = None
 
         # set to None if fine_status (nullable) is None
         # and __fields_set__ contains the field
```

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conduct_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/conduct_put_body.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,53 +53,55 @@
         None, description="The section of the period (sub-period)"
     )
     fixture_clock: Optional[constr(strict=True, max_length=20)] = Field(
         None, alias="fixtureClock", description="Fixture clock when the incident occurred"
     )
     role: Optional[constr(strict=True, max_length=100)] = Field(
         None,
-        description="The role of person >- `CAPTAIN` Captain >- `CAPTAIN_VICE` Vice Captain >- `CEO` CEO >- `COACH` Coach >- `COACH_ASSISTANT` Assistant Coach >- `COACH_ASSISTANT_HEAD` Assistant Head Coach >- `COACH_ASSOCIATE_HEAD` Associate Head Coach >- `COACH_DEVELOPMENT` Development Coach >- `COACH_HEAD` Head Coach >- `COACH_HEAD_INTERIM` Interim Head Coach >- `COACH_OTHER` Other coaching staff >- `COACH_SC` Strengh and Conditioning Coach >- `COACH_SENIOR` Senior Coach >- `COACH_SPECIALIST` Specialist Coach >- `COMMISSIONER` Commissioner >- `COMMITTEE` Committee >- `CREW_CHIEF` Crew Chief >- `DIRECTOR` Director >- `DOCTOR` Doctor >- `GENERAL` General >- `GROUNDSKEEPER` Groundskeeper >- `JUDGE_SCORING` Scoring Judge (SJ) >- `JUDGE_TIMING` Timing Judge (TJ) >- `MANAGER` Manager >- `MATCH_OFFICIAL` Match Official >- `MEDIA_OFFICER` Media Officer >- `MEDICAL_STAFF` Medical Staff >- `OTHER` Other >- `PHYSIOTHERAPIST` Physiotherapist >- `PRESIDENT` President >- `PRESIDENT_VICE` Vice President >- `REFEREE` Referee >- `REFEREE_ASSISTANT` Referee Assistant >- `REFEREE_ASSISTANT_RESERVE` Reserve Assistant Referee >- `REFEREE_RESERVE` Reserve Referee >- `SCOREKEEPER` Scorekeeper >- `SCOREKEEPER_ASSISTANT` Assistant Scorekeeper >- `SCORER` Scorer >- `SCORER_ASSISTANT` Assistant Scorer >- `SECRETARY` Secretary >- `STATISTICIAN` Statistician >- `TECHNICAL_OFFICIAL` Technical Official (TO) >- `TIMEKEEPER` Timekeeper >- `TIMER` Timer >- `TRAINER` Trainer >- `TRAINER_ASSISTANT` Assitant Trainer >- `TRANSLATOR` Translator >- `TREASURER` Treasurer >- `UMPIRE` Umpire >- `UMPIRE_RESERVE` Reserve Umpire (RU) >- `UMPIRE_VIDEO` Video Umpire (VU) >- `VIDEO_TECHNICIAN` Video Technician (VT) ",
+        description="The role of person >- None None >- `CAPTAIN` Captain >- `CAPTAIN_VICE` Vice Captain >- `CEO` CEO >- `COACH` Coach >- `COACH_ASSISTANT` Assistant Coach >- `COACH_ASSISTANT_HEAD` Assistant Head Coach >- `COACH_ASSOCIATE_HEAD` Associate Head Coach >- `COACH_DEVELOPMENT` Development Coach >- `COACH_HEAD` Head Coach >- `COACH_HEAD_INTERIM` Interim Head Coach >- `COACH_OTHER` Other coaching staff >- `COACH_SC` Strengh and Conditioning Coach >- `COACH_SENIOR` Senior Coach >- `COACH_SPECIALIST` Specialist Coach >- `COMMISSIONER` Commissioner >- `COMMITTEE` Committee >- `CREW_CHIEF` Crew Chief >- `DIRECTOR` Director >- `DOCTOR` Doctor >- `GENERAL` General >- `GROUNDSKEEPER` Groundskeeper >- `JUDGE_SCORING` Scoring Judge (SJ) >- `JUDGE_TIMING` Timing Judge (TJ) >- `MANAGER` Manager >- `MATCH_OFFICIAL` Match Official >- `MEDIA_OFFICER` Media Officer >- `MEDICAL_STAFF` Medical Staff >- `OTHER` Other >- `PHYSIOTHERAPIST` Physiotherapist >- `PRESIDENT` President >- `PRESIDENT_VICE` Vice President >- `REFEREE` Referee >- `REFEREE_ASSISTANT` Referee Assistant >- `REFEREE_ASSISTANT_RESERVE` Reserve Assistant Referee >- `REFEREE_RESERVE` Reserve Referee >- `SCOREKEEPER` Scorekeeper >- `SCOREKEEPER_ASSISTANT` Assistant Scorekeeper >- `SCORER` Scorer >- `SCORER_ASSISTANT` Assistant Scorer >- `SECRETARY` Secretary >- `STATISTICIAN` Statistician >- `TECHNICAL_OFFICIAL` Technical Official (TO) >- `TIMEKEEPER` Timekeeper >- `TIMER` Timer >- `TRAINER` Trainer >- `TRAINER_ASSISTANT` Assitant Trainer >- `TRANSLATOR` Translator >- `TREASURER` Treasurer >- `UMPIRE` Umpire >- `UMPIRE_RESERVE` Reserve Umpire (RU) >- `UMPIRE_VIDEO` Video Umpire (VU) >- `VIDEO_TECHNICIAN` Video Technician (VT) ",
     )
     date_offence_local: Optional[datetime] = Field(
         None, alias="dateOffenceLocal", description="Date & Time of the Offence in the local timezone"
     )
     conduct_type: Optional[conlist(StrictStr, min_items=1)] = Field(None, alias="conductType")
     conduct_notes: Optional[constr(strict=True, max_length=2000)] = Field(
         None, alias="conductNotes", description="Notes of the Conduct incident"
     )
     date_hearing_local: Optional[date] = Field(None, alias="dateHearingLocal", description="Date hearing")
     hearing_notes: Optional[constr(strict=True, max_length=500)] = Field(
         None, alias="hearingNotes", description="Notes from the conduct hearing"
     )
     hearing_status: Optional[StrictStr] = Field(
-        None, alias="hearingStatus", description="Conduct hearing status >- `FINALIZED` Finalized >- `PENDING` Pending "
+        None,
+        alias="hearingStatus",
+        description="Conduct hearing status >- None None >- `FINALIZED` Finalized >- `PENDING` Pending ",
     )
     life_sentence: Optional[StrictBool] = Field(
         None, alias="lifeSentence", description="Was the result of the conduct hearing a life sentence?"
     )
     penalty_results: Optional[conlist(ConductPenaltyResult)] = Field(None, alias="penaltyResults")
     fine_amount: Optional[Union[StrictFloat, StrictInt]] = Field(
         None, alias="fineAmount", description="Conduct fine amount"
     )
     fine_currency: Optional[constr(strict=True, max_length=20)] = Field(
         None, alias="fineCurrency", description="Fine currency"
     )
     fine_status: Optional[StrictStr] = Field(
         None,
         alias="fineStatus",
-        description="Conduct fine due status >- `CANCELLED` Cancelled >- `ISSUED` Issued >- `OTHER` Other >- `PAID` Paid >- `UNPAID` Unpaid ",
+        description="Conduct fine due status >- None None >- `CANCELLED` Cancelled >- `ISSUED` Issued >- `OTHER` Other >- `PAID` Paid >- `UNPAID` Unpaid ",
     )
     date_suspended_to: Optional[date] = Field(None, alias="dateSuspendedTo", description="Date the suspension ended")
     date_suspended_from: Optional[date] = Field(
         None, alias="dateSuspendedFrom", description="Date the suspension started"
     )
     date_fine_paid_local: Optional[date] = Field(None, alias="dateFinePaidLocal", description="Date the fine was paid")
     status: Optional[constr(strict=True, max_length=30)] = Field(
         None,
-        description="Conduct status >- `ACTIVE` Active >- `CLOSED` Closed >- `COMPLETE` Complete >- `INACTIVE` Inactive >- `PENDING` Pending ",
+        description="Conduct status >- None None >- `ACTIVE` Active >- `CLOSED` Closed >- `COMPLETE` Complete >- `INACTIVE` Inactive >- `PENDING` Pending ",
     )
     external_id: Optional[constr(strict=True, max_length=150)] = Field(
         None, alias="externalId", description="The Id of the data as set by the provider of the data"
     )
     __properties = [
         "personId",
         "entityGroupId",
@@ -188,17 +190,18 @@
             "UMPIRE_VIDEO",
             "JUDGE_SCORING",
             "JUDGE_TIMING",
             "TECHNICAL_OFFICIAL",
             "VIDEO_TECHNICIAN",
             "TRANSLATOR",
             "MEDIA_OFFICER",
+            "null",
         ):
             raise ValueError(
-                "must be one of enum values ('COACH', 'COACH_HEAD', 'COACH_HEAD_INTERIM', 'COACH_ASSISTANT', 'COACH_ASSISTANT_HEAD', 'COACH_ASSOCIATE_HEAD', 'COACH_SC', 'COACH_SENIOR', 'COACH_DEVELOPMENT', 'COACH_SPECIALIST', 'COACH_OTHER', 'CAPTAIN', 'CAPTAIN_VICE', 'DOCTOR', 'PHYSIOTHERAPIST', 'MEDICAL_STAFF', 'TRAINER', 'TRAINER_ASSISTANT', 'MATCH_OFFICIAL', 'COMMISSIONER', 'STATISTICIAN', 'SCOREKEEPER', 'SCOREKEEPER_ASSISTANT', 'TIMEKEEPER', 'SCORER', 'SCORER_ASSISTANT', 'TIMER', 'GROUNDSKEEPER', 'CEO', 'COMMITTEE', 'PRESIDENT', 'DIRECTOR', 'PRESIDENT_VICE', 'SECRETARY', 'TREASURER', 'MANAGER', 'GENERAL', 'OTHER', 'REFEREE', 'UMPIRE', 'REFEREE_ASSISTANT', 'REFEREE_RESERVE', 'REFEREE_ASSISTANT_RESERVE', 'CREW_CHIEF', 'UMPIRE_RESERVE', 'UMPIRE_VIDEO', 'JUDGE_SCORING', 'JUDGE_TIMING', 'TECHNICAL_OFFICIAL', 'VIDEO_TECHNICIAN', 'TRANSLATOR', 'MEDIA_OFFICER')"
+                "must be one of enum values ('COACH', 'COACH_HEAD', 'COACH_HEAD_INTERIM', 'COACH_ASSISTANT', 'COACH_ASSISTANT_HEAD', 'COACH_ASSOCIATE_HEAD', 'COACH_SC', 'COACH_SENIOR', 'COACH_DEVELOPMENT', 'COACH_SPECIALIST', 'COACH_OTHER', 'CAPTAIN', 'CAPTAIN_VICE', 'DOCTOR', 'PHYSIOTHERAPIST', 'MEDICAL_STAFF', 'TRAINER', 'TRAINER_ASSISTANT', 'MATCH_OFFICIAL', 'COMMISSIONER', 'STATISTICIAN', 'SCOREKEEPER', 'SCOREKEEPER_ASSISTANT', 'TIMEKEEPER', 'SCORER', 'SCORER_ASSISTANT', 'TIMER', 'GROUNDSKEEPER', 'CEO', 'COMMITTEE', 'PRESIDENT', 'DIRECTOR', 'PRESIDENT_VICE', 'SECRETARY', 'TREASURER', 'MANAGER', 'GENERAL', 'OTHER', 'REFEREE', 'UMPIRE', 'REFEREE_ASSISTANT', 'REFEREE_RESERVE', 'REFEREE_ASSISTANT_RESERVE', 'CREW_CHIEF', 'UMPIRE_RESERVE', 'UMPIRE_VIDEO', 'JUDGE_SCORING', 'JUDGE_TIMING', 'TECHNICAL_OFFICIAL', 'VIDEO_TECHNICIAN', 'TRANSLATOR', 'MEDIA_OFFICER', 'null')"
             )
         return value
 
     @validator("conduct_type")
     def conduct_type_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
@@ -222,36 +225,38 @@
 
     @validator("hearing_status")
     def hearing_status_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("PENDING", "FINALIZED"):
-            raise ValueError("must be one of enum values ('PENDING', 'FINALIZED')")
+        if value not in ("PENDING", "FINALIZED", "null"):
+            raise ValueError("must be one of enum values ('PENDING', 'FINALIZED', 'null')")
         return value
 
     @validator("fine_status")
     def fine_status_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("ISSUED", "PAID", "UNPAID", "CANCELLED", "OTHER"):
-            raise ValueError("must be one of enum values ('ISSUED', 'PAID', 'UNPAID', 'CANCELLED', 'OTHER')")
+        if value not in ("ISSUED", "PAID", "UNPAID", "CANCELLED", "OTHER", "null"):
+            raise ValueError("must be one of enum values ('ISSUED', 'PAID', 'UNPAID', 'CANCELLED', 'OTHER', 'null')")
         return value
 
     @validator("status")
     def status_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("ACTIVE", "INACTIVE", "PENDING", "COMPLETE", "CLOSED"):
-            raise ValueError("must be one of enum values ('ACTIVE', 'INACTIVE', 'PENDING', 'COMPLETE', 'CLOSED')")
+        if value not in ("ACTIVE", "INACTIVE", "PENDING", "COMPLETE", "CLOSED", "null"):
+            raise ValueError(
+                "must be one of enum values ('ACTIVE', 'INACTIVE', 'PENDING', 'COMPLETE', 'CLOSED', 'null')"
+            )
         return value
 
     @validator("external_id")
     def external_id_validate_regular_expression(cls, value):
         """Validates the regular expression"""
         if value is None:
             return value
@@ -325,14 +330,19 @@
             _dict["dateHearingLocal"] = None
 
         # set to None if hearing_notes (nullable) is None
         # and __fields_set__ contains the field
         if self.hearing_notes is None and "hearing_notes" in self.__fields_set__:
             _dict["hearingNotes"] = None
 
+        # set to None if hearing_status (nullable) is None
+        # and __fields_set__ contains the field
+        if self.hearing_status is None and "hearing_status" in self.__fields_set__:
+            _dict["hearingStatus"] = None
+
         # set to None if fine_currency (nullable) is None
         # and __fields_set__ contains the field
         if self.fine_currency is None and "fine_currency" in self.__fields_set__:
             _dict["fineCurrency"] = None
 
         # set to None if fine_status (nullable) is None
         # and __fields_set__ contains the field
```

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conduct_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/conduct_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conference_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/conference_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conference_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/conference_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conferences_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/conferences_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conferences_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/conferences_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/conferences_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/conferences_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/contact_details.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/contact_details.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/division_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/division_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/division_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/division_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/divisions_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/divisions_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/divisions_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/divisions_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/divisions_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/divisions_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entities_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entities_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,23 +87,23 @@
     )
     external_id: Optional[constr(strict=True, max_length=150)] = Field(
         None, alias="externalId", description="The Id of the data as set by the provider of the data"
     )
     age_group: Optional[constr(strict=True, max_length=50)] = Field(
         None,
         alias="ageGroup",
-        description="The age group of the entity >- `JUNIOR` Junior >- `MASTERS` Masters >- `SENIOR` Senior >- `UNDER_10` Under 10 >- `UNDER_11` Under 11 >- `UNDER_12` Under 12 >- `UNDER_13` Under 13 >- `UNDER_14` Under 14 >- `UNDER_15` Under 15 >- `UNDER_16` Under 16 >- `UNDER_17` Under 17 >- `UNDER_18` Under 18 >- `UNDER_19` Under 19 >- `UNDER_20` Under 20 >- `UNDER_21` Under 21 >- `UNDER_22` Under 22 >- `UNDER_23` Under 23 >- `YOUTH` Youth ",
+        description="The age group of the entity >- None None >- `JUNIOR` Junior >- `MASTERS` Masters >- `SENIOR` Senior >- `UNDER_10` Under 10 >- `UNDER_11` Under 11 >- `UNDER_12` Under 12 >- `UNDER_13` Under 13 >- `UNDER_14` Under 14 >- `UNDER_15` Under 15 >- `UNDER_16` Under 16 >- `UNDER_17` Under 17 >- `UNDER_18` Under 18 >- `UNDER_19` Under 19 >- `UNDER_20` Under 20 >- `UNDER_21` Under 21 >- `UNDER_22` Under 22 >- `UNDER_23` Under 23 >- `YOUTH` Youth ",
     )
     gender: Optional[constr(strict=True, max_length=20)] = Field(
         None,
-        description="The gender of the participants in the entity >- `FEMALE` Female >- `MALE` Male >- `MIXED` Mixed >- `UNKNOWN` Unknown ",
+        description="The gender of the participants in the entity >- None None >- `FEMALE` Female >- `MALE` Male >- `MIXED` Mixed >- `UNKNOWN` Unknown ",
     )
     standard: Optional[constr(strict=True, max_length=50)] = Field(
         None,
-        description="The playing standard of the entity >- `ELITE` Professional/elite organisation >- `FRIENDLY` International Friendly >- `GRASS_ROOT` Normal >- `INTERNATIONAL` International >- `NONCONTINENTAL_CHAMPIONSHIP` Non-continental Championship >- `OLYMPIC` Olympics >- `REGION` Regional >- `TIER2` lesser standard than elite >- `TIER3` lesser standard than tier 2 >- `WORLD_CHAMPIONSHIP` World Championship >- `ZONE_CHAMPIONSHIP` International Zone Championship ",
+        description="The playing standard of the entity >- None None >- `ELITE` Professional/elite organisation >- `FRIENDLY` International Friendly >- `GRASS_ROOT` Normal >- `INTERNATIONAL` International >- `NONCONTINENTAL_CHAMPIONSHIP` Non-continental Championship >- `OLYMPIC` Olympics >- `REGION` Regional >- `TIER2` lesser standard than elite >- `TIER3` lesser standard than tier 2 >- `WORLD_CHAMPIONSHIP` World Championship >- `ZONE_CHAMPIONSHIP` International Zone Championship ",
     )
     grade: Optional[constr(strict=True, max_length=50)] = Field(
         None, description="The playing grade of the fixtures for this entity"
     )
     updated: Optional[datetime] = Field(None, description="Date/time last modified. In UTC")
     added: Optional[datetime] = Field(None, description="Date/time added. In UTC")
     default_venue_id: Optional[StrictStr] = Field(
@@ -181,28 +181,29 @@
             "UNDER_19",
             "UNDER_20",
             "UNDER_21",
             "UNDER_22",
             "UNDER_23",
             "SENIOR",
             "MASTERS",
+            "null",
         ):
             raise ValueError(
-                "must be one of enum values ('JUNIOR', 'YOUTH', 'UNDER_10', 'UNDER_11', 'UNDER_12', 'UNDER_13', 'UNDER_14', 'UNDER_15', 'UNDER_16', 'UNDER_17', 'UNDER_18', 'UNDER_19', 'UNDER_20', 'UNDER_21', 'UNDER_22', 'UNDER_23', 'SENIOR', 'MASTERS')"
+                "must be one of enum values ('JUNIOR', 'YOUTH', 'UNDER_10', 'UNDER_11', 'UNDER_12', 'UNDER_13', 'UNDER_14', 'UNDER_15', 'UNDER_16', 'UNDER_17', 'UNDER_18', 'UNDER_19', 'UNDER_20', 'UNDER_21', 'UNDER_22', 'UNDER_23', 'SENIOR', 'MASTERS', 'null')"
             )
         return value
 
     @validator("gender")
     def gender_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("FEMALE", "MALE", "MIXED", "UNKNOWN"):
-            raise ValueError("must be one of enum values ('FEMALE', 'MALE', 'MIXED', 'UNKNOWN')")
+        if value not in ("FEMALE", "MALE", "MIXED", "UNKNOWN", "null"):
+            raise ValueError("must be one of enum values ('FEMALE', 'MALE', 'MIXED', 'UNKNOWN', 'null')")
         return value
 
     @validator("standard")
     def standard_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
@@ -215,17 +216,18 @@
             "NONCONTINENTAL_CHAMPIONSHIP",
             "OLYMPIC",
             "REGION",
             "TIER2",
             "TIER3",
             "WORLD_CHAMPIONSHIP",
             "ZONE_CHAMPIONSHIP",
+            "null",
         ):
             raise ValueError(
-                "must be one of enum values ('ELITE', 'FRIENDLY', 'GRASS_ROOT', 'INTERNATIONAL', 'NONCONTINENTAL_CHAMPIONSHIP', 'OLYMPIC', 'REGION', 'TIER2', 'TIER3', 'WORLD_CHAMPIONSHIP', 'ZONE_CHAMPIONSHIP')"
+                "must be one of enum values ('ELITE', 'FRIENDLY', 'GRASS_ROOT', 'INTERNATIONAL', 'NONCONTINENTAL_CHAMPIONSHIP', 'OLYMPIC', 'REGION', 'TIER2', 'TIER3', 'WORLD_CHAMPIONSHIP', 'ZONE_CHAMPIONSHIP', 'null')"
             )
         return value
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
@@ -344,14 +346,29 @@
             _dict["historicalNames"] = None
 
         # set to None if external_id (nullable) is None
         # and __fields_set__ contains the field
         if self.external_id is None and "external_id" in self.__fields_set__:
             _dict["externalId"] = None
 
+        # set to None if age_group (nullable) is None
+        # and __fields_set__ contains the field
+        if self.age_group is None and "age_group" in self.__fields_set__:
+            _dict["ageGroup"] = None
+
+        # set to None if gender (nullable) is None
+        # and __fields_set__ contains the field
+        if self.gender is None and "gender" in self.__fields_set__:
+            _dict["gender"] = None
+
+        # set to None if standard (nullable) is None
+        # and __fields_set__ contains the field
+        if self.standard is None and "standard" in self.__fields_set__:
+            _dict["standard"] = None
+
         # set to None if grade (nullable) is None
         # and __fields_set__ contains the field
         if self.grade is None and "grade" in self.__fields_set__:
             _dict["grade"] = None
 
         # set to None if default_venue_id (nullable) is None
         # and __fields_set__ contains the field
```

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entities_model_entity_group.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entities_model_entity_group.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entities_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entities_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entities_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entities_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_additional_details.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_additional_details.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_address.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_address.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_group_address.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_group_address.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_group_historical_name.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_group_historical_name.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_group_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_group_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_group_post_body_additional_names.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_group_post_body_additional_names.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_group_post_body_colors.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_group_post_body_colors.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_group_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_group_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_groups_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_groups_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_groups_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_groups_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_groups_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_groups_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_historical_name.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_historical_name.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_post_body.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,23 +78,23 @@
     )
     external_id: Optional[constr(strict=True, max_length=150)] = Field(
         None, alias="externalId", description="The Id of the data as set by the provider of the data"
     )
     age_group: Optional[constr(strict=True, max_length=50)] = Field(
         None,
         alias="ageGroup",
-        description="The age group of the entity >- `JUNIOR` Junior >- `MASTERS` Masters >- `SENIOR` Senior >- `UNDER_10` Under 10 >- `UNDER_11` Under 11 >- `UNDER_12` Under 12 >- `UNDER_13` Under 13 >- `UNDER_14` Under 14 >- `UNDER_15` Under 15 >- `UNDER_16` Under 16 >- `UNDER_17` Under 17 >- `UNDER_18` Under 18 >- `UNDER_19` Under 19 >- `UNDER_20` Under 20 >- `UNDER_21` Under 21 >- `UNDER_22` Under 22 >- `UNDER_23` Under 23 >- `YOUTH` Youth ",
+        description="The age group of the entity >- None None >- `JUNIOR` Junior >- `MASTERS` Masters >- `SENIOR` Senior >- `UNDER_10` Under 10 >- `UNDER_11` Under 11 >- `UNDER_12` Under 12 >- `UNDER_13` Under 13 >- `UNDER_14` Under 14 >- `UNDER_15` Under 15 >- `UNDER_16` Under 16 >- `UNDER_17` Under 17 >- `UNDER_18` Under 18 >- `UNDER_19` Under 19 >- `UNDER_20` Under 20 >- `UNDER_21` Under 21 >- `UNDER_22` Under 22 >- `UNDER_23` Under 23 >- `YOUTH` Youth ",
     )
     gender: Optional[constr(strict=True, max_length=20)] = Field(
         None,
-        description="The gender of the participants in the entity >- `FEMALE` Female >- `MALE` Male >- `MIXED` Mixed >- `UNKNOWN` Unknown ",
+        description="The gender of the participants in the entity >- None None >- `FEMALE` Female >- `MALE` Male >- `MIXED` Mixed >- `UNKNOWN` Unknown ",
     )
     standard: Optional[constr(strict=True, max_length=50)] = Field(
         None,
-        description="The playing standard of the entity >- `ELITE` Professional/elite organisation >- `FRIENDLY` International Friendly >- `GRASS_ROOT` Normal >- `INTERNATIONAL` International >- `NONCONTINENTAL_CHAMPIONSHIP` Non-continental Championship >- `OLYMPIC` Olympics >- `REGION` Regional >- `TIER2` lesser standard than elite >- `TIER3` lesser standard than tier 2 >- `WORLD_CHAMPIONSHIP` World Championship >- `ZONE_CHAMPIONSHIP` International Zone Championship ",
+        description="The playing standard of the entity >- None None >- `ELITE` Professional/elite organisation >- `FRIENDLY` International Friendly >- `GRASS_ROOT` Normal >- `INTERNATIONAL` International >- `NONCONTINENTAL_CHAMPIONSHIP` Non-continental Championship >- `OLYMPIC` Olympics >- `REGION` Regional >- `TIER2` lesser standard than elite >- `TIER3` lesser standard than tier 2 >- `WORLD_CHAMPIONSHIP` World Championship >- `ZONE_CHAMPIONSHIP` International Zone Championship ",
     )
     grade: Optional[constr(strict=True, max_length=50)] = Field(
         None, description="The playing grade of the fixtures for this entity"
     )
     default_venue_id: Optional[StrictStr] = Field(
         None, alias="defaultVenueId", description="The unique identifier of the default venue"
     )
@@ -160,28 +160,29 @@
             "UNDER_19",
             "UNDER_20",
             "UNDER_21",
             "UNDER_22",
             "UNDER_23",
             "SENIOR",
             "MASTERS",
+            "null",
         ):
             raise ValueError(
-                "must be one of enum values ('JUNIOR', 'YOUTH', 'UNDER_10', 'UNDER_11', 'UNDER_12', 'UNDER_13', 'UNDER_14', 'UNDER_15', 'UNDER_16', 'UNDER_17', 'UNDER_18', 'UNDER_19', 'UNDER_20', 'UNDER_21', 'UNDER_22', 'UNDER_23', 'SENIOR', 'MASTERS')"
+                "must be one of enum values ('JUNIOR', 'YOUTH', 'UNDER_10', 'UNDER_11', 'UNDER_12', 'UNDER_13', 'UNDER_14', 'UNDER_15', 'UNDER_16', 'UNDER_17', 'UNDER_18', 'UNDER_19', 'UNDER_20', 'UNDER_21', 'UNDER_22', 'UNDER_23', 'SENIOR', 'MASTERS', 'null')"
             )
         return value
 
     @validator("gender")
     def gender_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("FEMALE", "MALE", "MIXED", "UNKNOWN"):
-            raise ValueError("must be one of enum values ('FEMALE', 'MALE', 'MIXED', 'UNKNOWN')")
+        if value not in ("FEMALE", "MALE", "MIXED", "UNKNOWN", "null"):
+            raise ValueError("must be one of enum values ('FEMALE', 'MALE', 'MIXED', 'UNKNOWN', 'null')")
         return value
 
     @validator("standard")
     def standard_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
@@ -194,17 +195,18 @@
             "NONCONTINENTAL_CHAMPIONSHIP",
             "OLYMPIC",
             "REGION",
             "TIER2",
             "TIER3",
             "WORLD_CHAMPIONSHIP",
             "ZONE_CHAMPIONSHIP",
+            "null",
         ):
             raise ValueError(
-                "must be one of enum values ('ELITE', 'FRIENDLY', 'GRASS_ROOT', 'INTERNATIONAL', 'NONCONTINENTAL_CHAMPIONSHIP', 'OLYMPIC', 'REGION', 'TIER2', 'TIER3', 'WORLD_CHAMPIONSHIP', 'ZONE_CHAMPIONSHIP')"
+                "must be one of enum values ('ELITE', 'FRIENDLY', 'GRASS_ROOT', 'INTERNATIONAL', 'NONCONTINENTAL_CHAMPIONSHIP', 'OLYMPIC', 'REGION', 'TIER2', 'TIER3', 'WORLD_CHAMPIONSHIP', 'ZONE_CHAMPIONSHIP', 'null')"
             )
         return value
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
@@ -302,14 +304,29 @@
             _dict["historicalNames"] = None
 
         # set to None if external_id (nullable) is None
         # and __fields_set__ contains the field
         if self.external_id is None and "external_id" in self.__fields_set__:
             _dict["externalId"] = None
 
+        # set to None if age_group (nullable) is None
+        # and __fields_set__ contains the field
+        if self.age_group is None and "age_group" in self.__fields_set__:
+            _dict["ageGroup"] = None
+
+        # set to None if gender (nullable) is None
+        # and __fields_set__ contains the field
+        if self.gender is None and "gender" in self.__fields_set__:
+            _dict["gender"] = None
+
+        # set to None if standard (nullable) is None
+        # and __fields_set__ contains the field
+        if self.standard is None and "standard" in self.__fields_set__:
+            _dict["standard"] = None
+
         # set to None if grade (nullable) is None
         # and __fields_set__ contains the field
         if self.grade is None and "grade" in self.__fields_set__:
             _dict["grade"] = None
 
         # set to None if default_venue_id (nullable) is None
         # and __fields_set__ contains the field
```

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_post_body_additional_names.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_post_body_additional_names.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_post_body_colors.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_post_body_colors.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/entity_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/entity_put_body.py`

 * *Files 8% similar despite different names*

```diff
@@ -77,23 +77,23 @@
     )
     external_id: Optional[constr(strict=True, max_length=150)] = Field(
         None, alias="externalId", description="The Id of the data as set by the provider of the data"
     )
     age_group: Optional[constr(strict=True, max_length=50)] = Field(
         None,
         alias="ageGroup",
-        description="The age group of the entity >- `JUNIOR` Junior >- `MASTERS` Masters >- `SENIOR` Senior >- `UNDER_10` Under 10 >- `UNDER_11` Under 11 >- `UNDER_12` Under 12 >- `UNDER_13` Under 13 >- `UNDER_14` Under 14 >- `UNDER_15` Under 15 >- `UNDER_16` Under 16 >- `UNDER_17` Under 17 >- `UNDER_18` Under 18 >- `UNDER_19` Under 19 >- `UNDER_20` Under 20 >- `UNDER_21` Under 21 >- `UNDER_22` Under 22 >- `UNDER_23` Under 23 >- `YOUTH` Youth ",
+        description="The age group of the entity >- None None >- `JUNIOR` Junior >- `MASTERS` Masters >- `SENIOR` Senior >- `UNDER_10` Under 10 >- `UNDER_11` Under 11 >- `UNDER_12` Under 12 >- `UNDER_13` Under 13 >- `UNDER_14` Under 14 >- `UNDER_15` Under 15 >- `UNDER_16` Under 16 >- `UNDER_17` Under 17 >- `UNDER_18` Under 18 >- `UNDER_19` Under 19 >- `UNDER_20` Under 20 >- `UNDER_21` Under 21 >- `UNDER_22` Under 22 >- `UNDER_23` Under 23 >- `YOUTH` Youth ",
     )
     gender: Optional[constr(strict=True, max_length=20)] = Field(
         None,
-        description="The gender of the participants in the entity >- `FEMALE` Female >- `MALE` Male >- `MIXED` Mixed >- `UNKNOWN` Unknown ",
+        description="The gender of the participants in the entity >- None None >- `FEMALE` Female >- `MALE` Male >- `MIXED` Mixed >- `UNKNOWN` Unknown ",
     )
     standard: Optional[constr(strict=True, max_length=50)] = Field(
         None,
-        description="The playing standard of the entity >- `ELITE` Professional/elite organisation >- `FRIENDLY` International Friendly >- `GRASS_ROOT` Normal >- `INTERNATIONAL` International >- `NONCONTINENTAL_CHAMPIONSHIP` Non-continental Championship >- `OLYMPIC` Olympics >- `REGION` Regional >- `TIER2` lesser standard than elite >- `TIER3` lesser standard than tier 2 >- `WORLD_CHAMPIONSHIP` World Championship >- `ZONE_CHAMPIONSHIP` International Zone Championship ",
+        description="The playing standard of the entity >- None None >- `ELITE` Professional/elite organisation >- `FRIENDLY` International Friendly >- `GRASS_ROOT` Normal >- `INTERNATIONAL` International >- `NONCONTINENTAL_CHAMPIONSHIP` Non-continental Championship >- `OLYMPIC` Olympics >- `REGION` Regional >- `TIER2` lesser standard than elite >- `TIER3` lesser standard than tier 2 >- `WORLD_CHAMPIONSHIP` World Championship >- `ZONE_CHAMPIONSHIP` International Zone Championship ",
     )
     grade: Optional[constr(strict=True, max_length=50)] = Field(
         None, description="The playing grade of the fixtures for this entity"
     )
     default_venue_id: Optional[StrictStr] = Field(
         None, alias="defaultVenueId", description="The unique identifier of the default venue"
     )
@@ -161,28 +161,29 @@
             "UNDER_19",
             "UNDER_20",
             "UNDER_21",
             "UNDER_22",
             "UNDER_23",
             "SENIOR",
             "MASTERS",
+            "null",
         ):
             raise ValueError(
-                "must be one of enum values ('JUNIOR', 'YOUTH', 'UNDER_10', 'UNDER_11', 'UNDER_12', 'UNDER_13', 'UNDER_14', 'UNDER_15', 'UNDER_16', 'UNDER_17', 'UNDER_18', 'UNDER_19', 'UNDER_20', 'UNDER_21', 'UNDER_22', 'UNDER_23', 'SENIOR', 'MASTERS')"
+                "must be one of enum values ('JUNIOR', 'YOUTH', 'UNDER_10', 'UNDER_11', 'UNDER_12', 'UNDER_13', 'UNDER_14', 'UNDER_15', 'UNDER_16', 'UNDER_17', 'UNDER_18', 'UNDER_19', 'UNDER_20', 'UNDER_21', 'UNDER_22', 'UNDER_23', 'SENIOR', 'MASTERS', 'null')"
             )
         return value
 
     @validator("gender")
     def gender_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("FEMALE", "MALE", "MIXED", "UNKNOWN"):
-            raise ValueError("must be one of enum values ('FEMALE', 'MALE', 'MIXED', 'UNKNOWN')")
+        if value not in ("FEMALE", "MALE", "MIXED", "UNKNOWN", "null"):
+            raise ValueError("must be one of enum values ('FEMALE', 'MALE', 'MIXED', 'UNKNOWN', 'null')")
         return value
 
     @validator("standard")
     def standard_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
@@ -195,17 +196,18 @@
             "NONCONTINENTAL_CHAMPIONSHIP",
             "OLYMPIC",
             "REGION",
             "TIER2",
             "TIER3",
             "WORLD_CHAMPIONSHIP",
             "ZONE_CHAMPIONSHIP",
+            "null",
         ):
             raise ValueError(
-                "must be one of enum values ('ELITE', 'FRIENDLY', 'GRASS_ROOT', 'INTERNATIONAL', 'NONCONTINENTAL_CHAMPIONSHIP', 'OLYMPIC', 'REGION', 'TIER2', 'TIER3', 'WORLD_CHAMPIONSHIP', 'ZONE_CHAMPIONSHIP')"
+                "must be one of enum values ('ELITE', 'FRIENDLY', 'GRASS_ROOT', 'INTERNATIONAL', 'NONCONTINENTAL_CHAMPIONSHIP', 'OLYMPIC', 'REGION', 'TIER2', 'TIER3', 'WORLD_CHAMPIONSHIP', 'ZONE_CHAMPIONSHIP', 'null')"
             )
         return value
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
@@ -303,14 +305,29 @@
             _dict["historicalNames"] = None
 
         # set to None if external_id (nullable) is None
         # and __fields_set__ contains the field
         if self.external_id is None and "external_id" in self.__fields_set__:
             _dict["externalId"] = None
 
+        # set to None if age_group (nullable) is None
+        # and __fields_set__ contains the field
+        if self.age_group is None and "age_group" in self.__fields_set__:
+            _dict["ageGroup"] = None
+
+        # set to None if gender (nullable) is None
+        # and __fields_set__ contains the field
+        if self.gender is None and "gender" in self.__fields_set__:
+            _dict["gender"] = None
+
+        # set to None if standard (nullable) is None
+        # and __fields_set__ contains the field
+        if self.standard is None and "standard" in self.__fields_set__:
+            _dict["standard"] = None
+
         # set to None if grade (nullable) is None
         # and __fields_set__ contains the field
         if self.grade is None and "grade" in self.__fields_set__:
             _dict["grade"] = None
 
         # set to None if default_venue_id (nullable) is None
         # and __fields_set__ contains the field
```

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/environmental_details.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/environmental_details.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/error_list_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/error_list_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/error_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/error_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_competitor.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_competitor.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entities_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_entities_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entities_model_conference.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_entities_model_conference.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entities_model_division.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_entities_model_division.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entities_model_entity.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_entities_model_entity.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entities_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_entities_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entities_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_entities_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entities_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_entities_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_period_statistics_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_entity_period_statistics_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_statistics_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_statistics_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_statistics_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_entity_statistics_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_live_summary_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_live_summary_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_live_summary_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_live_summary_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_participant.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_participant.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_pbp_event_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_pbp_event_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_pbp_event_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_pbp_event_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_pbp_event_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_pbp_event_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_pbp_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_pbp_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_pbp_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_pbp_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_pbp_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_pbp_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_pbp_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_pbp_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_person_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_person_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_person_statistics_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_person_statistics_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_person_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_persons_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_persons_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_persons_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_persons_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_persons_model_person.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_persons_model_person.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_persons_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_persons_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_persons_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_persons_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_post_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     """
 
     fixture_id: Optional[StrictStr] = Field(None, alias="fixtureId", description="The unique identifier of the fixture")
     season_id: StrictStr = Field(..., alias="seasonId", description="The unique identifier of the season")
     practice_drill_type: Optional[constr(strict=True, max_length=100)] = Field(
         None,
         alias="practiceDrillType",
-        description="Practice types >- `DRILL` Drill >- `FITNESS` Fitness >- `GAME` Practice Game >- `OTHER` Other ",
+        description="Practice types >- None None >- `DRILL` Drill >- `FITNESS` Fitness >- `GAME` Practice Game >- `OTHER` Other ",
     )
     international_reference: Optional[constr(strict=True, max_length=30)] = Field(
         None,
         alias="internationalReference",
         description="The international reference for this fixture given by the sport governing body",
     )
     status: Optional[constr(strict=True, max_length=100)] = Field(
@@ -103,15 +103,15 @@
         None,
         alias="fixtureType",
         description="Type of fixture >- `ALL_STAR` All Star >- `DEMONSTRATION` Demonstration >- `FINAL` Final >- `FRIENDLY` Friendly >- `PLAYOFF` Playoff >- `PRESEASON` Pre Season >- `REGULAR` Regular ",
     )
     maximum_period_type_used: Optional[constr(strict=True, max_length=50)] = Field(
         None,
         alias="maximumPeriodTypeUsed",
-        description="Maximum Period Type Used >- `EXTRA_TIME` Extra Time >- `OVERTIME` Overtime >- `REGULAR` Regular >- `SHOOTOUT` Shoot-Out ",
+        description="Maximum Period Type Used >- None None >- `EXTRA_TIME` Extra Time >- `OVERTIME` Overtime >- `REGULAR` Regular >- `SHOOTOUT` Shoot-Out ",
     )
     competitor_type: constr(strict=True, max_length=50) = Field(
         ...,
         alias="competitorType",
         description="The type of competitors in this fixture >- `ENTITY` Entity >- `PERSON` Person ",
     )
     participants: Optional[conlist(FixtureParticipant)] = Field(None, description="Array of fixture participants")
@@ -177,16 +177,16 @@
 
     @validator("practice_drill_type")
     def practice_drill_type_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("DRILL", "GAME", "FITNESS", "OTHER"):
-            raise ValueError("must be one of enum values ('DRILL', 'GAME', 'FITNESS', 'OTHER')")
+        if value not in ("DRILL", "GAME", "FITNESS", "OTHER", "null"):
+            raise ValueError("must be one of enum values ('DRILL', 'GAME', 'FITNESS', 'OTHER', 'null')")
         return value
 
     @validator("status")
     def status_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
@@ -222,16 +222,16 @@
 
     @validator("maximum_period_type_used")
     def maximum_period_type_used_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("REGULAR", "EXTRA_TIME", "OVERTIME", "SHOOTOUT"):
-            raise ValueError("must be one of enum values ('REGULAR', 'EXTRA_TIME', 'OVERTIME', 'SHOOTOUT')")
+        if value not in ("REGULAR", "EXTRA_TIME", "OVERTIME", "SHOOTOUT", "null"):
+            raise ValueError("must be one of enum values ('REGULAR', 'EXTRA_TIME', 'OVERTIME', 'SHOOTOUT', 'null')")
         return value
 
     @validator("competitor_type")
     def competitor_type_validate_enum(cls, value):
         """Validates the enum"""
         if value not in ("PERSON", "ENTITY"):
             raise ValueError("must be one of enum values ('PERSON', 'ENTITY')")
@@ -390,14 +390,19 @@
             _dict["roundCode"] = None
 
         # set to None if round_number (nullable) is None
         # and __fields_set__ contains the field
         if self.round_number is None and "round_number" in self.__fields_set__:
             _dict["roundNumber"] = None
 
+        # set to None if maximum_period_type_used (nullable) is None
+        # and __fields_set__ contains the field
+        if self.maximum_period_type_used is None and "maximum_period_type_used" in self.__fields_set__:
+            _dict["maximumPeriodTypeUsed"] = None
+
         # set to None if participants (nullable) is None
         # and __fields_set__ contains the field
         if self.participants is None and "participants" in self.__fields_set__:
             _dict["participants"] = None
 
         # set to None if competitors (nullable) is None
         # and __fields_set__ contains the field
```

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_profiles_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_profiles_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_profiles_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_profiles_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_profiles_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_profiles_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_profiles_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_profiles_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_profiles_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_profiles_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_progression_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_progression_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_progression_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_progression_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_progressions_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_progressions_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_progressions_model_fixture.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_progressions_model_fixture.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_progressions_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_progressions_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_progressions_model_season.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_progressions_model_season.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_progressions_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_progressions_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_put_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     FixturePutBody
     """
 
     season_id: Optional[StrictStr] = Field(None, alias="seasonId", description="The unique identifier of the season")
     practice_drill_type: Optional[constr(strict=True, max_length=100)] = Field(
         None,
         alias="practiceDrillType",
-        description="Practice types >- `DRILL` Drill >- `FITNESS` Fitness >- `GAME` Practice Game >- `OTHER` Other ",
+        description="Practice types >- None None >- `DRILL` Drill >- `FITNESS` Fitness >- `GAME` Practice Game >- `OTHER` Other ",
     )
     international_reference: Optional[constr(strict=True, max_length=30)] = Field(
         None,
         alias="internationalReference",
         description="The international reference for this fixture given by the sport governing body",
     )
     status: Optional[constr(strict=True, max_length=100)] = Field(
@@ -102,15 +102,15 @@
         None,
         alias="fixtureType",
         description="Type of fixture >- `ALL_STAR` All Star >- `DEMONSTRATION` Demonstration >- `FINAL` Final >- `FRIENDLY` Friendly >- `PLAYOFF` Playoff >- `PRESEASON` Pre Season >- `REGULAR` Regular ",
     )
     maximum_period_type_used: Optional[constr(strict=True, max_length=50)] = Field(
         None,
         alias="maximumPeriodTypeUsed",
-        description="Maximum Period Type Used >- `EXTRA_TIME` Extra Time >- `OVERTIME` Overtime >- `REGULAR` Regular >- `SHOOTOUT` Shoot-Out ",
+        description="Maximum Period Type Used >- None None >- `EXTRA_TIME` Extra Time >- `OVERTIME` Overtime >- `REGULAR` Regular >- `SHOOTOUT` Shoot-Out ",
     )
     competitor_type: Optional[constr(strict=True, max_length=50)] = Field(
         None,
         alias="competitorType",
         description="The type of competitors in this fixture >- `ENTITY` Entity >- `PERSON` Person ",
     )
     participants: Optional[conlist(FixtureParticipant)] = Field(None, description="Array of fixture participants")
@@ -175,16 +175,16 @@
 
     @validator("practice_drill_type")
     def practice_drill_type_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("DRILL", "GAME", "FITNESS", "OTHER"):
-            raise ValueError("must be one of enum values ('DRILL', 'GAME', 'FITNESS', 'OTHER')")
+        if value not in ("DRILL", "GAME", "FITNESS", "OTHER", "null"):
+            raise ValueError("must be one of enum values ('DRILL', 'GAME', 'FITNESS', 'OTHER', 'null')")
         return value
 
     @validator("status")
     def status_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
@@ -220,16 +220,16 @@
 
     @validator("maximum_period_type_used")
     def maximum_period_type_used_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("REGULAR", "EXTRA_TIME", "OVERTIME", "SHOOTOUT"):
-            raise ValueError("must be one of enum values ('REGULAR', 'EXTRA_TIME', 'OVERTIME', 'SHOOTOUT')")
+        if value not in ("REGULAR", "EXTRA_TIME", "OVERTIME", "SHOOTOUT", "null"):
+            raise ValueError("must be one of enum values ('REGULAR', 'EXTRA_TIME', 'OVERTIME', 'SHOOTOUT', 'null')")
         return value
 
     @validator("competitor_type")
     def competitor_type_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
@@ -391,14 +391,19 @@
             _dict["roundCode"] = None
 
         # set to None if round_number (nullable) is None
         # and __fields_set__ contains the field
         if self.round_number is None and "round_number" in self.__fields_set__:
             _dict["roundNumber"] = None
 
+        # set to None if maximum_period_type_used (nullable) is None
+        # and __fields_set__ contains the field
+        if self.maximum_period_type_used is None and "maximum_period_type_used" in self.__fields_set__:
+            _dict["maximumPeriodTypeUsed"] = None
+
         # set to None if participants (nullable) is None
         # and __fields_set__ contains the field
         if self.participants is None and "participants" in self.__fields_set__:
             _dict["participants"] = None
 
         # set to None if competitors (nullable) is None
         # and __fields_set__ contains the field
```

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_roster_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_roster_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_roster_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_roster_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_roster_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_roster_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_roster_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_roster_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixture_videosteam_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixture_videosteam_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_by_entity_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixtures_by_competition_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,30 +36,30 @@
 )
 from atriumsports.datacore.openapi.models.season_fixture_stages_pools_list_model_stage import (
     SeasonFixtureStagesPoolsListModelStage,
 )
 from atriumsports.datacore.openapi.models.social_media import SocialMedia
 
 
-class FixturesByEntityModel(BaseModel):
+class FixturesByCompetitionModel(BaseModel):
     """
-    FixturesByEntityModel
+    FixturesByCompetitionModel
     """
 
     fixture_id: Optional[StrictStr] = Field(None, alias="fixtureId", description="The unique identifier of the fixture")
     organization_id: Optional[StrictStr] = Field(
         None, alias="organizationId", description="The unique identifier of the organization"
     )
     organization: Optional[FixturesModelOrganization] = None
     season_id: Optional[StrictStr] = Field(None, alias="seasonId", description="The unique identifier of the season")
     season: Optional[FixtureProgressionsModelSeason] = None
     practice_drill_type: Optional[constr(strict=True, max_length=100)] = Field(
         None,
         alias="practiceDrillType",
-        description="Practice types >- `DRILL` Drill >- `FITNESS` Fitness >- `GAME` Practice Game >- `OTHER` Other ",
+        description="Practice types >- None None >- `DRILL` Drill >- `FITNESS` Fitness >- `GAME` Practice Game >- `OTHER` Other ",
     )
     international_reference: Optional[constr(strict=True, max_length=30)] = Field(
         None,
         alias="internationalReference",
         description="The international reference for this fixture given by the sport governing body",
     )
     status: Optional[constr(strict=True, max_length=100)] = Field(
@@ -135,15 +135,15 @@
         None,
         alias="fixtureType",
         description="Type of fixture >- `ALL_STAR` All Star >- `DEMONSTRATION` Demonstration >- `FINAL` Final >- `FRIENDLY` Friendly >- `PLAYOFF` Playoff >- `PRESEASON` Pre Season >- `REGULAR` Regular ",
     )
     maximum_period_type_used: Optional[constr(strict=True, max_length=50)] = Field(
         None,
         alias="maximumPeriodTypeUsed",
-        description="Maximum Period Type Used >- `EXTRA_TIME` Extra Time >- `OVERTIME` Overtime >- `REGULAR` Regular >- `SHOOTOUT` Shoot-Out ",
+        description="Maximum Period Type Used >- None None >- `EXTRA_TIME` Extra Time >- `OVERTIME` Overtime >- `REGULAR` Regular >- `SHOOTOUT` Shoot-Out ",
     )
     competitor_type: Optional[constr(strict=True, max_length=50)] = Field(
         None,
         alias="competitorType",
         description="The type of competitors in this fixture >- `ENTITY` Entity >- `PERSON` Person ",
     )
     participants: Optional[conlist(FixtureParticipant)] = Field(None, description="Array of fixture participants")
@@ -231,16 +231,16 @@
 
     @validator("practice_drill_type")
     def practice_drill_type_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("DRILL", "GAME", "FITNESS", "OTHER"):
-            raise ValueError("must be one of enum values ('DRILL', 'GAME', 'FITNESS', 'OTHER')")
+        if value not in ("DRILL", "GAME", "FITNESS", "OTHER", "null"):
+            raise ValueError("must be one of enum values ('DRILL', 'GAME', 'FITNESS', 'OTHER', 'null')")
         return value
 
     @validator("status")
     def status_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
@@ -276,16 +276,16 @@
 
     @validator("maximum_period_type_used")
     def maximum_period_type_used_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("REGULAR", "EXTRA_TIME", "OVERTIME", "SHOOTOUT"):
-            raise ValueError("must be one of enum values ('REGULAR', 'EXTRA_TIME', 'OVERTIME', 'SHOOTOUT')")
+        if value not in ("REGULAR", "EXTRA_TIME", "OVERTIME", "SHOOTOUT", "null"):
+            raise ValueError("must be one of enum values ('REGULAR', 'EXTRA_TIME', 'OVERTIME', 'SHOOTOUT', 'null')")
         return value
 
     @validator("competitor_type")
     def competitor_type_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
@@ -315,16 +315,16 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> FixturesByEntityModel:
-        """Create an instance of FixturesByEntityModel from a JSON string"""
+    def from_json(cls, json_str: str) -> FixturesByCompetitionModel:
+        """Create an instance of FixturesByCompetitionModel from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(
             by_alias=True,
             exclude={
@@ -488,14 +488,19 @@
             _dict["roundCode"] = None
 
         # set to None if round_number (nullable) is None
         # and __fields_set__ contains the field
         if self.round_number is None and "round_number" in self.__fields_set__:
             _dict["roundNumber"] = None
 
+        # set to None if maximum_period_type_used (nullable) is None
+        # and __fields_set__ contains the field
+        if self.maximum_period_type_used is None and "maximum_period_type_used" in self.__fields_set__:
+            _dict["maximumPeriodTypeUsed"] = None
+
         # set to None if participants (nullable) is None
         # and __fields_set__ contains the field
         if self.participants is None and "participants" in self.__fields_set__:
             _dict["participants"] = None
 
         # set to None if competitors (nullable) is None
         # and __fields_set__ contains the field
@@ -521,23 +526,23 @@
         # and __fields_set__ contains the field
         if self.series_fixture_number is None and "series_fixture_number" in self.__fields_set__:
             _dict["seriesFixtureNumber"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> FixturesByEntityModel:
-        """Create an instance of FixturesByEntityModel from a dict"""
+    def from_dict(cls, obj: dict) -> FixturesByCompetitionModel:
+        """Create an instance of FixturesByCompetitionModel from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return FixturesByEntityModel.parse_obj(obj)
+            return FixturesByCompetitionModel.parse_obj(obj)
 
-        _obj = FixturesByEntityModel.parse_obj(
+        _obj = FixturesByCompetitionModel.parse_obj(
             {
                 "fixture_id": obj.get("fixtureId"),
                 "organization_id": obj.get("organizationId"),
                 "organization": FixturesModelOrganization.from_dict(obj.get("organization"))
                 if obj.get("organization") is not None
                 else None,
                 "season_id": obj.get("seasonId"),
```

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_by_entity_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixtures_by_entity_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixtures_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     )
     organization: Optional[FixturesModelOrganization] = None
     season_id: Optional[StrictStr] = Field(None, alias="seasonId", description="The unique identifier of the season")
     season: Optional[FixtureProgressionsModelSeason] = None
     practice_drill_type: Optional[constr(strict=True, max_length=100)] = Field(
         None,
         alias="practiceDrillType",
-        description="Practice types >- `DRILL` Drill >- `FITNESS` Fitness >- `GAME` Practice Game >- `OTHER` Other ",
+        description="Practice types >- None None >- `DRILL` Drill >- `FITNESS` Fitness >- `GAME` Practice Game >- `OTHER` Other ",
     )
     international_reference: Optional[constr(strict=True, max_length=30)] = Field(
         None,
         alias="internationalReference",
         description="The international reference for this fixture given by the sport governing body",
     )
     status: Optional[constr(strict=True, max_length=100)] = Field(
@@ -135,15 +135,15 @@
         None,
         alias="fixtureType",
         description="Type of fixture >- `ALL_STAR` All Star >- `DEMONSTRATION` Demonstration >- `FINAL` Final >- `FRIENDLY` Friendly >- `PLAYOFF` Playoff >- `PRESEASON` Pre Season >- `REGULAR` Regular ",
     )
     maximum_period_type_used: Optional[constr(strict=True, max_length=50)] = Field(
         None,
         alias="maximumPeriodTypeUsed",
-        description="Maximum Period Type Used >- `EXTRA_TIME` Extra Time >- `OVERTIME` Overtime >- `REGULAR` Regular >- `SHOOTOUT` Shoot-Out ",
+        description="Maximum Period Type Used >- None None >- `EXTRA_TIME` Extra Time >- `OVERTIME` Overtime >- `REGULAR` Regular >- `SHOOTOUT` Shoot-Out ",
     )
     competitor_type: Optional[constr(strict=True, max_length=50)] = Field(
         None,
         alias="competitorType",
         description="The type of competitors in this fixture >- `ENTITY` Entity >- `PERSON` Person ",
     )
     participants: Optional[conlist(FixtureParticipant)] = Field(None, description="Array of fixture participants")
@@ -231,16 +231,16 @@
 
     @validator("practice_drill_type")
     def practice_drill_type_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("DRILL", "GAME", "FITNESS", "OTHER"):
-            raise ValueError("must be one of enum values ('DRILL', 'GAME', 'FITNESS', 'OTHER')")
+        if value not in ("DRILL", "GAME", "FITNESS", "OTHER", "null"):
+            raise ValueError("must be one of enum values ('DRILL', 'GAME', 'FITNESS', 'OTHER', 'null')")
         return value
 
     @validator("status")
     def status_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
@@ -276,16 +276,16 @@
 
     @validator("maximum_period_type_used")
     def maximum_period_type_used_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("REGULAR", "EXTRA_TIME", "OVERTIME", "SHOOTOUT"):
-            raise ValueError("must be one of enum values ('REGULAR', 'EXTRA_TIME', 'OVERTIME', 'SHOOTOUT')")
+        if value not in ("REGULAR", "EXTRA_TIME", "OVERTIME", "SHOOTOUT", "null"):
+            raise ValueError("must be one of enum values ('REGULAR', 'EXTRA_TIME', 'OVERTIME', 'SHOOTOUT', 'null')")
         return value
 
     @validator("competitor_type")
     def competitor_type_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
@@ -488,14 +488,19 @@
             _dict["roundCode"] = None
 
         # set to None if round_number (nullable) is None
         # and __fields_set__ contains the field
         if self.round_number is None and "round_number" in self.__fields_set__:
             _dict["roundNumber"] = None
 
+        # set to None if maximum_period_type_used (nullable) is None
+        # and __fields_set__ contains the field
+        if self.maximum_period_type_used is None and "maximum_period_type_used" in self.__fields_set__:
+            _dict["maximumPeriodTypeUsed"] = None
+
         # set to None if participants (nullable) is None
         # and __fields_set__ contains the field
         if self.participants is None and "participants" in self.__fields_set__:
             _dict["participants"] = None
 
         # set to None if competitors (nullable) is None
         # and __fields_set__ contains the field
```

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_model_fixture_profile.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixtures_model_fixture_profile.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixtures_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_model_round.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixtures_model_round.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_model_series.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixtures_model_series.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_model_venue.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixtures_model_venue.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/fixtures_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/fixtures_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/game_log_entity_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/game_log_entity_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/game_log_entity_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/game_log_entity_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/game_log_entity_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/game_log_entity_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/game_log_person_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/game_log_person_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/game_log_person_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/game_log_person_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/game_log_person_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/game_log_person_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/head_to_head_identification.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/head_to_head_identification.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/head_to_head_identification_for_subsequent_checks.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/head_to_head_identification_for_subsequent_checks.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/head_to_head_resolution.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/head_to_head_resolution.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/head_to_head_resolution_for_extra_depth_h2h_s.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/head_to_head_resolution_for_extra_depth_h2h_s.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/images_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/images_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         None,
         alias="imageType",
         description="Upload Type >- `LOGO` Logo - Not valid for 'PERSON' baseType >- `LOGO_ALTERNATE` Logo (alternate) - Not valid for 'PERSON' baseType >- `LOGO_BACKGROUND` Stylised logo for background purposes - Not valid for 'PERSON' baseType >- `PERSON_HEAD` Head shot (shoulders and head) - Only valid for 'PERSON' baseType >- `PERSON_POSE` Person posing - Only valid for 'PERSON' baseType >- `PERSON_WAIST` Head shot from the waist up - Only valid for 'PERSON' baseType >- `TEAM_PHOTO` Team Photo - Only valid for 'ENTITY' baseType ",
     )
     secondary_type: Optional[constr(strict=True, max_length=100)] = Field(
         None,
         alias="secondaryType",
-        description="If the image relates to a secondary object. Such as a photo of a person in an entity, then baseType would be PERSON and secondaryType would be ENTITY. >- `COMPETITION` Competition >- `CONFERENCE` Conference >- `DIVISION` Division >- `ENTITY` Entity >- `ENTITYGROUP` Entity Group >- `LEAGUE` League >- `SEASON` Season ",
+        description="If the image relates to a secondary object. Such as a photo of a person in an entity, then baseType would be PERSON and secondaryType would be ENTITY. >- None None >- `COMPETITION` Competition >- `CONFERENCE` Conference >- `DIVISION` Division >- `ENTITY` Entity >- `ENTITYGROUP` Entity Group >- `LEAGUE` League >- `SEASON` Season ",
     )
     secondary_id: Optional[StrictStr] = Field(
         None, alias="secondaryId", description="The unique identifier of the object associated with the secondaryType"
     )
     rating: Optional[constr(strict=True, max_length=100)] = Field(
         None,
         description="The rating given to the quality of the image.  All images are LOW by default but are set ad MEDIUM if they are large enough and have transparency.  Images are only marked as HIGH if they have been manually reviewed.  You should take your use-case into account when you go to use the image. >- `HIGH` High >- `LOW` Low >- `MEDIUM` Medium ",
@@ -150,17 +150,17 @@
 
     @validator("secondary_type")
     def secondary_type_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("ENTITY", "ENTITYGROUP", "COMPETITION", "SEASON", "LEAGUE", "DIVISION", "CONFERENCE"):
+        if value not in ("ENTITY", "ENTITYGROUP", "COMPETITION", "SEASON", "LEAGUE", "DIVISION", "CONFERENCE", "null"):
             raise ValueError(
-                "must be one of enum values ('ENTITY', 'ENTITYGROUP', 'COMPETITION', 'SEASON', 'LEAGUE', 'DIVISION', 'CONFERENCE')"
+                "must be one of enum values ('ENTITY', 'ENTITYGROUP', 'COMPETITION', 'SEASON', 'LEAGUE', 'DIVISION', 'CONFERENCE', 'null')"
             )
         return value
 
     @validator("rating")
     def rating_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
@@ -205,14 +205,19 @@
                 "added",
             },
             exclude_none=True,
         )
         # override the default output from pydantic by calling `to_dict()` of organization
         if self.organization:
             _dict["organization"] = self.organization.to_dict()
+        # set to None if secondary_type (nullable) is None
+        # and __fields_set__ contains the field
+        if self.secondary_type is None and "secondary_type" in self.__fields_set__:
+            _dict["secondaryType"] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> ImagesModel:
         """Create an instance of ImagesModel from a dict"""
         if obj is None:
             return None
```

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/images_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/images_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/images_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/images_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/images_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/images_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/images_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/images_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/included_data.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/included_data.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_criteria_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leader_criteria_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_criteria_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leader_criteria_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_criteria_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leader_criteria_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_criteria_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leader_criteria_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_criteria_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leader_criteria_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_qualifier_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leader_qualifier_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_qualifier_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leader_qualifier_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_qualifiers_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leader_qualifiers_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_qualifiers_model_leaders_criteria.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leader_qualifiers_model_leaders_criteria.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_qualifiers_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leader_qualifiers_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_qualifiers_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leader_qualifiers_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_summary_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leader_summary_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leader_summary_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leader_summary_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/league_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/league_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/league_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/league_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leagues_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leagues_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leagues_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leagues_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/leagues_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/leagues_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/organization_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/organization_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/organization_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/organization_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/organizations_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/organizations_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/organizations_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/organizations_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/person_additional_details.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/person_additional_details.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/person_historical_name.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/person_historical_name.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/person_list_default_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/person_list_default_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/person_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/person_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/person_post_body_additional_names_value.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/person_post_body_additional_names_value.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/person_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/person_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/persons_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/persons_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/persons_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/persons_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/persons_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/persons_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/pool_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/pool_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/pool_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/pool_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/ranking_rows_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/ranking_rows_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/ranking_rows_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/ranking_rows_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/ranking_rows_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/ranking_rows_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/ranking_rows_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/ranking_rows_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/response_links.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/response_links.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/response_meta_data.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/response_meta_data.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/role_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/role_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/role_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/role_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/roles_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/roles_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/roles_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/roles_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/roles_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/roles_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/round_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/round_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/round_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/round_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entities_list_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_entities_list_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entities_list_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_entities_list_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entities_list_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_entities_list_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entities_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_entities_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entities_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_entities_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entities_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_entities_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_base_statistics_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_base_statistics_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_base_statistics_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_base_statistics_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_placings_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_entity_placings_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_placings_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_entity_placings_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_statistics_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_entity_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_statistics_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_entity_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_entity_statistics_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_entity_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_pool.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_pool.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_stage.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_stage.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_base_statistics_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_person_base_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_base_statistics_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_person_base_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_base_statistics_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_person_base_statistics_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_base_statistics_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_person_base_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_placings_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_person_placings_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_placings_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_person_placings_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_statistics_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_person_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_statistics_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_person_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_statistics_periods_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_person_statistics_periods_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_statistics_periods_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_person_statistics_periods_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_statistics_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_person_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_total_statistics_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_person_total_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_total_statistics_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_person_total_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_person_total_statistics_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_person_total_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_persons_list_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_persons_list_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_persons_list_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_persons_list_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_persons_list_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_persons_list_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_persons_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_persons_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_persons_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_persons_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_persons_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_persons_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_pools_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_pools_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_pools_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_pools_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_pools_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_pools_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_roster_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_roster_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_roster_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_roster_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_roster_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_roster_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_roster_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_roster_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_rounds_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_rounds_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_rounds_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_rounds_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_rounds_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_rounds_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_series_competitor.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_series_competitor.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_series_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_series_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_series_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_series_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_series_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_series_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_stage_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_stage_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_stage_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_stage_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_stages_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_stages_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_stages_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_stages_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_stages_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_stages_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_venues_address.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_venues_address.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_venues_list_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_venues_list_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_venues_list_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_venues_list_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_venues_list_model_site.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_venues_list_model_site.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/season_venues_list_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/season_venues_list_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasonentity_placings_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/seasonentity_placings_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasonentity_placings_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/seasonentity_placings_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasonperson_placings_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/seasonperson_placings_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasonperson_placings_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/seasonperson_placings_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasonroster_configuration.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/seasonroster_configuration.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasons_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/seasons_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasons_model_competition.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/seasons_model_competition.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasons_model_fixture_profile.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/seasons_model_fixture_profile.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasons_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/seasons_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasons_model_standing_configuration.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/seasons_model_standing_configuration.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/seasons_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/seasons_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/series_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/series_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/series_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/series_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/site_address.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/site_address.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/site_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/site_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/site_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/site_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/sites_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/sites_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/sites_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/sites_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/sites_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/sites_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/social_media.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/social_media.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/sorting.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/sorting.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_adjustment_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_adjustment_post_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,16 +49,16 @@
     )
     conference_id: Optional[StrictStr] = Field(
         None, alias="conferenceId", description="The unique identifier of the conference"
     )
     apply_to_all_standings: Optional[StrictBool] = Field(
         None, alias="applyToAllStandings", description="Apply to all generated standing types ?"
     )
-    adjustment_group: Optional[StrictStr] = Field(
-        None,
+    adjustment_group: StrictStr = Field(
+        ...,
         alias="adjustmentGroup",
         description="Adjustment Group >- `IN_CONFERENCE` In Conference >- `IN_DIVISION` In Division >- `OUT_CONFERENCE` Out Conference >- `OUT_DIVISION` Out Division >- `OVERALL` Overall ",
     )
     adjustment_type: StrictStr = Field(
         ..., alias="adjustmentType", description="Adjustment Type >- `ADD_MINUS` Add/Subtract Value >- `SET` Set Value "
     )
     adjustment_field: StrictStr = Field(
@@ -91,17 +91,14 @@
         "reasonType",
         "reasonDescription",
     ]
 
     @validator("adjustment_group")
     def adjustment_group_validate_enum(cls, value):
         """Validates the enum"""
-        if value is None:
-            return value
-
         if value not in ("OVERALL", "IN_CONFERENCE", "OUT_CONFERENCE", "IN_DIVISION", "OUT_DIVISION"):
             raise ValueError(
                 "must be one of enum values ('OVERALL', 'IN_CONFERENCE', 'OUT_CONFERENCE', 'IN_DIVISION', 'OUT_DIVISION')"
             )
         return value
 
     @validator("adjustment_type")
```

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_adjustment_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_adjustment_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_adjustments_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_adjustments_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_adjustments_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_adjustments_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_adjustments_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_adjustments_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_building.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_building.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_configuration.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_configuration.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_configurations_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_configurations_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_configurations_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_configurations_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_configurations_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_configurations_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_configurations_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_configurations_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_configurations_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_configurations_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_post_body_calculated_value.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_post_body_calculated_value.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_post_body_points_value.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_post_body_points_value.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standing_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standing_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standings_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standings_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standings_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standings_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/standings_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/standings_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/success_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/success_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/success_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/success_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/transfer_component.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/transfer_component.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/transfer_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/transfer_post_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,16 @@
     )
     competition_id: Optional[StrictStr] = Field(
         None, alias="competitionId", description="The unique identifier of the competition"
     )
     season_id: Optional[StrictStr] = Field(None, alias="seasonId", description="The unique identifier of the season")
     components: Optional[conlist(TransferComponent)] = Field(None, description="List of transfer components")
     status: Optional[constr(strict=True, max_length=30)] = Field(
-        None, description="Transfer Status >- `APPROVED` Approved >- `DECLINED` Decline >- `PENDING` Pending "
+        None,
+        description="Transfer Status >- None None >- `APPROVED` Approved >- `DECLINED` Decline >- `PENDING` Pending ",
     )
     reference: Optional[constr(strict=True, max_length=100)] = Field(None, description="Transfer reference number")
     transfer_type: constr(strict=True, max_length=100) = Field(
         ...,
         alias="transferType",
         description="Type of transfer >- `DROPPED` Dropped >- `OTHER` Other >- `PERMIT` Permit >- `TRADE` Trade >- `TRANSFER` Transfer ",
     )
@@ -71,16 +72,16 @@
 
     @validator("status")
     def status_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("APPROVED", "PENDING", "DECLINED"):
-            raise ValueError("must be one of enum values ('APPROVED', 'PENDING', 'DECLINED')")
+        if value not in ("APPROVED", "PENDING", "DECLINED", "null"):
+            raise ValueError("must be one of enum values ('APPROVED', 'PENDING', 'DECLINED', 'null')")
         return value
 
     @validator("transfer_type")
     def transfer_type_validate_enum(cls, value):
         """Validates the enum"""
         if value not in ("TRADE", "TRANSFER", "DROPPED", "PERMIT", "OTHER"):
             raise ValueError("must be one of enum values ('TRADE', 'TRANSFER', 'DROPPED', 'PERMIT', 'OTHER')")
@@ -126,14 +127,19 @@
                     _items.append(_item.to_dict())
             _dict["components"] = _items
         # set to None if components (nullable) is None
         # and __fields_set__ contains the field
         if self.components is None and "components" in self.__fields_set__:
             _dict["components"] = None
 
+        # set to None if status (nullable) is None
+        # and __fields_set__ contains the field
+        if self.status is None and "status" in self.__fields_set__:
+            _dict["status"] = None
+
         # set to None if date_transfer (nullable) is None
         # and __fields_set__ contains the field
         if self.date_transfer is None and "date_transfer" in self.__fields_set__:
             _dict["dateTransfer"] = None
 
         # set to None if date_permit_from (nullable) is None
         # and __fields_set__ contains the field
```

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/transfer_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/transfer_put_body.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 
     competition_id: Optional[StrictStr] = Field(
         None, alias="competitionId", description="The unique identifier of the competition"
     )
     season_id: Optional[StrictStr] = Field(None, alias="seasonId", description="The unique identifier of the season")
     components: Optional[conlist(TransferComponent)] = Field(None, description="List of transfer components")
     status: Optional[constr(strict=True, max_length=30)] = Field(
-        None, description="Transfer Status >- `APPROVED` Approved >- `DECLINED` Decline >- `PENDING` Pending "
+        None,
+        description="Transfer Status >- None None >- `APPROVED` Approved >- `DECLINED` Decline >- `PENDING` Pending ",
     )
     reference: Optional[constr(strict=True, max_length=100)] = Field(None, description="Transfer reference number")
     transfer_type: Optional[constr(strict=True, max_length=100)] = Field(
         None,
         alias="transferType",
         description="Type of transfer >- `DROPPED` Dropped >- `OTHER` Other >- `PERMIT` Permit >- `TRADE` Trade >- `TRANSFER` Transfer ",
     )
@@ -67,16 +68,16 @@
 
     @validator("status")
     def status_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("APPROVED", "PENDING", "DECLINED"):
-            raise ValueError("must be one of enum values ('APPROVED', 'PENDING', 'DECLINED')")
+        if value not in ("APPROVED", "PENDING", "DECLINED", "null"):
+            raise ValueError("must be one of enum values ('APPROVED', 'PENDING', 'DECLINED', 'null')")
         return value
 
     @validator("transfer_type")
     def transfer_type_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
@@ -125,14 +126,19 @@
                     _items.append(_item.to_dict())
             _dict["components"] = _items
         # set to None if components (nullable) is None
         # and __fields_set__ contains the field
         if self.components is None and "components" in self.__fields_set__:
             _dict["components"] = None
 
+        # set to None if status (nullable) is None
+        # and __fields_set__ contains the field
+        if self.status is None and "status" in self.__fields_set__:
+            _dict["status"] = None
+
         # set to None if date_transfer (nullable) is None
         # and __fields_set__ contains the field
         if self.date_transfer is None and "date_transfer" in self.__fields_set__:
             _dict["dateTransfer"] = None
 
         # set to None if date_permit_from (nullable) is None
         # and __fields_set__ contains the field
```

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/transfers_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/transfers_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,16 @@
         None, alias="competitionId", description="The unique identifier of the competition"
     )
     competition: Optional[SeasonsModelCompetition] = None
     season_id: Optional[StrictStr] = Field(None, alias="seasonId", description="The unique identifier of the season")
     season: Optional[FixtureProgressionsModelSeason] = None
     components: Optional[conlist(TransferComponent)] = Field(None, description="List of transfer components")
     status: Optional[constr(strict=True, max_length=30)] = Field(
-        None, description="Transfer Status >- `APPROVED` Approved >- `DECLINED` Decline >- `PENDING` Pending "
+        None,
+        description="Transfer Status >- None None >- `APPROVED` Approved >- `DECLINED` Decline >- `PENDING` Pending ",
     )
     reference: Optional[constr(strict=True, max_length=100)] = Field(None, description="Transfer reference number")
     transfer_type: Optional[constr(strict=True, max_length=100)] = Field(
         None,
         alias="transferType",
         description="Type of transfer >- `DROPPED` Dropped >- `OTHER` Other >- `PERMIT` Permit >- `TRADE` Trade >- `TRANSFER` Transfer ",
     )
@@ -88,16 +89,16 @@
 
     @validator("status")
     def status_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("APPROVED", "PENDING", "DECLINED"):
-            raise ValueError("must be one of enum values ('APPROVED', 'PENDING', 'DECLINED')")
+        if value not in ("APPROVED", "PENDING", "DECLINED", "null"):
+            raise ValueError("must be one of enum values ('APPROVED', 'PENDING', 'DECLINED', 'null')")
         return value
 
     @validator("transfer_type")
     def transfer_type_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
@@ -163,14 +164,19 @@
                     _items.append(_item.to_dict())
             _dict["components"] = _items
         # set to None if components (nullable) is None
         # and __fields_set__ contains the field
         if self.components is None and "components" in self.__fields_set__:
             _dict["components"] = None
 
+        # set to None if status (nullable) is None
+        # and __fields_set__ contains the field
+        if self.status is None and "status" in self.__fields_set__:
+            _dict["status"] = None
+
         # set to None if date_transfer (nullable) is None
         # and __fields_set__ contains the field
         if self.date_transfer is None and "date_transfer" in self.__fields_set__:
             _dict["dateTransfer"] = None
 
         # set to None if date_permit_from (nullable) is None
         # and __fields_set__ contains the field
```

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/transfers_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/transfers_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/transfers_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/transfers_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venue_address.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/venue_address.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venue_historical_name.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/venue_historical_name.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venue_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/venue_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venue_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/venue_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venues_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/venues_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venues_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/venues_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venues_model_site.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/venues_model_site.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/venues_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/venues_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_file_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_file_post_body.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,35 +52,35 @@
     content: constr(strict=True, max_length=30) = Field(
         ...,
         description="Content of the stream >- `CLEAN` Output signal is the same as the input signal >- `PROGRAM` Score overlays and other enhancements have been added to the stream ",
     )
     fps: StrictInt = Field(..., description="fps for the video stream")
     origin: Optional[constr(strict=True, max_length=30)] = Field(
         None,
-        description="The origin of the video file >- `STREAM` Streamed >- `UPLOAD` Uploaded >- `VENUE` Recorded in venue ",
+        description="The origin of the video file >- None None >- `STREAM` Streamed >- `UPLOAD` Uploaded >- `VENUE` Recorded in venue ",
     )
     format: Optional[constr(strict=True, max_length=30)] = Field(
         None, description="The format of the video file >- `HLS` A HLS play list >- `MP4` One MP4 file "
     )
     storage_provider: Optional[constr(strict=True, max_length=30)] = Field(
         None,
         alias="storageProvider",
-        description="Where the video file is stored? >- `5STREAM` 5stream >- `KEEMOTION` Keemotion >- `SYNERGY` Synergy ",
+        description="Where the video file is stored? >- None None >- `5STREAM` 5stream >- `KEEMOTION` Keemotion >- `SYNERGY` Synergy ",
     )
     size: Optional[Union[StrictFloat, StrictInt]] = Field(
         None, description="Size (Mb) of the video (only given if a single file)"
     )
     length: Optional[Union[StrictFloat, StrictInt]] = Field(None, description="Lenth (mins) of the video")
     encoding: Optional[constr(strict=True, max_length=30)] = Field(
         None, description="How is the video/audio encoded. codecs etc."
     )
     url: constr(strict=True, max_length=200) = Field(..., description="The URL where the file can be found")
     status: Optional[constr(strict=True, max_length=30)] = Field(
         None,
-        description="What is the status of the file? >- `AVAILABLE` Available for access >- `BUILDABLE` Not currently available - but can be built on request >- `PENDING` Being added - some parts may be available ",
+        description="What is the status of the file? >- None None >- `AVAILABLE` Available for access >- `BUILDABLE` Not currently available - but can be built on request >- `PENDING` Being added - some parts may be available ",
     )
     start_time: datetime = Field(..., alias="startTime", description="The time this recording started (UTC)")
     expiry: Optional[datetime] = Field(None, description="When does this file expire? (UTC)")
     __properties = [
         "videoId",
         "provider",
         "locale",
@@ -133,16 +133,16 @@
 
     @validator("origin")
     def origin_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("STREAM", "VENUE", "UPLOAD"):
-            raise ValueError("must be one of enum values ('STREAM', 'VENUE', 'UPLOAD')")
+        if value not in ("STREAM", "VENUE", "UPLOAD", "null"):
+            raise ValueError("must be one of enum values ('STREAM', 'VENUE', 'UPLOAD', 'null')")
         return value
 
     @validator("format")
     def format_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
@@ -153,26 +153,26 @@
 
     @validator("storage_provider")
     def storage_provider_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("5STREAM", "KEEMOTION", "SYNERGY"):
-            raise ValueError("must be one of enum values ('5STREAM', 'KEEMOTION', 'SYNERGY')")
+        if value not in ("5STREAM", "KEEMOTION", "SYNERGY", "null"):
+            raise ValueError("must be one of enum values ('5STREAM', 'KEEMOTION', 'SYNERGY', 'null')")
         return value
 
     @validator("status")
     def status_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("AVAILABLE", "BUILDABLE", "PENDING"):
-            raise ValueError("must be one of enum values ('AVAILABLE', 'BUILDABLE', 'PENDING')")
+        if value not in ("AVAILABLE", "BUILDABLE", "PENDING", "null"):
+            raise ValueError("must be one of enum values ('AVAILABLE', 'BUILDABLE', 'PENDING', 'null')")
         return value
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
@@ -189,24 +189,39 @@
     def from_json(cls, json_str: str) -> VideoFilePostBody:
         """Create an instance of VideoFilePostBody from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
+        # set to None if origin (nullable) is None
+        # and __fields_set__ contains the field
+        if self.origin is None and "origin" in self.__fields_set__:
+            _dict["origin"] = None
+
+        # set to None if storage_provider (nullable) is None
+        # and __fields_set__ contains the field
+        if self.storage_provider is None and "storage_provider" in self.__fields_set__:
+            _dict["storageProvider"] = None
+
         # set to None if size (nullable) is None
         # and __fields_set__ contains the field
         if self.size is None and "size" in self.__fields_set__:
             _dict["size"] = None
 
         # set to None if length (nullable) is None
         # and __fields_set__ contains the field
         if self.length is None and "length" in self.__fields_set__:
             _dict["length"] = None
 
+        # set to None if status (nullable) is None
+        # and __fields_set__ contains the field
+        if self.status is None and "status" in self.__fields_set__:
+            _dict["status"] = None
+
         # set to None if expiry (nullable) is None
         # and __fields_set__ contains the field
         if self.expiry is None and "expiry" in self.__fields_set__:
             _dict["expiry"] = None
 
         return _dict
```

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_files_download_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_files_download_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_files_download_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_files_download_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_files_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_files_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,34 +64,34 @@
     content: Optional[constr(strict=True, max_length=30)] = Field(
         None,
         description="Content of the stream >- `CLEAN` Output signal is the same as the input signal >- `PROGRAM` Score overlays and other enhancements have been added to the stream ",
     )
     fps: Optional[StrictInt] = Field(25, description="fps for the video stream")
     origin: Optional[constr(strict=True, max_length=30)] = Field(
         None,
-        description="The origin of the video file >- `STREAM` Streamed >- `UPLOAD` Uploaded >- `VENUE` Recorded in venue ",
+        description="The origin of the video file >- None None >- `STREAM` Streamed >- `UPLOAD` Uploaded >- `VENUE` Recorded in venue ",
     )
     format: Optional[constr(strict=True, max_length=30)] = Field(
         None, description="The format of the video file >- `HLS` A HLS play list >- `MP4` One MP4 file "
     )
     storage_provider: Optional[constr(strict=True, max_length=30)] = Field(
         None,
         alias="storageProvider",
-        description="Where the video file is stored? >- `5STREAM` 5stream >- `KEEMOTION` Keemotion >- `SYNERGY` Synergy ",
+        description="Where the video file is stored? >- None None >- `5STREAM` 5stream >- `KEEMOTION` Keemotion >- `SYNERGY` Synergy ",
     )
     size: Optional[Union[StrictFloat, StrictInt]] = Field(
         None, description="Size (Mb) of the video (only given if a single file)"
     )
     length: Optional[Union[StrictFloat, StrictInt]] = Field(None, description="Lenth (mins) of the video")
     encoding: Optional[constr(strict=True, max_length=30)] = Field(
         None, description="How is the video/audio encoded. codecs etc."
     )
     status: Optional[constr(strict=True, max_length=30)] = Field(
         None,
-        description="What is the status of the file? >- `AVAILABLE` Available for access >- `BUILDABLE` Not currently available - but can be built on request >- `PENDING` Being added - some parts may be available ",
+        description="What is the status of the file? >- None None >- `AVAILABLE` Available for access >- `BUILDABLE` Not currently available - but can be built on request >- `PENDING` Being added - some parts may be available ",
     )
     start_time: Optional[datetime] = Field(None, alias="startTime", description="The time this recording started (UTC)")
     expiry: Optional[datetime] = Field(None, description="When does this file expire? (UTC)")
     updated: Optional[datetime] = Field(None, description="Date/time last modified. In UTC")
     added: Optional[datetime] = Field(None, description="Date/time added. In UTC")
     __properties = [
         "videoId",
@@ -162,16 +162,16 @@
 
     @validator("origin")
     def origin_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("STREAM", "VENUE", "UPLOAD"):
-            raise ValueError("must be one of enum values ('STREAM', 'VENUE', 'UPLOAD')")
+        if value not in ("STREAM", "VENUE", "UPLOAD", "null"):
+            raise ValueError("must be one of enum values ('STREAM', 'VENUE', 'UPLOAD', 'null')")
         return value
 
     @validator("format")
     def format_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
@@ -182,26 +182,26 @@
 
     @validator("storage_provider")
     def storage_provider_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("5STREAM", "KEEMOTION", "SYNERGY"):
-            raise ValueError("must be one of enum values ('5STREAM', 'KEEMOTION', 'SYNERGY')")
+        if value not in ("5STREAM", "KEEMOTION", "SYNERGY", "null"):
+            raise ValueError("must be one of enum values ('5STREAM', 'KEEMOTION', 'SYNERGY', 'null')")
         return value
 
     @validator("status")
     def status_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ("AVAILABLE", "BUILDABLE", "PENDING"):
-            raise ValueError("must be one of enum values ('AVAILABLE', 'BUILDABLE', 'PENDING')")
+        if value not in ("AVAILABLE", "BUILDABLE", "PENDING", "null"):
+            raise ValueError("must be one of enum values ('AVAILABLE', 'BUILDABLE', 'PENDING', 'null')")
         return value
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
@@ -232,24 +232,39 @@
         )
         # override the default output from pydantic by calling `to_dict()` of organization
         if self.organization:
             _dict["organization"] = self.organization.to_dict()
         # override the default output from pydantic by calling `to_dict()` of fixture
         if self.fixture:
             _dict["fixture"] = self.fixture.to_dict()
+        # set to None if origin (nullable) is None
+        # and __fields_set__ contains the field
+        if self.origin is None and "origin" in self.__fields_set__:
+            _dict["origin"] = None
+
+        # set to None if storage_provider (nullable) is None
+        # and __fields_set__ contains the field
+        if self.storage_provider is None and "storage_provider" in self.__fields_set__:
+            _dict["storageProvider"] = None
+
         # set to None if size (nullable) is None
         # and __fields_set__ contains the field
         if self.size is None and "size" in self.__fields_set__:
             _dict["size"] = None
 
         # set to None if length (nullable) is None
         # and __fields_set__ contains the field
         if self.length is None and "length" in self.__fields_set__:
             _dict["length"] = None
 
+        # set to None if status (nullable) is None
+        # and __fields_set__ contains the field
+        if self.status is None and "status" in self.__fields_set__:
+            _dict["status"] = None
+
         # set to None if expiry (nullable) is None
         # and __fields_set__ contains the field
         if self.expiry is None and "expiry" in self.__fields_set__:
             _dict["expiry"] = None
 
         return _dict
```

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_files_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_files_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_files_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_files_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_inputs_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_stream_inputs_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_inputs_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_stream_inputs_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_inputs_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_stream_inputs_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_local_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_stream_local_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_local_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_stream_local_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_local_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_stream_local_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_local_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_stream_local_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_local_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_stream_local_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_outputs_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_stream_outputs_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_outputs_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_stream_outputs_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_stream_outputs_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_stream_outputs_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_subscription_post_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_subscription_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_subscription_put_body.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_subscription_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_subscriptions_model.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_subscriptions_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_subscriptions_model_organization.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_subscriptions_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/models/video_subscriptions_response.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/models/video_subscriptions_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore/openapi/rest.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore/openapi/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,14 +153,15 @@
                 timeout = urllib3.Timeout(total=_request_timeout)
             elif isinstance(_request_timeout, tuple) and len(_request_timeout) == 2:
                 timeout = urllib3.Timeout(connect=_request_timeout[0], read=_request_timeout[1])
 
         try:
             # For `POST`, `PUT`, `PATCH`, `OPTIONS`, `DELETE`
             if method in ["POST", "PUT", "PATCH", "OPTIONS", "DELETE"]:
+
                 # no content type provided or payload is json
                 if not headers.get("Content-Type") or re.search("json", headers["Content-Type"], re.IGNORECASE):
                     request_body = None
                     if body is not None:
                         request_body = json.dumps(body)
                     r = self.pool_manager.request(
                         method,
```

### Comparing `atriumsports_sdk-1.3.2/atriumsports/datacore_stream/datacore_stream.py` & `atriumsports_sdk-1.4.0/atriumsports/datacore_stream/datacore_stream.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports/endpoints.py` & `atriumsports_sdk-1.4.0/atriumsports/endpoints.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.3.2/atriumsports_sdk.egg-info/PKG-INFO` & `atriumsports_sdk-1.4.0/atriumsports_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atriumsports-sdk
-Version: 1.3.2
+Version: 1.4.0
 Summary: Python module for integration to Atrium Sports APIs
 Author: Atrium Sports
 Author-email: python_dev@atriumsports.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `atriumsports_sdk-1.3.2/atriumsports_sdk.egg-info/SOURCES.txt` & `atriumsports_sdk-1.4.0/atriumsports_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -195,14 +195,16 @@
 atriumsports/datacore/openapi/models/fixture_progressions_response.py
 atriumsports/datacore/openapi/models/fixture_put_body.py
 atriumsports/datacore/openapi/models/fixture_roster_model.py
 atriumsports/datacore/openapi/models/fixture_roster_model_organization.py
 atriumsports/datacore/openapi/models/fixture_roster_post_body.py
 atriumsports/datacore/openapi/models/fixture_roster_response.py
 atriumsports/datacore/openapi/models/fixture_videosteam_post_body.py
+atriumsports/datacore/openapi/models/fixtures_by_competition_model.py
+atriumsports/datacore/openapi/models/fixtures_by_competition_response.py
 atriumsports/datacore/openapi/models/fixtures_by_entity_model.py
 atriumsports/datacore/openapi/models/fixtures_by_entity_response.py
 atriumsports/datacore/openapi/models/fixtures_model.py
 atriumsports/datacore/openapi/models/fixtures_model_fixture_profile.py
 atriumsports/datacore/openapi/models/fixtures_model_organization.py
 atriumsports/datacore/openapi/models/fixtures_model_round.py
 atriumsports/datacore/openapi/models/fixtures_model_series.py
```

### Comparing `atriumsports_sdk-1.3.2/setup.py` & `atriumsports_sdk-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     setuptools.setup(
         name="atriumsports_sdk",
-        version="1.3.2",
+        version="1.4.0",
         author="Atrium Sports",
         author_email="python_dev@atriumsports.com",
         description="Python module for integration to Atrium Sports APIs",
         long_description=long_description,
         long_description_content_type="text/markdown",
         packages=setuptools.find_packages(),
         classifiers=[
```

