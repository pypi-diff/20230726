# Comparing `tmp/getajob-0.5.0.tar.gz` & `tmp/getajob-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getajob-0.5.0.tar", max compression
+gzip compressed data, was "getajob-0.5.1.tar", max compression
```

## Comparing `getajob-0.5.0.tar` & `getajob-0.5.1.tar`

### file list

```diff
@@ -1,152 +1,152 @@
--rw-r--r--   0        0        0    11357 2023-07-26 19:33:33.250794 getajob-0.5.0/LICENSE
--rw-r--r--   0        0        0       69 2023-07-26 19:33:33.250794 getajob-0.5.0/README.md
--rw-r--r--   0        0        0       22 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/__init__.py
--rw-r--r--   0        0        0     2927 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/abstractions/models.py
--rw-r--r--   0        0        0    16351 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/abstractions/repository.py
--rw-r--r--   0        0        0      385 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/abstractions/vendor_client_factory.py
--rw-r--r--   0        0        0     2121 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/config/settings.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/contexts/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/contexts/admin/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/contexts/admin/search/__init__.py
--rw-r--r--   0        0        0      177 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/contexts/admin/search/models.py
--rw-r--r--   0        0        0      607 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/contexts/admin/search/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/contexts/admin/users/__init__.py
--rw-r--r--   0        0        0      620 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/contexts/admin/users/models.py
--rw-r--r--   0        0        0      844 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/contexts/admin/users/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/contexts/applicant_matching/__init__.py
--rw-r--r--   0        0        0     1347 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/contexts/applicant_matching/models.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/contexts/applications/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/contexts/applications/applicant_tracking/__init__.py
--rw-r--r--   0        0        0     1044 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/contexts/applications/applicant_tracking/models.py
--rw-r--r--   0        0        0     2498 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/contexts/applications/applicant_tracking/repository.py
--rw-r--r--   0        0        0      277 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/contexts/applications/enumerations.py
--rw-r--r--   0        0        0      726 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/applications/models.py
--rw-r--r--   0        0        0     3635 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/applications/repository.py
--rw-r--r--   0        0        0     2629 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/applications/unit_of_work.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/chat/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/chat/message/__init__.py
--rw-r--r--   0        0        0      616 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/chat/message/models.py
--rw-r--r--   0        0        0      889 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/chat/message/repository.py
--rw-r--r--   0        0        0      272 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/chat/models.py
--rw-r--r--   0        0        0     1770 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/chat/repository.py
--rw-r--r--   0        0        0     1650 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/chat/unit_of_work.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/applicant_tracking_settings/__init__.py
--rw-r--r--   0        0        0      331 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/applicant_tracking_settings/models.py
--rw-r--r--   0        0        0      817 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/applicant_tracking_settings/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/audit/__init__.py
--rw-r--r--   0        0        0      482 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/audit/models.py
--rw-r--r--   0        0        0     1101 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/audit/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/details/__init__.py
--rw-r--r--   0        0        0      743 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/details/models.py
--rw-r--r--   0        0        0     1451 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/details/repository.py
--rw-r--r--   0        0        0     1870 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/enumerations.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/invitations/__init__.py
--rw-r--r--   0        0        0      145 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/invitations/models.py
--rw-r--r--   0        0        0      783 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/invitations/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/jobs/__init__.py
--rw-r--r--   0        0        0     3174 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/jobs/models.py
--rw-r--r--   0        0        0     1422 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/jobs/repository.py
--rw-r--r--   0        0        0      533 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/jobs/unit_of_work.py
--rw-r--r--   0        0        0      102 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/models.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/recruiters/__init__.py
--rw-r--r--   0        0        0      117 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/recruiters/models.py
--rw-r--r--   0        0        0      741 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/recruiters/repository.py
--rw-r--r--   0        0        0     1353 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/scheduled_events/__init__.py
--rw-r--r--   0        0        0      210 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/scheduled_events/enumerations.py
--rw-r--r--   0        0        0      995 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/scheduled_events/models.py
--rw-r--r--   0        0        0     1862 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/scheduled_events/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/search/__init__.py
--rw-r--r--   0        0        0     1699 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/search/models.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/static/__init__.py
--rw-r--r--   0        0        0     1327 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/static/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/users/cover_letters/__init__.py
--rw-r--r--   0        0        0      277 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/users/cover_letters/models.py
--rw-r--r--   0        0        0      851 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/users/cover_letters/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/users/details/__init__.py
--rw-r--r--   0        0        0     2974 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/users/details/models.py
--rw-r--r--   0        0        0     1419 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/users/details/repository.py
--rw-r--r--   0        0        0     1213 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/users/enumerations.py
--rw-r--r--   0        0        0       89 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/users/models.py
--rw-r--r--   0        0        0     1358 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/users/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/users/resumes/__init__.py
--rw-r--r--   0        0        0      196 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/users/resumes/models.py
--rw-r--r--   0        0        0      797 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/users/resumes/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/users/sessions/__init__.py
--rw-r--r--   0        0        0      481 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/users/sessions/models.py
--rw-r--r--   0        0        0     2607 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/static/__init__.py
--rw-r--r--   0        0        0     1518 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/static/enumerations.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/test_support/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/test_support/fixtures/__init__.py
--rw-r--r--   0        0        0     2116 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/test_support/fixtures/application.py
--rw-r--r--   0        0        0     1684 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/test_support/fixtures/chat.py
--rw-r--r--   0        0        0     1027 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/test_support/fixtures/company.py
--rw-r--r--   0        0        0      382 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/test_support/fixtures/job.py
--rw-r--r--   0        0        0     1843 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/test_support/fixtures/recruiter.py
--rw-r--r--   0        0        0      645 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/test_support/fixtures/recruiter_invitation.py
--rw-r--r--   0        0        0     1706 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/test_support/fixtures/scheduled_events.py
--rw-r--r--   0        0        0     2442 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/test_support/fixtures/users.py
--rw-r--r--   0        0        0      886 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/utils.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/__init__.py
--rw-r--r--   0        0        0      165 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/aiocron.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/algolia/__init__.py
--rw-r--r--   0        0        0      468 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/algolia/client_factory.py
--rw-r--r--   0        0        0     1270 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/algolia/mock.py
--rw-r--r--   0        0        0      758 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/algolia/models.py
--rw-r--r--   0        0        0     1757 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/algolia/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/clerk/__init__.py
--rw-r--r--   0        0        0     2139 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/clerk/client.py
--rw-r--r--   0        0        0      340 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/clerk/client_factory.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/clerk/companies/__init__.py
--rw-r--r--   0        0        0      894 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/clerk/companies/models.py
--rw-r--r--   0        0        0     2694 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/clerk/companies/repository.py
--rw-r--r--   0        0        0     2553 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/clerk/mock.py
--rw-r--r--   0        0        0      413 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/clerk/models.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/clerk/recruiter_invitation/__init__.py
--rw-r--r--   0        0        0      747 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/clerk/recruiter_invitation/models.py
--rw-r--r--   0        0        0     2043 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/clerk/recruiter_invitation/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/clerk/recruiters/__init__.py
--rw-r--r--   0        0        0     1588 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/clerk/recruiters/models.py
--rw-r--r--   0        0        0     2371 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/clerk/recruiters/repository.py
--rw-r--r--   0        0        0     2318 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/clerk/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/clerk/users/__init__.py
--rw-r--r--   0        0        0     1320 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/clerk/users/models.py
--rw-r--r--   0        0        0     2642 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/clerk/users/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/firebase_storage/__init__.py
--rw-r--r--   0        0        0      680 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/firebase_storage/client_factory.py
--rw-r--r--   0        0        0     1102 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/firebase_storage/helpers.py
--rw-r--r--   0        0        0      192 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/firebase_storage/mock.py
--rw-r--r--   0        0        0     1975 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/firebase_storage/models.py
--rw-r--r--   0        0        0     1212 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/firebase_storage/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/firestore/__init__.py
--rw-r--r--   0        0        0      582 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/firestore/client_factory.py
--rw-r--r--   0        0        0     1102 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/firestore/helpers.py
--rw-r--r--   0        0        0      507 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/firestore/mock.py
--rw-r--r--   0        0        0     1975 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/firestore/models.py
--rw-r--r--   0        0        0     9200 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/firestore/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/kafka/__init__.py
--rw-r--r--   0        0        0      725 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/kafka/authentication.py
--rw-r--r--   0        0        0     1369 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/kafka/client_factory.py
--rw-r--r--   0        0        0      320 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/kafka/exceptions.py
--rw-r--r--   0        0        0      716 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/kafka/mock.py
--rw-r--r--   0        0        0     2087 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/kafka/models.py
--rw-r--r--   0        0        0     1517 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/kafka/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/mailgun/__init__.py
--rw-r--r--   0        0        0      989 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/mailgun/client_factory.py
--rw-r--r--   0        0        0      282 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/mailgun/mock.py
--rw-r--r--   0        0        0     1231 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/mailgun/repository.py
--rw-r--r--   0        0        0      104 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/mailgun/templates/chat_message.html
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/openai/__init__.py
--rw-r--r--   0        0        0      443 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/openai/client_factory.py
--rw-r--r--   0        0        0      690 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/openai/mock.py
--rw-r--r--   0        0        0      985 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/openai/repository.py
--rw-r--r--   0        0        0      590 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/openai/settings.py
--rw-r--r--   0        0        0        0 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/redis/__init__.py
--rw-r--r--   0        0        0      502 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/redis/client_factory.py
--rw-r--r--   0        0        0      343 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/redis/mock.py
--rw-r--r--   0        0        0     2451 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/redis/repository.py
--rw-r--r--   0        0        0      251 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/sentry.py
--rw-r--r--   0        0        0     1786 2023-07-26 19:33:33.258794 getajob-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2892 1970-01-01 00:00:00.000000 getajob-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-26 20:03:40.893400 getajob-0.5.1/LICENSE
+-rw-r--r--   0        0        0       69 2023-07-26 20:03:40.897400 getajob-0.5.1/README.md
+-rw-r--r--   0        0        0       22 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/__init__.py
+-rw-r--r--   0        0        0     2927 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/abstractions/models.py
+-rw-r--r--   0        0        0    16351 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/abstractions/repository.py
+-rw-r--r--   0        0        0      385 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/abstractions/vendor_client_factory.py
+-rw-r--r--   0        0        0     2121 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/config/settings.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/admin/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/admin/search/__init__.py
+-rw-r--r--   0        0        0      177 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/admin/search/models.py
+-rw-r--r--   0        0        0      607 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/admin/search/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/admin/users/__init__.py
+-rw-r--r--   0        0        0      620 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/admin/users/models.py
+-rw-r--r--   0        0        0      844 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/admin/users/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/applicant_matching/__init__.py
+-rw-r--r--   0        0        0     1347 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/applicant_matching/models.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/applications/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/applications/applicant_tracking/__init__.py
+-rw-r--r--   0        0        0     1044 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/applications/applicant_tracking/models.py
+-rw-r--r--   0        0        0     2498 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/applications/applicant_tracking/repository.py
+-rw-r--r--   0        0        0      277 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/applications/enumerations.py
+-rw-r--r--   0        0        0      726 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/applications/models.py
+-rw-r--r--   0        0        0     3635 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/applications/repository.py
+-rw-r--r--   0        0        0     2629 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/applications/unit_of_work.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/chat/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/chat/message/__init__.py
+-rw-r--r--   0        0        0      616 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/chat/message/models.py
+-rw-r--r--   0        0        0      889 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/chat/message/repository.py
+-rw-r--r--   0        0        0      272 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/chat/models.py
+-rw-r--r--   0        0        0     1770 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/chat/repository.py
+-rw-r--r--   0        0        0     1650 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/chat/unit_of_work.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/applicant_tracking_settings/__init__.py
+-rw-r--r--   0        0        0      331 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/applicant_tracking_settings/models.py
+-rw-r--r--   0        0        0      817 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/applicant_tracking_settings/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/audit/__init__.py
+-rw-r--r--   0        0        0      482 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/audit/models.py
+-rw-r--r--   0        0        0     1101 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/audit/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/details/__init__.py
+-rw-r--r--   0        0        0      743 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/details/models.py
+-rw-r--r--   0        0        0     1451 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/details/repository.py
+-rw-r--r--   0        0        0     1870 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/enumerations.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/invitations/__init__.py
+-rw-r--r--   0        0        0      145 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/invitations/models.py
+-rw-r--r--   0        0        0      783 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/invitations/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/jobs/__init__.py
+-rw-r--r--   0        0        0     3174 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/jobs/models.py
+-rw-r--r--   0        0        0     1422 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/jobs/repository.py
+-rw-r--r--   0        0        0      533 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/jobs/unit_of_work.py
+-rw-r--r--   0        0        0      102 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/models.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/recruiters/__init__.py
+-rw-r--r--   0        0        0      117 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/recruiters/models.py
+-rw-r--r--   0        0        0      741 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/recruiters/repository.py
+-rw-r--r--   0        0        0     1353 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/scheduled_events/__init__.py
+-rw-r--r--   0        0        0      210 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/scheduled_events/enumerations.py
+-rw-r--r--   0        0        0      995 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/scheduled_events/models.py
+-rw-r--r--   0        0        0     1862 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/scheduled_events/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/search/__init__.py
+-rw-r--r--   0        0        0     1732 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/search/models.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/static/__init__.py
+-rw-r--r--   0        0        0     1327 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/static/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/users/cover_letters/__init__.py
+-rw-r--r--   0        0        0      277 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/users/cover_letters/models.py
+-rw-r--r--   0        0        0      851 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/users/cover_letters/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/users/details/__init__.py
+-rw-r--r--   0        0        0     2974 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/users/details/models.py
+-rw-r--r--   0        0        0     1419 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/users/details/repository.py
+-rw-r--r--   0        0        0     1213 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/users/enumerations.py
+-rw-r--r--   0        0        0       89 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/users/models.py
+-rw-r--r--   0        0        0     1358 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/users/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/users/resumes/__init__.py
+-rw-r--r--   0        0        0      196 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/users/resumes/models.py
+-rw-r--r--   0        0        0      797 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/users/resumes/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/users/sessions/__init__.py
+-rw-r--r--   0        0        0      481 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/users/sessions/models.py
+-rw-r--r--   0        0        0     2607 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/static/__init__.py
+-rw-r--r--   0        0        0     1518 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/static/enumerations.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/test_support/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/test_support/fixtures/__init__.py
+-rw-r--r--   0        0        0     2116 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/test_support/fixtures/application.py
+-rw-r--r--   0        0        0     1684 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/test_support/fixtures/chat.py
+-rw-r--r--   0        0        0     1027 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/test_support/fixtures/company.py
+-rw-r--r--   0        0        0      382 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/test_support/fixtures/job.py
+-rw-r--r--   0        0        0     1843 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/test_support/fixtures/recruiter.py
+-rw-r--r--   0        0        0      645 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/test_support/fixtures/recruiter_invitation.py
+-rw-r--r--   0        0        0     1706 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/test_support/fixtures/scheduled_events.py
+-rw-r--r--   0        0        0     2442 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/test_support/fixtures/users.py
+-rw-r--r--   0        0        0      886 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/utils.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/vendor/__init__.py
+-rw-r--r--   0        0        0      165 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/vendor/aiocron.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/vendor/algolia/__init__.py
+-rw-r--r--   0        0        0      468 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/vendor/algolia/client_factory.py
+-rw-r--r--   0        0        0     1270 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/vendor/algolia/mock.py
+-rw-r--r--   0        0        0      758 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/vendor/algolia/models.py
+-rw-r--r--   0        0        0     1757 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/vendor/algolia/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/vendor/clerk/__init__.py
+-rw-r--r--   0        0        0     2139 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/client.py
+-rw-r--r--   0        0        0      340 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/client_factory.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/companies/__init__.py
+-rw-r--r--   0        0        0      894 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/companies/models.py
+-rw-r--r--   0        0        0     2694 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/companies/repository.py
+-rw-r--r--   0        0        0     2553 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/mock.py
+-rw-r--r--   0        0        0      413 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/models.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/recruiter_invitation/__init__.py
+-rw-r--r--   0        0        0      747 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/recruiter_invitation/models.py
+-rw-r--r--   0        0        0     2043 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/recruiter_invitation/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/recruiters/__init__.py
+-rw-r--r--   0        0        0     1588 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/recruiters/models.py
+-rw-r--r--   0        0        0     2371 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/recruiters/repository.py
+-rw-r--r--   0        0        0     2318 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/users/__init__.py
+-rw-r--r--   0        0        0     1353 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/users/models.py
+-rw-r--r--   0        0        0     2642 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/users/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/firebase_storage/__init__.py
+-rw-r--r--   0        0        0      680 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/firebase_storage/client_factory.py
+-rw-r--r--   0        0        0     1102 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/firebase_storage/helpers.py
+-rw-r--r--   0        0        0      192 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/firebase_storage/mock.py
+-rw-r--r--   0        0        0     1975 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/firebase_storage/models.py
+-rw-r--r--   0        0        0     1212 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/firebase_storage/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/firestore/__init__.py
+-rw-r--r--   0        0        0      582 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/firestore/client_factory.py
+-rw-r--r--   0        0        0     1102 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/firestore/helpers.py
+-rw-r--r--   0        0        0      507 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/firestore/mock.py
+-rw-r--r--   0        0        0     1975 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/firestore/models.py
+-rw-r--r--   0        0        0     9200 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/firestore/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/kafka/__init__.py
+-rw-r--r--   0        0        0      725 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/kafka/authentication.py
+-rw-r--r--   0        0        0     1369 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/kafka/client_factory.py
+-rw-r--r--   0        0        0      320 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/kafka/exceptions.py
+-rw-r--r--   0        0        0      716 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/kafka/mock.py
+-rw-r--r--   0        0        0     2087 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/kafka/models.py
+-rw-r--r--   0        0        0     1517 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/kafka/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/mailgun/__init__.py
+-rw-r--r--   0        0        0      989 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/mailgun/client_factory.py
+-rw-r--r--   0        0        0      282 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/mailgun/mock.py
+-rw-r--r--   0        0        0     1231 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/mailgun/repository.py
+-rw-r--r--   0        0        0      104 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/mailgun/templates/chat_message.html
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/openai/__init__.py
+-rw-r--r--   0        0        0      443 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/openai/client_factory.py
+-rw-r--r--   0        0        0      690 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/openai/mock.py
+-rw-r--r--   0        0        0      985 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/openai/repository.py
+-rw-r--r--   0        0        0      590 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/openai/settings.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/redis/__init__.py
+-rw-r--r--   0        0        0      502 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/redis/client_factory.py
+-rw-r--r--   0        0        0      343 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/redis/mock.py
+-rw-r--r--   0        0        0     2451 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/redis/repository.py
+-rw-r--r--   0        0        0      251 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/sentry.py
+-rw-r--r--   0        0        0     1786 2023-07-26 20:03:40.901399 getajob-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2892 1970-01-01 00:00:00.000000 getajob-0.5.1/PKG-INFO
```

### Comparing `getajob-0.5.0/LICENSE` & `getajob-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/abstractions/models.py` & `getajob-0.5.1/getajob/abstractions/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/abstractions/repository.py` & `getajob-0.5.1/getajob/abstractions/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/config/settings.py` & `getajob-0.5.1/getajob/config/settings.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/admin/search/repository.py` & `getajob-0.5.1/getajob/contexts/admin/search/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/admin/users/models.py` & `getajob-0.5.1/getajob/contexts/admin/users/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/admin/users/repository.py` & `getajob-0.5.1/getajob/contexts/admin/users/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/applicant_matching/models.py` & `getajob-0.5.1/getajob/contexts/applicant_matching/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/applications/applicant_tracking/models.py` & `getajob-0.5.1/getajob/contexts/applications/applicant_tracking/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/applications/applicant_tracking/repository.py` & `getajob-0.5.1/getajob/contexts/applications/applicant_tracking/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/applications/models.py` & `getajob-0.5.1/getajob/contexts/applications/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/applications/repository.py` & `getajob-0.5.1/getajob/contexts/applications/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/applications/unit_of_work.py` & `getajob-0.5.1/getajob/contexts/applications/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/chat/message/models.py` & `getajob-0.5.1/getajob/contexts/chat/message/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/chat/message/repository.py` & `getajob-0.5.1/getajob/contexts/chat/message/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/chat/repository.py` & `getajob-0.5.1/getajob/contexts/chat/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/chat/unit_of_work.py` & `getajob-0.5.1/getajob/contexts/chat/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/companies/applicant_tracking_settings/repository.py` & `getajob-0.5.1/getajob/contexts/companies/applicant_tracking_settings/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/companies/audit/repository.py` & `getajob-0.5.1/getajob/contexts/companies/audit/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/companies/details/models.py` & `getajob-0.5.1/getajob/contexts/companies/details/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/companies/details/repository.py` & `getajob-0.5.1/getajob/contexts/companies/details/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/companies/enumerations.py` & `getajob-0.5.1/getajob/contexts/companies/enumerations.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/companies/invitations/repository.py` & `getajob-0.5.1/getajob/contexts/companies/invitations/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/companies/jobs/models.py` & `getajob-0.5.1/getajob/contexts/companies/jobs/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/companies/jobs/repository.py` & `getajob-0.5.1/getajob/contexts/companies/jobs/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/companies/jobs/unit_of_work.py` & `getajob-0.5.1/getajob/contexts/companies/jobs/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/companies/recruiters/repository.py` & `getajob-0.5.1/getajob/contexts/companies/recruiters/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/companies/repository.py` & `getajob-0.5.1/getajob/contexts/companies/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/scheduled_events/models.py` & `getajob-0.5.1/getajob/contexts/scheduled_events/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/scheduled_events/repository.py` & `getajob-0.5.1/getajob/contexts/scheduled_events/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/search/models.py` & `getajob-0.5.1/getajob/contexts/search/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 
 class CandidateSearch(BaseDataModel):
     """A generic search across all users and their details"""
 
     user: User
     user_details: UserDetails | None = None
+    thumbnail: str | None = None
 
     is_deleted: bool = False  # Soft delete flag
 
 
 class ApplicantSearch(BaseDataModel):
     """
     A Search for within a company to view all applicants for their jobs
```

### Comparing `getajob-0.5.0/getajob/contexts/static/repository.py` & `getajob-0.5.1/getajob/contexts/static/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/users/cover_letters/repository.py` & `getajob-0.5.1/getajob/contexts/users/cover_letters/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/users/details/models.py` & `getajob-0.5.1/getajob/contexts/users/details/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/users/details/repository.py` & `getajob-0.5.1/getajob/contexts/users/details/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/users/enumerations.py` & `getajob-0.5.1/getajob/contexts/users/enumerations.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/users/repository.py` & `getajob-0.5.1/getajob/contexts/users/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/contexts/users/resumes/repository.py` & `getajob-0.5.1/getajob/contexts/users/resumes/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/exceptions.py` & `getajob-0.5.1/getajob/exceptions.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/static/enumerations.py` & `getajob-0.5.1/getajob/static/enumerations.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/test_support/fixtures/application.py` & `getajob-0.5.1/getajob/test_support/fixtures/application.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/test_support/fixtures/chat.py` & `getajob-0.5.1/getajob/test_support/fixtures/chat.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/test_support/fixtures/company.py` & `getajob-0.5.1/getajob/test_support/fixtures/company.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/test_support/fixtures/recruiter.py` & `getajob-0.5.1/getajob/test_support/fixtures/recruiter.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/test_support/fixtures/recruiter_invitation.py` & `getajob-0.5.1/getajob/test_support/fixtures/recruiter_invitation.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/test_support/fixtures/scheduled_events.py` & `getajob-0.5.1/getajob/test_support/fixtures/scheduled_events.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/test_support/fixtures/users.py` & `getajob-0.5.1/getajob/test_support/fixtures/users.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/utils.py` & `getajob-0.5.1/getajob/utils.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/algolia/mock.py` & `getajob-0.5.1/getajob/vendor/algolia/mock.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/algolia/models.py` & `getajob-0.5.1/getajob/vendor/algolia/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/algolia/repository.py` & `getajob-0.5.1/getajob/vendor/algolia/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/clerk/client.py` & `getajob-0.5.1/getajob/vendor/clerk/client.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/clerk/companies/models.py` & `getajob-0.5.1/getajob/vendor/clerk/companies/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/clerk/companies/repository.py` & `getajob-0.5.1/getajob/vendor/clerk/companies/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/clerk/mock.py` & `getajob-0.5.1/getajob/vendor/clerk/mock.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/clerk/recruiter_invitation/models.py` & `getajob-0.5.1/getajob/vendor/clerk/recruiter_invitation/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/clerk/recruiter_invitation/repository.py` & `getajob-0.5.1/getajob/vendor/clerk/recruiter_invitation/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/clerk/recruiters/models.py` & `getajob-0.5.1/getajob/vendor/clerk/recruiters/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/clerk/recruiters/repository.py` & `getajob-0.5.1/getajob/vendor/clerk/recruiters/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/clerk/repository.py` & `getajob-0.5.1/getajob/vendor/clerk/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/clerk/users/models.py` & `getajob-0.5.1/getajob/vendor/clerk/users/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     email_addresses: list[ClerkUserEmailAddresses]
     phone_numbers: list[ClertkUserPhoneNumbers]
     first_name: str
     last_name: str
     gender: str
     external_id: str | None = None
     birthday: str
+    image_url: str | None = None
 
 
 class ClerkWebhookUserUpdated(ClerkBaseModel):
     primary_email_address_id: str | None = None
     email_addresses: list[ClerkUserEmailAddresses] | None = None
     phone_numbers: list[ClertkUserPhoneNumbers] | None = None
     first_name: str | None = None
```

### Comparing `getajob-0.5.0/getajob/vendor/clerk/users/repository.py` & `getajob-0.5.1/getajob/vendor/clerk/users/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/firebase_storage/client_factory.py` & `getajob-0.5.1/getajob/vendor/firebase_storage/client_factory.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/firebase_storage/helpers.py` & `getajob-0.5.1/getajob/vendor/firebase_storage/helpers.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/firebase_storage/models.py` & `getajob-0.5.1/getajob/vendor/firebase_storage/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/firebase_storage/repository.py` & `getajob-0.5.1/getajob/vendor/firebase_storage/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/firestore/client_factory.py` & `getajob-0.5.1/getajob/vendor/firestore/client_factory.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/firestore/helpers.py` & `getajob-0.5.1/getajob/vendor/firestore/helpers.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/firestore/models.py` & `getajob-0.5.1/getajob/vendor/firestore/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/firestore/repository.py` & `getajob-0.5.1/getajob/vendor/firestore/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/kafka/authentication.py` & `getajob-0.5.1/getajob/vendor/kafka/authentication.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/kafka/client_factory.py` & `getajob-0.5.1/getajob/vendor/kafka/client_factory.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/kafka/mock.py` & `getajob-0.5.1/getajob/vendor/kafka/mock.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/kafka/models.py` & `getajob-0.5.1/getajob/vendor/kafka/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/kafka/repository.py` & `getajob-0.5.1/getajob/vendor/kafka/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/mailgun/client_factory.py` & `getajob-0.5.1/getajob/vendor/mailgun/client_factory.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/mailgun/repository.py` & `getajob-0.5.1/getajob/vendor/mailgun/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/openai/mock.py` & `getajob-0.5.1/getajob/vendor/openai/mock.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/openai/repository.py` & `getajob-0.5.1/getajob/vendor/openai/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/openai/settings.py` & `getajob-0.5.1/getajob/vendor/openai/settings.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/getajob/vendor/redis/repository.py` & `getajob-0.5.1/getajob/vendor/redis/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.0/pyproject.toml` & `getajob-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "getajob"
-version = "0.5.0"
+version = "0.5.1"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 aiohttp = "3.8.4"
```

### Comparing `getajob-0.5.0/PKG-INFO` & `getajob-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getajob
-Version: 0.5.0
+Version: 0.5.1
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiocron (>=1.8,<2.0)
```

