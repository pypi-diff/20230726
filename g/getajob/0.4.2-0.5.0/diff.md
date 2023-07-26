# Comparing `tmp/getajob-0.4.2.tar.gz` & `tmp/getajob-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getajob-0.4.2.tar", max compression
+gzip compressed data, was "getajob-0.5.0.tar", max compression
```

## Comparing `getajob-0.4.2.tar` & `getajob-0.5.0.tar`

### file list

```diff
@@ -1,145 +1,152 @@
--rw-r--r--   0        0        0    11357 2023-07-24 01:30:01.795068 getajob-0.4.2/LICENSE
--rw-r--r--   0        0        0       69 2023-07-24 01:30:01.795068 getajob-0.4.2/README.md
--rw-r--r--   0        0        0       22 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/__init__.py
--rw-r--r--   0        0        0     2653 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/abstractions/models.py
--rw-r--r--   0        0        0    15322 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/abstractions/repository.py
--rw-r--r--   0        0        0      385 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/abstractions/vendor_client_factory.py
--rw-r--r--   0        0        0     2034 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/config/settings.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/admin/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/admin/search/__init__.py
--rw-r--r--   0        0        0      177 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/admin/search/models.py
--rw-r--r--   0        0        0      659 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/admin/search/repository.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/admin/users/__init__.py
--rw-r--r--   0        0        0      620 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/admin/users/models.py
--rw-r--r--   0        0        0      803 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/admin/users/repository.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/applications/__init__.py
--rw-r--r--   0        0        0      188 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/applications/enumerations.py
--rw-r--r--   0        0        0      726 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/applications/models.py
--rw-r--r--   0        0        0     3429 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/applications/repository.py
--rw-r--r--   0        0        0     2176 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/applications/unit_of_work.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/chat/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/chat/message/__init__.py
--rw-r--r--   0        0        0      616 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/chat/message/models.py
--rw-r--r--   0        0        0      848 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/chat/message/repository.py
--rw-r--r--   0        0        0      272 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/chat/models.py
--rw-r--r--   0        0        0     1797 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/chat/repository.py
--rw-r--r--   0        0        0     1650 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/chat/unit_of_work.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/companies/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/companies/audit/__init__.py
--rw-r--r--   0        0        0      482 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/companies/audit/models.py
--rw-r--r--   0        0        0     1060 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/companies/audit/repository.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/companies/details/__init__.py
--rw-r--r--   0        0        0      425 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/companies/details/models.py
--rw-r--r--   0        0        0      805 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/companies/details/repository.py
--rw-r--r--   0        0        0     1870 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/companies/enumerations.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/companies/invitations/__init__.py
--rw-r--r--   0        0        0      145 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/companies/invitations/models.py
--rw-r--r--   0        0        0      742 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/companies/invitations/repository.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.795068 getajob-0.4.2/getajob/contexts/companies/jobs/__init__.py
--rw-r--r--   0        0        0     3153 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/companies/jobs/models.py
--rw-r--r--   0        0        0     1357 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/companies/jobs/repository.py
--rw-r--r--   0        0        0      533 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/companies/jobs/unit_of_work.py
--rw-r--r--   0        0        0      102 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/companies/models.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/companies/recruiters/__init__.py
--rw-r--r--   0        0        0      117 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/companies/recruiters/models.py
--rw-r--r--   0        0        0      700 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/companies/recruiters/repository.py
--rw-r--r--   0        0        0      864 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/companies/repository.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/scheduled_events/__init__.py
--rw-r--r--   0        0        0      210 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/scheduled_events/enumerations.py
--rw-r--r--   0        0        0      995 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/scheduled_events/models.py
--rw-r--r--   0        0        0     1821 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/scheduled_events/repository.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/static/__init__.py
--rw-r--r--   0        0        0     1327 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/static/repository.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/users/contact_info/__init__.py
--rw-r--r--   0        0        0      417 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/users/contact_info/models.py
--rw-r--r--   0        0        0      807 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/users/contact_info/repository.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/users/cover_letters/__init__.py
--rw-r--r--   0        0        0      277 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/users/cover_letters/models.py
--rw-r--r--   0        0        0      870 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/users/cover_letters/repository.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/users/demographics/__init__.py
--rw-r--r--   0        0        0      916 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/users/demographics/models.py
--rw-r--r--   0        0        0      861 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/users/demographics/repository.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/users/enumerations.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/users/job_preferences/__init__.py
--rw-r--r--   0        0        0     1653 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/users/job_preferences/models.py
--rw-r--r--   0        0        0      801 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/users/job_preferences/repository.py
--rw-r--r--   0        0        0       89 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/users/models.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/users/qualifications/__init__.py
--rw-r--r--   0        0        0     2592 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/users/qualifications/models.py
--rw-r--r--   0        0        0      860 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/users/qualifications/repository.py
--rw-r--r--   0        0        0      937 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/users/repository.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/users/resumes/__init__.py
--rw-r--r--   0        0        0      196 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/users/resumes/models.py
--rw-r--r--   0        0        0      816 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/users/resumes/repository.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/users/sessions/__init__.py
--rw-r--r--   0        0        0      481 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/contexts/users/sessions/models.py
--rw-r--r--   0        0        0     2607 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/static/__init__.py
--rw-r--r--   0        0        0      362 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/static/enumerations.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/test_support/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/test_support/fixtures/__init__.py
--rw-r--r--   0        0        0     2116 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/test_support/fixtures/application.py
--rw-r--r--   0        0        0     1684 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/test_support/fixtures/chat.py
--rw-r--r--   0        0        0     1027 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/test_support/fixtures/company.py
--rw-r--r--   0        0        0      382 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/test_support/fixtures/job.py
--rw-r--r--   0        0        0     1843 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/test_support/fixtures/recruiter.py
--rw-r--r--   0        0        0      645 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/test_support/fixtures/recruiter_invitation.py
--rw-r--r--   0        0        0     1706 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/test_support/fixtures/scheduled_events.py
--rw-r--r--   0        0        0     2442 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/test_support/fixtures/users.py
--rw-r--r--   0        0        0      594 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/utils.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/__init__.py
--rw-r--r--   0        0        0      165 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/aiocron.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/algolia/__init__.py
--rw-r--r--   0        0        0      468 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/algolia/client_factory.py
--rw-r--r--   0        0        0     1258 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/algolia/mock.py
--rw-r--r--   0        0        0      702 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/algolia/models.py
--rw-r--r--   0        0        0     1545 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/algolia/repository.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/clerk/__init__.py
--rw-r--r--   0        0        0     2139 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/clerk/client.py
--rw-r--r--   0        0        0      340 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/clerk/client_factory.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/clerk/companies/__init__.py
--rw-r--r--   0        0        0      894 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/clerk/companies/models.py
--rw-r--r--   0        0        0     2110 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/clerk/companies/repository.py
--rw-r--r--   0        0        0     2553 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/clerk/mock.py
--rw-r--r--   0        0        0      413 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/clerk/models.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/clerk/recruiter_invitation/__init__.py
--rw-r--r--   0        0        0      747 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/clerk/recruiter_invitation/models.py
--rw-r--r--   0        0        0     2043 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/clerk/recruiter_invitation/repository.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/clerk/recruiters/__init__.py
--rw-r--r--   0        0        0     1588 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/clerk/recruiters/models.py
--rw-r--r--   0        0        0     2371 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/clerk/recruiters/repository.py
--rw-r--r--   0        0        0     2318 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/clerk/repository.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/clerk/users/__init__.py
--rw-r--r--   0        0        0     1320 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/clerk/users/models.py
--rw-r--r--   0        0        0     2101 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/clerk/users/repository.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/firestore/__init__.py
--rw-r--r--   0        0        0      582 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/firestore/client_factory.py
--rw-r--r--   0        0        0     1102 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/firestore/helpers.py
--rw-r--r--   0        0        0      507 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/firestore/mock.py
--rw-r--r--   0        0        0     1975 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/firestore/models.py
--rw-r--r--   0        0        0     9100 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/firestore/repository.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/kafka/__init__.py
--rw-r--r--   0        0        0      725 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/kafka/authentication.py
--rw-r--r--   0        0        0     1369 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/kafka/client_factory.py
--rw-r--r--   0        0        0      320 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/kafka/exceptions.py
--rw-r--r--   0        0        0      716 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/kafka/mock.py
--rw-r--r--   0        0        0     1853 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/kafka/models.py
--rw-r--r--   0        0        0     1517 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/kafka/repository.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/mailgun/__init__.py
--rw-r--r--   0        0        0      989 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/mailgun/client_factory.py
--rw-r--r--   0        0        0      282 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/mailgun/mock.py
--rw-r--r--   0        0        0     1231 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/mailgun/repository.py
--rw-r--r--   0        0        0      104 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/mailgun/templates/chat_message.html
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/openai/__init__.py
--rw-r--r--   0        0        0      443 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/openai/client_factory.py
--rw-r--r--   0        0        0      690 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/openai/mock.py
--rw-r--r--   0        0        0      985 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/openai/repository.py
--rw-r--r--   0        0        0      590 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/openai/settings.py
--rw-r--r--   0        0        0        0 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/redis/__init__.py
--rw-r--r--   0        0        0      502 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/redis/client_factory.py
--rw-r--r--   0        0        0      343 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/redis/mock.py
--rw-r--r--   0        0        0     2129 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/redis/repository.py
--rw-r--r--   0        0        0      251 2023-07-24 01:30:01.799068 getajob-0.4.2/getajob/vendor/sentry.py
--rw-r--r--   0        0        0     1786 2023-07-24 01:30:01.803068 getajob-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     2892 1970-01-01 00:00:00.000000 getajob-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-26 19:33:33.250794 getajob-0.5.0/LICENSE
+-rw-r--r--   0        0        0       69 2023-07-26 19:33:33.250794 getajob-0.5.0/README.md
+-rw-r--r--   0        0        0       22 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/__init__.py
+-rw-r--r--   0        0        0     2927 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/abstractions/models.py
+-rw-r--r--   0        0        0    16351 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/abstractions/repository.py
+-rw-r--r--   0        0        0      385 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/abstractions/vendor_client_factory.py
+-rw-r--r--   0        0        0     2121 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/config/settings.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/contexts/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/contexts/admin/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/contexts/admin/search/__init__.py
+-rw-r--r--   0        0        0      177 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/contexts/admin/search/models.py
+-rw-r--r--   0        0        0      607 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/contexts/admin/search/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/contexts/admin/users/__init__.py
+-rw-r--r--   0        0        0      620 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/contexts/admin/users/models.py
+-rw-r--r--   0        0        0      844 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/contexts/admin/users/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/contexts/applicant_matching/__init__.py
+-rw-r--r--   0        0        0     1347 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/contexts/applicant_matching/models.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/contexts/applications/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/contexts/applications/applicant_tracking/__init__.py
+-rw-r--r--   0        0        0     1044 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/contexts/applications/applicant_tracking/models.py
+-rw-r--r--   0        0        0     2498 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/contexts/applications/applicant_tracking/repository.py
+-rw-r--r--   0        0        0      277 2023-07-26 19:33:33.250794 getajob-0.5.0/getajob/contexts/applications/enumerations.py
+-rw-r--r--   0        0        0      726 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/applications/models.py
+-rw-r--r--   0        0        0     3635 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/applications/repository.py
+-rw-r--r--   0        0        0     2629 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/applications/unit_of_work.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/chat/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/chat/message/__init__.py
+-rw-r--r--   0        0        0      616 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/chat/message/models.py
+-rw-r--r--   0        0        0      889 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/chat/message/repository.py
+-rw-r--r--   0        0        0      272 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/chat/models.py
+-rw-r--r--   0        0        0     1770 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/chat/repository.py
+-rw-r--r--   0        0        0     1650 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/chat/unit_of_work.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/applicant_tracking_settings/__init__.py
+-rw-r--r--   0        0        0      331 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/applicant_tracking_settings/models.py
+-rw-r--r--   0        0        0      817 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/applicant_tracking_settings/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/audit/__init__.py
+-rw-r--r--   0        0        0      482 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/audit/models.py
+-rw-r--r--   0        0        0     1101 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/audit/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/details/__init__.py
+-rw-r--r--   0        0        0      743 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/details/models.py
+-rw-r--r--   0        0        0     1451 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/details/repository.py
+-rw-r--r--   0        0        0     1870 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/enumerations.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/invitations/__init__.py
+-rw-r--r--   0        0        0      145 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/invitations/models.py
+-rw-r--r--   0        0        0      783 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/invitations/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/jobs/__init__.py
+-rw-r--r--   0        0        0     3174 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/jobs/models.py
+-rw-r--r--   0        0        0     1422 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/jobs/repository.py
+-rw-r--r--   0        0        0      533 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/jobs/unit_of_work.py
+-rw-r--r--   0        0        0      102 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/models.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/recruiters/__init__.py
+-rw-r--r--   0        0        0      117 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/recruiters/models.py
+-rw-r--r--   0        0        0      741 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/recruiters/repository.py
+-rw-r--r--   0        0        0     1353 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/companies/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/scheduled_events/__init__.py
+-rw-r--r--   0        0        0      210 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/scheduled_events/enumerations.py
+-rw-r--r--   0        0        0      995 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/scheduled_events/models.py
+-rw-r--r--   0        0        0     1862 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/scheduled_events/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/search/__init__.py
+-rw-r--r--   0        0        0     1699 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/search/models.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/static/__init__.py
+-rw-r--r--   0        0        0     1327 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/static/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/users/cover_letters/__init__.py
+-rw-r--r--   0        0        0      277 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/users/cover_letters/models.py
+-rw-r--r--   0        0        0      851 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/users/cover_letters/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/users/details/__init__.py
+-rw-r--r--   0        0        0     2974 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/users/details/models.py
+-rw-r--r--   0        0        0     1419 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/users/details/repository.py
+-rw-r--r--   0        0        0     1213 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/users/enumerations.py
+-rw-r--r--   0        0        0       89 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/users/models.py
+-rw-r--r--   0        0        0     1358 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/users/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/users/resumes/__init__.py
+-rw-r--r--   0        0        0      196 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/users/resumes/models.py
+-rw-r--r--   0        0        0      797 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/users/resumes/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/users/sessions/__init__.py
+-rw-r--r--   0        0        0      481 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/contexts/users/sessions/models.py
+-rw-r--r--   0        0        0     2607 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/static/__init__.py
+-rw-r--r--   0        0        0     1518 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/static/enumerations.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/test_support/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/test_support/fixtures/__init__.py
+-rw-r--r--   0        0        0     2116 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/test_support/fixtures/application.py
+-rw-r--r--   0        0        0     1684 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/test_support/fixtures/chat.py
+-rw-r--r--   0        0        0     1027 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/test_support/fixtures/company.py
+-rw-r--r--   0        0        0      382 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/test_support/fixtures/job.py
+-rw-r--r--   0        0        0     1843 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/test_support/fixtures/recruiter.py
+-rw-r--r--   0        0        0      645 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/test_support/fixtures/recruiter_invitation.py
+-rw-r--r--   0        0        0     1706 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/test_support/fixtures/scheduled_events.py
+-rw-r--r--   0        0        0     2442 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/test_support/fixtures/users.py
+-rw-r--r--   0        0        0      886 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/utils.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/__init__.py
+-rw-r--r--   0        0        0      165 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/aiocron.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/algolia/__init__.py
+-rw-r--r--   0        0        0      468 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/algolia/client_factory.py
+-rw-r--r--   0        0        0     1270 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/algolia/mock.py
+-rw-r--r--   0        0        0      758 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/algolia/models.py
+-rw-r--r--   0        0        0     1757 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/algolia/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/clerk/__init__.py
+-rw-r--r--   0        0        0     2139 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/clerk/client.py
+-rw-r--r--   0        0        0      340 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/clerk/client_factory.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/clerk/companies/__init__.py
+-rw-r--r--   0        0        0      894 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/clerk/companies/models.py
+-rw-r--r--   0        0        0     2694 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/clerk/companies/repository.py
+-rw-r--r--   0        0        0     2553 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/clerk/mock.py
+-rw-r--r--   0        0        0      413 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/clerk/models.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.254794 getajob-0.5.0/getajob/vendor/clerk/recruiter_invitation/__init__.py
+-rw-r--r--   0        0        0      747 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/clerk/recruiter_invitation/models.py
+-rw-r--r--   0        0        0     2043 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/clerk/recruiter_invitation/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/clerk/recruiters/__init__.py
+-rw-r--r--   0        0        0     1588 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/clerk/recruiters/models.py
+-rw-r--r--   0        0        0     2371 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/clerk/recruiters/repository.py
+-rw-r--r--   0        0        0     2318 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/clerk/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/clerk/users/__init__.py
+-rw-r--r--   0        0        0     1320 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/clerk/users/models.py
+-rw-r--r--   0        0        0     2642 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/clerk/users/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/firebase_storage/__init__.py
+-rw-r--r--   0        0        0      680 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/firebase_storage/client_factory.py
+-rw-r--r--   0        0        0     1102 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/firebase_storage/helpers.py
+-rw-r--r--   0        0        0      192 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/firebase_storage/mock.py
+-rw-r--r--   0        0        0     1975 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/firebase_storage/models.py
+-rw-r--r--   0        0        0     1212 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/firebase_storage/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/firestore/__init__.py
+-rw-r--r--   0        0        0      582 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/firestore/client_factory.py
+-rw-r--r--   0        0        0     1102 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/firestore/helpers.py
+-rw-r--r--   0        0        0      507 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/firestore/mock.py
+-rw-r--r--   0        0        0     1975 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/firestore/models.py
+-rw-r--r--   0        0        0     9200 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/firestore/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/kafka/__init__.py
+-rw-r--r--   0        0        0      725 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/kafka/authentication.py
+-rw-r--r--   0        0        0     1369 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/kafka/client_factory.py
+-rw-r--r--   0        0        0      320 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/kafka/exceptions.py
+-rw-r--r--   0        0        0      716 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/kafka/mock.py
+-rw-r--r--   0        0        0     2087 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/kafka/models.py
+-rw-r--r--   0        0        0     1517 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/kafka/repository.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/mailgun/__init__.py
+-rw-r--r--   0        0        0      989 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/mailgun/client_factory.py
+-rw-r--r--   0        0        0      282 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/mailgun/mock.py
+-rw-r--r--   0        0        0     1231 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/mailgun/repository.py
+-rw-r--r--   0        0        0      104 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/mailgun/templates/chat_message.html
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/openai/__init__.py
+-rw-r--r--   0        0        0      443 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/openai/client_factory.py
+-rw-r--r--   0        0        0      690 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/openai/mock.py
+-rw-r--r--   0        0        0      985 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/openai/repository.py
+-rw-r--r--   0        0        0      590 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/openai/settings.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/redis/__init__.py
+-rw-r--r--   0        0        0      502 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/redis/client_factory.py
+-rw-r--r--   0        0        0      343 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/redis/mock.py
+-rw-r--r--   0        0        0     2451 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/redis/repository.py
+-rw-r--r--   0        0        0      251 2023-07-26 19:33:33.258794 getajob-0.5.0/getajob/vendor/sentry.py
+-rw-r--r--   0        0        0     1786 2023-07-26 19:33:33.258794 getajob-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2892 1970-01-01 00:00:00.000000 getajob-0.5.0/PKG-INFO
```

### Comparing `getajob-0.4.2/LICENSE` & `getajob-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/abstractions/models.py` & `getajob-0.5.0/getajob/abstractions/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from pydantic import BaseModel
 
 from getajob.config.settings import SETTINGS
 from getajob.vendor.firestore.repository import FirestoreDB
 from getajob.vendor.kafka.repository import KafkaProducerRepository
 from getajob.vendor.kafka.models import KafkaEventConfig
+from getajob.vendor.redis.repository import RedisRepository
 
 
 DataSchema = t.Type[BaseModel]
 
 
 @dataclass
 class PaginatedRequest:
@@ -56,50 +57,58 @@
     CHAT_MESSAGES = "chat_messages"
     ADMIN_USERS = "admin_users"
     SKILLS = "skills"
     COVER_LETTERS = "cover_letters"
     RESUMES = "resumes"
     COMPANIES = "companies"  # Comes from clerk
     COMPANY_DETAILS = "company_details"  # What we add to company data
+    COMPANY_ATS_CONFIG = "company_ats_config"
     COMPANY_AUDITS = "company_audits"
     RECRUITERS = "recruiters"  # Comes from clerk
     RECRUITER_INVITATIONS = "recruiter_invitations"  # Comes from clerk
     RECRUITER_DETAILS = "recruiter_details"  # What we add to recruiter data
     JOBS = "jobs"
     APPLICATIONS = "applications"
+    APPLICATION_TRACKING = "application_tracking"
     USER_NOTIFICATIONS = "user_notifications"
     SCHEDULED_EVENTS = "scheduled_events"
 
-    # Child collections
-    USER_CONTACT_INFORMATION = "user_contact_information"
-    USER_DEMOGRAPHICS = "user_demographics"
-    USER_JOB_PREFERENCES = "user_job_preferences"
-    USER_QUALIFICATIONS = "user_qualifications"
-
 
 class Location(BaseModel):
     address_line_1: str
     address_line_2: str | None = None
     city: str
     state: str
     zipcode: str
     country: str
     lat: float
     lon: float
 
 
-@dataclass
-class RepositoryDependencies:
+class RepositoryDependencies(BaseModel):
     user_id: str
     db: FirestoreDB
     collection_name: str
     entity_models: EntityModels
     kafka: t.Optional[KafkaProducerRepository] = None
     kafka_event_config: t.Optional[KafkaEventConfig] = None
+    redis: t.Optional[RedisRepository] = None
 
+    class Config:
+        arbitrary_types_allowed = True
 
-@dataclass
-class UserAndDatabaseConnection:
+
+class UserAndDatabaseConnection(BaseModel):
     """Created during a request"""
 
     initiating_user_id: str
     db: FirestoreDB
+
+    class Config:
+        arbitrary_types_allowed = True
+
+
+class ProcessedKafkaMessage(BaseModel):
+    request_scope: UserAndDatabaseConnection
+    object_id: str
+    parent_collections: dict
+    data: BaseModel | dict[str, t.Any] | None
```

### Comparing `getajob-0.4.2/getajob/abstractions/repository.py` & `getajob-0.5.0/getajob/abstractions/repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typing as t
 from datetime import datetime
 from functools import wraps
 from pydantic import BaseModel
 
 from getajob.abstractions.models import BaseDataModel
-from getajob.utils import generate_random_short_code
+from getajob.utils import generate_random_short_code, get_value_from_enum
 from getajob.exceptions import (
     KafkaEventTopicNotProvidedError,
     EntityNotFound,
     MissingParentKeyError,
 )
 from getajob.vendor.firestore.models import (
     FirestoreDocument,
@@ -104,25 +104,14 @@
         filters=filters,
         order_by=order_by,
         pagination=pagination,
     )
     return format_paginated_response(res, entity_model)
 
 
-# def query_subcollection(
-#     db: FirestoreDB,
-#     collection_name: str,
-#     entity_model: t.Optional[t.Type[BaseModel]] = None,
-#     filters: t.Optional[t.List[FirestoreFilters]] = None,
-#     order_by: t.Optional[FirestoreOrderBy] = None,
-#     pagination: FirestorePagination = FirestorePagination(),
-# ):
-#     res = db.q
-
-
 class BaseRepository:
     """
     This is the base repository layer that sites between a context's repository and the database.
     It's purpose is to provide basic query function with a conversion to pydantic models.
 
     It also handles the relationship between collections and sub-collections and can
     be given a Kafka client and configuration to create event streams based on CRUD operations.
@@ -166,24 +155,26 @@
     def _produce_repository_kafka_event(
         self,
         event_type: KafkaEventType,
         object_id: str,
         parent_collections: dict = {},
         data: dict | None = None,
     ):
-        if (
-            not self.kafka
-            or not self.kafka_event_config
-            or not self.kafka_event_config.dict()[event_type]
-        ):
+        if not self.kafka or not self.kafka_event_config:
+            return
+        event_enum = get_value_from_enum(
+            value=event_type.value, 
+            enumeration=self.kafka_event_config.message_type_enum
+        )
+        if not event_enum:
             return
         self.kafka.publish(
             topic=self.kafka_event_config.topic,
             message=BaseKafkaMessage(
-                message_type=f"{event_type.value}_{self.collection_name}",
+                message_type=event_enum.value,
                 requesting_user_id=self.requesting_user_id,
                 object_id=object_id,
                 parent_collections=parent_collections,
                 data=data if data else None,
             ),
         )
 
@@ -432,30 +423,63 @@
     """
     This class extends the base repository is meant for interacting with a
     sub-collection of a root level document where there can be only one sub
     collection of the same type.
 
     An example is a company's details, which there can only be one of
     directly under the company
+
+    This repository includes additional handling for cacheing data. I expect
+    that this type of data is better suited for cacheing that the multiple
+    child or parent classes above.
     """
 
     def __init__(
         self, dependencies: RepositoryDependencies, required_parent_keys: t.List[str]
     ):
         self.dependencies = dependencies
         self.repo = BaseRepository(dependencies)
         self.required_parent_keys = required_parent_keys
+        self.redis = dependencies.redis
+
+    def _get_cached_data(self, parent_collections: dict):
+        if not self.redis:
+            return None
+        return self.redis.get(
+            entity_type=self.dependencies.collection_name,
+            entity_id=self.dependencies.collection_name,
+            parent_collections=parent_collections,
+            model=self.dependencies.entity_models.entity,
+        )
+
+    def _set_cached_data(self, parent_collections: dict, data: BaseModel):
+        if not self.redis:
+            return None
+        self.redis.set(
+            entity_type=self.dependencies.collection_name,
+            entity_id=self.dependencies.collection_name,
+            parent_collections=parent_collections,
+            data=data,
+        )
 
     @ensure_parent_keys
     def get_sub_entity(self, parent_collections: dict):
-        return self.repo.get(self.dependencies.collection_name, parent_collections)
+        cached_result = self._get_cached_data(parent_collections)
+        if cached_result:
+            return cached_result
+        result = self.repo.get(self.dependencies.collection_name, parent_collections)
+        if result:
+            self._set_cached_data(parent_collections, result)
+        return result
 
     @ensure_parent_keys
     def set_sub_entity(self, data: BaseModel, parent_collections: dict):
         try:
-            return self.repo.update(
+            result = self.repo.update(
                 self.dependencies.collection_name, data, parent_collections
             )
         except EntityNotFound:
-            return self.repo.create(
+            result = self.repo.create(
                 data, parent_collections, self.dependencies.collection_name
             )
+        self._set_cached_data(parent_collections, result)
+        return result
```

### Comparing `getajob-0.4.2/getajob/config/settings.py` & `getajob-0.5.0/getajob/config/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,29 +7,30 @@
 
 class AppSettings:
     # General
     APP_VERSION: str = os.getenv("APP_VERSION", "0.0.0")
 
     # Firebase config
     FIRESTORE_JSON_CONFIG: str = os.getenv("FIRESTORE_JSON_CONFIG", "")
+    FIREBASE_FILE_STORAGE_BUCKET: str = os.getenv("FIREBASE_FILE_STORAGE_BUCKET", "")
 
     # Openai config
     OPENAI_API_KEY: str = os.getenv("OPENAI_API_KEY", "")
     OPENAI_MOCK_RESPONSES: str = os.getenv("OPENAI_MOCK_RESPONSES", "false")
     OPENAI_MODEL_ABILITY: int = 1
 
     # Clerk config
     CLERK_JWT_PEM_KEY: str = os.getenv("CLERK_JWT_PEM_KEY", "").replace(r"\n", "\n")
     CLERK_TOKEN_LEEWAY: int = int(os.getenv("CLERK_TOKEN_LEEWAY", "3600"))
     CLERK_USER_WEBHOOK_SECRET: str = os.getenv("CLERK_USER_WEBHOOK_SECRET", "")
     CLERK_SECRET_KEY: str = os.getenv("CLERK_SECRET_KEY", "")
 
     DEFAULT_PAGE_LIMIT: int = 20
 
-    LOCAL_TESTING: bool = get_bool_from_string(os.getenv("LOCAL_TESTING", "true"))
+    LOCAL_TESTING: bool = get_bool_from_string(os.getenv("LOCAL_TESTING", "false"))
     ENABLED_KAFKA_EVENTS: bool = get_bool_from_string(
         os.getenv("ENABLED_KAFKA_EVENTS", "false")
     )
 
     # Algolia config
     ALGOLA_APP_ID: str = os.getenv("ALGOLA_APP_ID", "")
     ALGOLIA_API_KEY: str = os.getenv("ALGOLIA_API_KEY", "")
```

### Comparing `getajob-0.4.2/getajob/contexts/admin/search/repository.py` & `getajob-0.5.0/getajob/contexts/admin/search/repository.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,11 +6,10 @@
 
 class AdminSearchRepository:
     def __init__(self, request_scope: UserAndDatabaseConnection):
         self.db = request_scope.db
 
     def admin_collection_search(self, search: AdminEntitySearch):
         return query_collection(db=self.db, collection_name=search.entity_type.value)
-    
+
     def admin_subcollection_search(self, search: AdminEntitySearch):
-        # TODO add subcollection query again...
         return query_collection(db=self.db, collection_name=search.entity_type.value)
```

### Comparing `getajob-0.4.2/getajob/contexts/admin/users/models.py` & `getajob-0.5.0/getajob/contexts/admin/users/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/contexts/admin/users/repository.py` & `getajob-0.5.0/getajob/contexts/admin/users/repository.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 )
 
 
 class AdminUserRepository(ParentRepository):
     def __init__(self, request_scope: UserAndDatabaseConnection):
         super().__init__(
             RepositoryDependencies(
-                request_scope.initiating_user_id,
-                request_scope.db,
-                Entity.ADMIN_USERS.value,
-                entity_models,
+                user_id=request_scope.initiating_user_id,
+                db=request_scope.db,
+                collection_name=Entity.ADMIN_USERS.value,
+                entity_models=entity_models,
             )
         )
 
     def get_by_user_id(self, user_id: str):
         return self.get_one_by_attribute("user_id", user_id)
```

### Comparing `getajob-0.4.2/getajob/contexts/applications/models.py` & `getajob-0.5.0/getajob/contexts/applications/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/contexts/applications/repository.py` & `getajob-0.5.0/getajob/contexts/applications/repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 import typing as t
 
 from getajob.abstractions.models import Entity
 from getajob.abstractions.repository import ParentRepository, RepositoryDependencies
 from getajob.vendor.firestore.models import FirestoreFilters
 from getajob.abstractions.models import UserAndDatabaseConnection
 from getajob.vendor.kafka.repository import KafkaProducerRepository
-from getajob.vendor.kafka.models import KafkaEventConfig, KafkaTopic
+from getajob.vendor.kafka.models import (
+    KafkaEventConfig,
+    KafkaTopic,
+    KafkaApplicationsEnum,
+)
 from getajob.contexts.users.resumes.repository import ResumeRepository
 from getajob.contexts.companies.jobs.repository import JobsRepository
+from getajob.contexts.applications.applicant_tracking.repository import ATSRepository
 
 from .models import entity_models, UserCreatedApplication
 from .unit_of_work import ApplicationsUnitOfWork
 
 
 class ApplicationRepository(ParentRepository):
     def __init__(
         self,
         request_scope: UserAndDatabaseConnection,
         kafka: t.Optional[KafkaProducerRepository] = None,
     ):
         self.request_scope = request_scope
         kafka_event_config = KafkaEventConfig(
-            topic=KafkaTopic.applications,
-            create=True,
-            update=True,
-            delete=True,
-            get=True,
+            topic=KafkaTopic.applications, message_type_enum=KafkaApplicationsEnum
         )
         super().__init__(
             RepositoryDependencies(
-                request_scope.initiating_user_id,
-                request_scope.db,
-                Entity.APPLICATIONS.value,
-                entity_models,
-                kafka,
-                kafka_event_config,
+                user_id=request_scope.initiating_user_id,
+                db=request_scope.db,
+                collection_name=Entity.APPLICATIONS.value,
+                entity_models=entity_models,
+                kafka=kafka,
+                kafka_event_config=kafka_event_config,
             ),
         )
 
     def user_creates_application(
         self, user_id: str, application: UserCreatedApplication
     ):
         return ApplicationsUnitOfWork(self).user_creates_application(
             user_id=user_id,
             resume_repo=ResumeRepository(self.request_scope),
             job_repo=JobsRepository(self.request_scope),
+            applicant_tracking_repo=ATSRepository(self.request_scope),
             create_application=application,
         )
 
     def get_applications_by_company(self, company_id: str):
         return super().query(
             filters=[
                 FirestoreFilters(field="company_id", operator="==", value=company_id),
```

### Comparing `getajob-0.4.2/getajob/contexts/applications/unit_of_work.py` & `getajob-0.5.0/getajob/contexts/applications/unit_of_work.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import typing as t
 from fastapi import HTTPException
 
 from getajob.abstractions.models import Entity
-from getajob.abstractions.repository import BaseRepository
+from getajob.abstractions.repository import BaseRepository, SingleChildRepository
 from getajob.contexts.companies.jobs.models import Job
+from getajob.contexts.applications.applicant_tracking.models import SetATSDetails
 from getajob.vendor.firestore.models import FirestoreFilters
 
 from .models import UserCreatedApplication, CreateApplication
 
 
 class ApplicationsUnitOfWork:
     def __init__(self, application_repo: BaseRepository):
         self.application_repo = application_repo
 
     def user_creates_application(
         self,
         user_id: str,
         resume_repo: BaseRepository,
         job_repo: BaseRepository,
+        applicant_tracking_repo: SingleChildRepository,
         create_application: UserCreatedApplication,
     ):
         # Check that the company and job is still viable
         job = t.cast(
             Job,
             job_repo.get(
                 create_application.job_id,
@@ -50,15 +52,24 @@
         # Check that resume exists
         assert resume_repo.get(
             parent_collections={Entity.USERS.value: user_id},
             doc_id=create_application.resume_id,
         )
 
         # Create the application
-        return self.application_repo.create(
+        application = self.application_repo.create(
             data=CreateApplication(
                 user_id=user_id,
                 job_id=create_application.job_id,
                 resume_id=create_application.resume_id,
                 company_id=create_application.company_id,
             )
         )
+
+        # Create the default application tracking details
+        applicant_tracking_repo.set_sub_entity(
+            data=SetATSDetails(),
+            parent_collections={
+                Entity.APPLICATIONS.value: application.id,
+            },
+        )
+        return application
```

### Comparing `getajob-0.4.2/getajob/contexts/chat/message/models.py` & `getajob-0.5.0/getajob/contexts/chat/message/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/contexts/chat/message/repository.py` & `getajob-0.5.0/getajob/contexts/chat/message/repository.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 )
 
 
 class ChatMessageRepository(MultipleChildrenRepository):
     def __init__(self, request_scope: UserAndDatabaseConnection):
         super().__init__(
             RepositoryDependencies(
-                request_scope.initiating_user_id,
-                request_scope.db,
-                Entity.CHAT_MESSAGES.value,
-                entity_models,
+                user_id=request_scope.initiating_user_id,
+                db=request_scope.db,
+                collection_name=Entity.CHAT_MESSAGES.value,
+                entity_models=entity_models,
             ),
             required_parent_keys=[Entity.CHAT.value],
         )
```

### Comparing `getajob-0.4.2/getajob/contexts/chat/repository.py` & `getajob-0.5.0/getajob/contexts/chat/repository.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 entity_models = EntityModels(entity=Chat, create=UserCreateChat)
 
 
 class ChatRepository(ParentRepository):
     def __init__(self, request_scope: UserAndDatabaseConnection):
         super().__init__(
             RepositoryDependencies(
-                request_scope.initiating_user_id,
-                request_scope.db,
-                Entity.CHAT.value,
-                entity_models,
+                user_id=request_scope.initiating_user_id,
+                db=request_scope.db,
+                collection_name=Entity.CHAT.value,
+                entity_models=entity_models,
             )
         )
         self.request_scope = request_scope
 
     def create_new_chat(self, create_chat: UserCreateChat):
         return CreateChatUnitOfWork(
             application_repository=ApplicationRepository(self.request_scope),
@@ -35,13 +35,9 @@
             user_repository=UserRepository(self.request_scope),
             chat_repository=self,
         ).create_new_chat(create_chat)
 
     def get_all_chats_user_is_part_of(self, user_id: str, is_recruiter: bool = False):
         query_field = "recruiter_user_id" if is_recruiter else "applicant_user_id"
         return self.query(
-            filters=[
-                FirestoreFilters(
-                    field=query_field, operator="==", value=user_id
-                )
-            ]
+            filters=[FirestoreFilters(field=query_field, operator="==", value=user_id)]
         )
```

### Comparing `getajob-0.4.2/getajob/contexts/chat/unit_of_work.py` & `getajob-0.5.0/getajob/contexts/chat/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/contexts/companies/audit/repository.py` & `getajob-0.5.0/getajob/contexts/companies/audit/repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 entity_models = EntityModels(create=CreateAuditLog, entity=AuditLog)
 
 
 class AuditLogRepository(MultipleChildrenRepository):
     def __init__(self, request_scope: UserAndDatabaseConnection):
         super().__init__(
             RepositoryDependencies(
-                request_scope.initiating_user_id,
-                request_scope.db,
-                Entity.COMPANY_AUDITS.value,
-                entity_models,
+                user_id=request_scope.initiating_user_id,
+                db=request_scope.db,
+                collection_name=Entity.COMPANY_AUDITS.value,
+                entity_models=entity_models,
             ),
             [Entity.COMPANIES.value],
         )
 
     def update(self, *args, **kwargs):
         raise NotImplementedError("Audit logs cannot be updated")
```

### Comparing `getajob-0.4.2/getajob/contexts/companies/details/repository.py` & `getajob-0.5.0/getajob/contexts/companies/applicant_tracking_settings/repository.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from getajob.abstractions.repository import (
     SingleChildRepository,
     RepositoryDependencies,
 )
 from getajob.abstractions.models import Entity, EntityModels, UserAndDatabaseConnection
 
-from .models import CreateCompanyDetails, CompanyDetails
+from .models import SetATSConfig, ATSConfig
 
 entity_models = EntityModels(
-    create=CreateCompanyDetails,
-    update=CreateCompanyDetails,
-    entity=CompanyDetails,
+    create=SetATSConfig,
+    update=SetATSConfig,
+    entity=ATSConfig,
 )
 
 
-class CompanyDetailsRepository(SingleChildRepository):
+class CompanyATSConfigRepository(SingleChildRepository):
     def __init__(self, request_scope: UserAndDatabaseConnection):
         super().__init__(
             RepositoryDependencies(
-                request_scope.initiating_user_id,
-                request_scope.db,
-                Entity.COMPANY_DETAILS.value,
-                entity_models,
+                user_id=request_scope.initiating_user_id,
+                db=request_scope.db,
+                collection_name=Entity.COMPANY_ATS_CONFIG.value,
+                entity_models=entity_models,
             ),
             required_parent_keys=[Entity.COMPANIES.value],
         )
```

### Comparing `getajob-0.4.2/getajob/contexts/companies/enumerations.py` & `getajob-0.5.0/getajob/contexts/companies/enumerations.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/contexts/companies/invitations/repository.py` & `getajob-0.5.0/getajob/contexts/companies/invitations/repository.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 entity_models = EntityModels(entity=RecruiterInvitation)
 
 
 class RecruiterInvitationsRepository(MultipleChildrenRepository):
     def __init__(self, request_scope: UserAndDatabaseConnection):
         super().__init__(
             RepositoryDependencies(
-                request_scope.initiating_user_id,
-                request_scope.db,
-                Entity.RECRUITER_INVITATIONS.value,
-                entity_models,
+                user_id=request_scope.initiating_user_id,
+                db=request_scope.db,
+                collection_name=Entity.RECRUITER_INVITATIONS.value,
+                entity_models=entity_models,
             ),
             required_parent_keys=[Entity.COMPANIES.value],
         )
```

### Comparing `getajob-0.4.2/getajob/contexts/companies/jobs/models.py` & `getajob-0.5.0/getajob/contexts/companies/jobs/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import typing as t
 from pydantic import BaseModel
 
 from getajob.abstractions.models import Location, BaseDataModel
-from getajob.static.enumerations import LangaugeOptions
+from getajob.static.enumerations import LanguageEnum
 
 from ..enumerations import (
     PayType,
     ScheduleType,
     ExperienceLevel,
     JobLocationType,
     ResumeRequirement,
@@ -76,28 +76,30 @@
     on_job_training_offered: bool | None = None
 
     weekly_day_range: t.List[WeeklyScheduleType] | None = None
     shift_type: t.List[ShiftType] | None = None
 
     pay: Pay | None = None
 
-    language_requirements: t.List[LangaugeOptions] | None = None
+    language_requirements: t.List[LanguageEnum] | None = None
 
     background_check_required: bool | None = None
     drug_test_required: bool | None = None
     felons_accepted: bool | None = None
     disability_accepted: bool | None = None
 
     ideal_days_to_hire: int | None = None
     internal_reference_code: str | None = None
     job_associated_company_description: str | None = None
 
     application_settings: ApplicationSettings | None = None
     application_questions: t.List[ApplicationQuestion] | None = None
 
+    is_live: bool = False
+
 
 class CreateJob(UserCreateJob):
     view_count: int = 0
 
 
 class UpdateJob(UserCreateJob):
     position_title: str | None = None  # type: ignore
```

### Comparing `getajob-0.4.2/getajob/contexts/companies/jobs/repository.py` & `getajob-0.5.0/getajob/contexts/companies/jobs/repository.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typing as t
 from getajob.vendor.kafka.repository import KafkaProducerRepository
-from getajob.vendor.kafka.models import KafkaEventConfig, KafkaTopic
+from getajob.vendor.kafka.models import KafkaEventConfig, KafkaTopic, KafkaJobsEnum
 from getajob.abstractions.repository import (
     MultipleChildrenRepository,
     RepositoryDependencies,
 )
 from getajob.abstractions.models import Entity, EntityModels, UserAndDatabaseConnection
 
 from .models import CreateJob, UpdateJob, Job, UserCreateJob
@@ -17,23 +17,23 @@
 class JobsRepository(MultipleChildrenRepository):
     def __init__(
         self,
         request_scope: UserAndDatabaseConnection,
         kafka: t.Optional[KafkaProducerRepository] = None,
     ):
         kafka_event_config = KafkaEventConfig(
-            topic=KafkaTopic.jobs, create=True, update=True, delete=True, get=True
+            topic=KafkaTopic.jobs, message_type_enum=KafkaJobsEnum
         )
         super().__init__(
             RepositoryDependencies(
-                request_scope.initiating_user_id,
-                request_scope.db,
-                Entity.JOBS.value,
-                entity_models,
-                kafka,
-                kafka_event_config,
+                user_id=request_scope.initiating_user_id,
+                db=request_scope.db,
+                collection_name=Entity.JOBS.value,
+                entity_models=entity_models,
+                kafka=kafka,
+                kafka_event_config=kafka_event_config,
             ),
             required_parent_keys=[Entity.COMPANIES.value],
         )
 
     def create_job(self, company_id: str, job: UserCreateJob):
         return JobsUnitOfWork(self).create_job(company_id, job)
```

### Comparing `getajob-0.4.2/getajob/contexts/companies/jobs/unit_of_work.py` & `getajob-0.5.0/getajob/contexts/companies/jobs/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/contexts/companies/recruiters/repository.py` & `getajob-0.5.0/getajob/contexts/companies/recruiters/repository.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 entity_models = EntityModels(entity=Recruiter)
 
 
 class RecruiterRepository(MultipleChildrenRepository):
     def __init__(self, request_scope: UserAndDatabaseConnection):
         super().__init__(
             RepositoryDependencies(
-                request_scope.initiating_user_id,
-                request_scope.db,
-                Entity.RECRUITERS.value,
-                entity_models,
+                user_id=request_scope.initiating_user_id,
+                db=request_scope.db,
+                collection_name=Entity.RECRUITERS.value,
+                entity_models=entity_models,
             ),
             required_parent_keys=[Entity.COMPANIES.value],
         )
```

### Comparing `getajob-0.4.2/getajob/contexts/companies/repository.py` & `getajob-0.5.0/getajob/contexts/companies/repository.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,35 @@
 from getajob.vendor.firestore.models import FirestoreFilters
 from getajob.abstractions.repository import ParentRepository, RepositoryDependencies
 from getajob.abstractions.models import Entity, EntityModels, UserAndDatabaseConnection
+from getajob.vendor.kafka.models import KafkaEventConfig, KafkaTopic, KafkaCompanyEnum
+from getajob.vendor.kafka.repository import KafkaProducerRepository
 
 from .models import Company
 
 entity_models = EntityModels(entity=Company)
 
 
 class CompanyRepository(ParentRepository):
-    def __init__(self, request_scope: UserAndDatabaseConnection):
+    def __init__(
+        self,
+        request_scope: UserAndDatabaseConnection,
+        kafka: KafkaProducerRepository | None = None,
+    ):
+        kafka_event_config = KafkaEventConfig(
+            topic=KafkaTopic.companies, message_type_enum=KafkaCompanyEnum
+        )
         super().__init__(
             RepositoryDependencies(
-                request_scope.initiating_user_id,
-                request_scope.db,
-                Entity.COMPANIES.value,
-                entity_models,
+                user_id=request_scope.initiating_user_id,
+                db=request_scope.db,
+                collection_name=Entity.COMPANIES.value,
+                entity_models=entity_models,
+                kafka=kafka,
+                kafka_event_config=kafka_event_config,
             )
         )
 
     def get_companies_by_company_id_list(self, company_id_list: list[str]):
         return self.query(
             filters=[FirestoreFilters(field="id", operator="in", value=company_id_list)]
         )
```

### Comparing `getajob-0.4.2/getajob/contexts/scheduled_events/models.py` & `getajob-0.5.0/getajob/contexts/scheduled_events/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/contexts/scheduled_events/repository.py` & `getajob-0.5.0/getajob/contexts/scheduled_events/repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 )
 
 
 class ScheduledEventsRepository(ParentRepository):
     def __init__(self, request_scope: UserAndDatabaseConnection):
         super().__init__(
             RepositoryDependencies(
-                request_scope.initiating_user_id,
-                request_scope.db,
-                Entity.SCHEDULED_EVENTS.value,
-                entity_models,
+                user_id=request_scope.initiating_user_id,
+                db=request_scope.db,
+                collection_name=Entity.SCHEDULED_EVENTS.value,
+                entity_models=entity_models,
             )
         )
 
     def create_scheduled_event(self, data: CreateScheduledEvent):
         data.next_run_time = data.calculate_next_invocation()
         return super().create(data)
```

### Comparing `getajob-0.4.2/getajob/contexts/static/repository.py` & `getajob-0.5.0/getajob/contexts/static/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/contexts/users/contact_info/repository.py` & `getajob-0.5.0/getajob/contexts/users/resumes/repository.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 from getajob.abstractions.repository import (
-    SingleChildRepository,
+    MultipleChildrenRepository,
     RepositoryDependencies,
 )
 from getajob.abstractions.models import Entity, EntityModels, UserAndDatabaseConnection
 
-from .models import (
-    UserContactInformation,
-    ContactInformation,
-)
+from .models import Resume, CreateResume
 
 
 entity_models = EntityModels(
-    entity=UserContactInformation,
-    create=ContactInformation,
+    entity=Resume,
+    create=CreateResume,
+    update=CreateResume,
 )
 
 
-class ContactInformationRepository(SingleChildRepository):
+class ResumeRepository(MultipleChildrenRepository):
     def __init__(self, request_scope: UserAndDatabaseConnection):
         super().__init__(
             RepositoryDependencies(
-                request_scope.initiating_user_id,
-                request_scope.db,
-                Entity.USER_CONTACT_INFORMATION.value,
-                entity_models,
+                user_id=request_scope.initiating_user_id,
+                db=request_scope.db,
+                collection_name=Entity.RESUMES.value,
+                entity_models=entity_models,
             ),
             required_parent_keys=[Entity.USERS.value],
         )
```

### Comparing `getajob-0.4.2/getajob/contexts/users/qualifications/repository.py` & `getajob-0.5.0/getajob/contexts/users/cover_letters/repository.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-from getajob.vendor.firestore.repository import FirestoreDB
 from getajob.abstractions.repository import (
-    SingleChildRepository,
+    MultipleChildrenRepository,
     RepositoryDependencies,
 )
 from getajob.abstractions.models import Entity, EntityModels, UserAndDatabaseConnection
 
-from .models import Qualifications, UserQualifications
-
+from .models import CoverLetter, CreateCoverLetter, UpdateCoverLetter
 
 entity_models = EntityModels(
-    entity=UserQualifications,
-    create=Qualifications,
-    update=Qualifications,
+    entity=CoverLetter,
+    create=CreateCoverLetter,
+    update=UpdateCoverLetter,
 )
 
 
-class UserQualificationsRepository(SingleChildRepository):
+class CoverLetterRepository(MultipleChildrenRepository):
     def __init__(self, request_scope: UserAndDatabaseConnection):
         super().__init__(
             RepositoryDependencies(
-                request_scope.initiating_user_id,
-                request_scope.db,
-                Entity.USER_QUALIFICATIONS.value,
-                entity_models,
+                user_id=request_scope.initiating_user_id,
+                db=request_scope.db,
+                collection_name=Entity.COVER_LETTERS.value,
+                entity_models=entity_models,
             ),
             required_parent_keys=[Entity.USERS.value],
         )
```

### Comparing `getajob-0.4.2/getajob/exceptions.py` & `getajob-0.5.0/getajob/exceptions.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/test_support/fixtures/application.py` & `getajob-0.5.0/getajob/test_support/fixtures/application.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/test_support/fixtures/chat.py` & `getajob-0.5.0/getajob/test_support/fixtures/chat.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/test_support/fixtures/company.py` & `getajob-0.5.0/getajob/test_support/fixtures/company.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/test_support/fixtures/recruiter.py` & `getajob-0.5.0/getajob/test_support/fixtures/recruiter.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/test_support/fixtures/recruiter_invitation.py` & `getajob-0.5.0/getajob/test_support/fixtures/recruiter_invitation.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/test_support/fixtures/scheduled_events.py` & `getajob-0.5.0/getajob/test_support/fixtures/scheduled_events.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/test_support/fixtures/users.py` & `getajob-0.5.0/getajob/test_support/fixtures/users.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/vendor/algolia/mock.py` & `getajob-0.5.0/getajob/vendor/algolia/mock.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,24 +16,24 @@
             hitsPerPage=0,
             processingTimeMS=0,
             exhaustiveNbHits=False,
             query="",
             params="",
         ).dict()
 
-    def get_object(self, object_id: str, *args):
+    def get_object(self, object_id: str, request_options=None):
         return self.local_items[object_id]
 
-    def save_object(self, object_data: dict, *args):
-        self.local_items[object_data["objectID"]] = object_data
+    def save_object(self, obj: dict, request_options=None):
+        self.local_items[obj["objectID"]] = obj
 
-    def partial_update_object(self, object_data: dict, *args):
-        self.local_items[object_data["objectID"]] = object_data
+    def partial_update_object(self, obj: dict, request_options=None):
+        self.local_items[obj["objectID"]] = obj
 
-    def delete_object(self, object_id: str, *args):
+    def delete_object(self, object_id: str, request_options=None):
         del self.local_items[object_id]
 
 
 class MockAlgoliaClient(SearchClient):
     # pylint: disable=super-init-not-called
     def __init__(self, *args, **kwargs):
         ...
```

### Comparing `getajob-0.4.2/getajob/vendor/algolia/models.py` & `getajob-0.5.0/getajob/vendor/algolia/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 from pydantic import BaseModel
 
 
 class AlgoliaIndex(str, Enum):
     job_search = "job_search"
     company_search = "company_search"
     candidate_search = "candidate_search"
+    applicant_search = "applicant_search"
 
 
 class AlgoliaSearchParams(BaseModel):
-    query: str
+    query: str | None = None
     filters: Optional[str] = None
     facet_filters: Optional[str] = None
     attributes_to_retrieve: Optional[str] = None
     page: int = 0
     hits_per_page: int = 10
```

### Comparing `getajob-0.4.2/getajob/vendor/algolia/repository.py` & `getajob-0.5.0/getajob/vendor/algolia/repository.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,9 +34,13 @@
         object_data["objectID"] = object_id
         return self.index.save_object(object_data)
 
     def update_object(self, object_id: str, object_data: dict):
         object_data["objectID"] = object_id
         return self.index.partial_update_object(object_data)
 
-    def delete_object(self, object_id: str):
-        return self.index.delete_object(object_id)
+    def replace_all_objects(self, objects: list[dict]):
+        return self.index.replace_all_objects(objects)
+
+    # For now we are using soft delete for these search databases so this method is unavailable
+    # def delete_object(self, object_id: str):
+    #     return self.index.delete_object(object_id)
```

### Comparing `getajob-0.4.2/getajob/vendor/clerk/client.py` & `getajob-0.5.0/getajob/vendor/clerk/client.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/vendor/clerk/companies/models.py` & `getajob-0.5.0/getajob/vendor/clerk/companies/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/vendor/clerk/companies/repository.py` & `getajob-0.5.0/getajob/vendor/clerk/companies/repository.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import typing as t
 
 from getajob.vendor.kafka.repository import KafkaProducerRepository
-from getajob.vendor.kafka.models import KafkaEventConfig, KafkaTopic
+from getajob.vendor.kafka.models import KafkaEventConfig, KafkaTopic, KafkaCompanyEnum
 from getajob.abstractions.repository import ParentRepository, RepositoryDependencies
 from getajob.abstractions.models import Entity, EntityModels, UserAndDatabaseConnection
+from getajob.contexts.companies.details.models import SetCompanyDetails
+from getajob.contexts.companies.details.repository import CompanyDetailsRepository
 
 from .models import (
     ClerkCompanyWebhookEvent,
     ClerkCompany,
     ClerkCompanyDeleted,
     ClerkCompanyWebhookType,
 )
@@ -18,41 +20,47 @@
 class WebhookCompanyRepository(ParentRepository):
     def __init__(
         self,
         request_scope: UserAndDatabaseConnection,
         kafka: t.Optional[KafkaProducerRepository] = None,
     ):
         kafka_event_config = KafkaEventConfig(
-            topic=KafkaTopic.companies,
-            create=True,
-            update=True,
-            delete=True,
+            topic=KafkaTopic.companies, message_type_enum=KafkaCompanyEnum
         )
+        self.request_scope = request_scope
         super().__init__(
             RepositoryDependencies(
-                request_scope.initiating_user_id,
-                request_scope.db,
-                Entity.COMPANIES.value,
-                entity_models,
-                kafka,
-                kafka_event_config,
+                user_id=request_scope.initiating_user_id,
+                db=request_scope.db,
+                collection_name=Entity.COMPANIES.value,
+                entity_models=entity_models,
+                kafka=kafka,
+                kafka_event_config=kafka_event_config,
             )
         )
 
     def handle_webhook_event(self, event: ClerkCompanyWebhookEvent):
         event_dict = {
             ClerkCompanyWebhookType.organization_created: self.create_company,
             ClerkCompanyWebhookType.organization_updated: self.update_company,
             ClerkCompanyWebhookType.organization_deleted: self.delete_company,
         }
         return event_dict[event.type](event)
 
+    def _create_default_company_details(self, company_id: str):
+        CompanyDetailsRepository(self.request_scope).set_sub_entity(
+            data=SetCompanyDetails(),
+            parent_collections={Entity.COMPANIES.value: company_id},
+        )
+
     def create_company(self, event: ClerkCompanyWebhookEvent):
         create_event = ClerkCompany(**event.data)
-        return self.create(data=create_event, provided_id=create_event.id)
+        res = self.create(data=create_event, provided_id=create_event.id)
+        self._create_default_company_details(company_id=create_event.id)
+        return res
 
     def delete_company(self, event: ClerkCompanyWebhookEvent):
         delete_event = ClerkCompanyDeleted(**event.data)
         return self.delete(doc_id=delete_event.id)
 
     def update_company(self, event: ClerkCompanyWebhookEvent):
         update_event = ClerkCompany(**event.data)
```

### Comparing `getajob-0.4.2/getajob/vendor/clerk/mock.py` & `getajob-0.5.0/getajob/vendor/clerk/mock.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/vendor/clerk/recruiter_invitation/models.py` & `getajob-0.5.0/getajob/vendor/clerk/recruiter_invitation/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/vendor/clerk/recruiter_invitation/repository.py` & `getajob-0.5.0/getajob/vendor/clerk/recruiter_invitation/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/vendor/clerk/recruiters/models.py` & `getajob-0.5.0/getajob/vendor/clerk/recruiters/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/vendor/clerk/recruiters/repository.py` & `getajob-0.5.0/getajob/vendor/clerk/recruiters/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/vendor/clerk/repository.py` & `getajob-0.5.0/getajob/vendor/clerk/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/vendor/clerk/users/models.py` & `getajob-0.5.0/getajob/vendor/clerk/users/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/vendor/clerk/users/repository.py` & `getajob-0.5.0/getajob/vendor/clerk/users/repository.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import typing as t
 
 from getajob.vendor.kafka.repository import KafkaProducerRepository
-from getajob.vendor.kafka.models import KafkaEventConfig, KafkaTopic
+from getajob.vendor.kafka.models import KafkaEventConfig, KafkaTopic, KafkaUsersEnum
 from getajob.abstractions.repository import ParentRepository, RepositoryDependencies
 from getajob.abstractions.models import Entity, EntityModels, UserAndDatabaseConnection
+from getajob.contexts.users.details.repository import UserDetailsRepository
+from getajob.contexts.users.details.models import SetUserDetails
 
 from .models import (
     ClerkUser,
     ClerkUserWebhookEvent,
     ClerkUserWebhookType,
     ClerkWebhookUserDeleted,
     ClerkWebhookUserUpdated,
@@ -19,41 +21,47 @@
 class WebhookUserRepository(ParentRepository):
     def __init__(
         self,
         request_scope: UserAndDatabaseConnection,
         kafka: t.Optional[KafkaProducerRepository] = None,
     ):
         kafka_event_config = KafkaEventConfig(
-            topic=KafkaTopic.users,
-            create=True,
-            update=True,
-            delete=True,
+            topic=KafkaTopic.users, message_type_enum=KafkaUsersEnum
         )
+        self.request_scope = request_scope
         super().__init__(
             RepositoryDependencies(
-                request_scope.initiating_user_id,
-                request_scope.db,
-                Entity.USERS.value,
-                entity_models,
-                kafka,
-                kafka_event_config,
+                user_id=request_scope.initiating_user_id,
+                db=request_scope.db,
+                collection_name=Entity.USERS.value,
+                entity_models=entity_models,
+                kafka=kafka,
+                kafka_event_config=kafka_event_config,
             )
         )
 
     def handle_webhook_event(self, event: ClerkUserWebhookEvent):
         event_dict = {
             ClerkUserWebhookType.user_created: self.create_user,
             ClerkUserWebhookType.user_updated: self.update_user,
             ClerkUserWebhookType.user_deleted: self.delete_user,
         }
         return event_dict[event.type](event)
 
+    def _create_default_user_details(self, user_id: str):
+        UserDetailsRepository(self.request_scope).set_sub_entity(
+            data=SetUserDetails(),
+            parent_collections={Entity.USERS.value: user_id},
+        )
+
     def create_user(self, event: ClerkUserWebhookEvent):
         create_event = ClerkUser(**event.data)
-        return self.create(data=create_event, provided_id=create_event.id)
+        res = self.create(data=create_event, provided_id=create_event.id)
+        self._create_default_user_details(user_id=create_event.id)
+        return res
 
     def update_user(self, event: ClerkUserWebhookEvent):
         update_event = ClerkWebhookUserUpdated(**event.data)
         return self.update(doc_id=update_event.id, data=update_event)
 
     def delete_user(self, event: ClerkUserWebhookEvent):
         delete_event = ClerkWebhookUserDeleted(**event.data)
```

### Comparing `getajob-0.4.2/getajob/vendor/firestore/client_factory.py` & `getajob-0.5.0/getajob/vendor/firestore/client_factory.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/vendor/firestore/helpers.py` & `getajob-0.5.0/getajob/vendor/firebase_storage/helpers.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/vendor/firestore/models.py` & `getajob-0.5.0/getajob/vendor/firebase_storage/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/vendor/firestore/repository.py` & `getajob-0.5.0/getajob/vendor/firestore/repository.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,17 @@
     FirestoreBatchActionType,
     GetWithJoins,
     QueryWithJoins,
 )
 
 
 class FirestoreDB:
-    def __init__(self, client: Client = FirestoreClientFactory.get_client()):
+    def __init__(
+        self, client: Client | MockFirestoreClient = FirestoreClientFactory.get_client()
+    ):
         self._client = client
 
     def disconnect(self):
         self._client.close()
 
     def _reset_mock(self):
         if isinstance(self._client, MockFirestoreClient):
@@ -178,28 +180,28 @@
         batch = self._client.batch()
         for write in writes:
             if write.action == FirestoreBatchActionType.CREATE:
                 collection_ref = self._get_collection_ref(
                     write.parent_collections, write.collection_name
                 )
                 doc_ref = collection_ref.document(write.document_id)
-                batch.set(doc_ref, write.document_data)
+                batch.set(doc_ref, write.document_data)  # type: ignore
             elif write.action == FirestoreBatchActionType.UPDATE:
                 collection_ref = self._get_collection_ref(
                     write.parent_collections, write.collection_name
                 )
                 doc_ref = collection_ref.document(write.document_id)
-                batch.update(doc_ref, write.document_data)
+                batch.update(doc_ref, write.document_data)  # type: ignore
             elif write.action == FirestoreBatchActionType.DELETE:
                 collection_ref = self._get_collection_ref(
                     write.parent_collections, write.collection_name
                 )
                 doc_ref = collection_ref.document(write.document_id)
-                batch.delete(doc_ref)
-        return batch.commit()
+                batch.delete(doc_ref)  # type: ignore
+        return batch.commit()  # type: ignore
 
     def get_with_joins(self, join_model: GetWithJoins) -> FirestoreDocument:
         """
         This is limited to single depth
         """
         res = self.get(
             join_model.parent_collections, join_model.get_collection, join_model.get_id
```

### Comparing `getajob-0.4.2/getajob/vendor/kafka/authentication.py` & `getajob-0.5.0/getajob/vendor/kafka/authentication.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/vendor/kafka/client_factory.py` & `getajob-0.5.0/getajob/vendor/kafka/client_factory.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/vendor/kafka/mock.py` & `getajob-0.5.0/getajob/vendor/kafka/mock.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/vendor/kafka/repository.py` & `getajob-0.5.0/getajob/vendor/kafka/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/vendor/mailgun/client_factory.py` & `getajob-0.5.0/getajob/vendor/mailgun/client_factory.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/vendor/mailgun/repository.py` & `getajob-0.5.0/getajob/vendor/mailgun/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/vendor/openai/mock.py` & `getajob-0.5.0/getajob/vendor/openai/mock.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/vendor/openai/repository.py` & `getajob-0.5.0/getajob/vendor/openai/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/vendor/openai/settings.py` & `getajob-0.5.0/getajob/vendor/openai/settings.py`

 * *Files identical despite different names*

### Comparing `getajob-0.4.2/getajob/vendor/redis/repository.py` & `getajob-0.5.0/getajob/vendor/redis/repository.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import json
 from typing import Type
 from pydantic import BaseModel
 from redis import Redis
 
-from getajob.abstractions.models import Entity
-
 from .client_factory import RedisFactory
 
 
 class RedisRepository:
     def __init__(self, client: Redis = RedisFactory.get_client()):
         self.client = client
 
-    def _get_cached_id(self, entity: Entity, entity_id: str) -> str:
-        return f"{entity.value}:{entity_id}"
+    def _get_cached_id(
+        self, entity_type: str, entity_id: str, parent_collections: dict
+    ) -> str:
+        redis_key = ""
+        for key, val in parent_collections.items():
+            redis_key += f"{key}:{val}:"
+        redis_key += f"{entity_type}:{entity_id}"
+        return redis_key
 
     def _convert_to_json(
         self, data: str | int | BaseModel | dict | list[BaseModel] | list[dict]
     ) -> str | int:
         if isinstance(
             data,
             (
@@ -37,28 +41,36 @@
                     object_as_list_of_dicts.append(item.dict())
                 else:
                     object_as_list_of_dicts.append(item)
         return json.dumps(object_as_list_of_dicts)
 
     def set(
         self,
-        entity: Entity,
+        entity_type: str,
         entity_id: str,
+        parent_collections: dict,
         data: str | int | BaseModel | dict | list[BaseModel] | list[dict] | None,
     ):
         if not data:
             return
         self.client.set(
-            self._get_cached_id(entity, entity_id), self._convert_to_json(data)
+            self._get_cached_id(entity_type, entity_id, parent_collections),
+            self._convert_to_json(data),
         )
 
     def get(
-        self, entity: Entity, entity_id: str, model: Type[BaseModel] | None = None
+        self,
+        entity_type: str,
+        entity_id: str,
+        parent_collections: dict,
+        model: Type[BaseModel] | None = None,
     ) -> BaseModel | dict | str | int | list | None:
-        res = self.client.get(self._get_cached_id(entity, entity_id))
+        res = self.client.get(
+            self._get_cached_id(entity_type, entity_id, parent_collections)
+        )
         if not res:
             return None
         if isinstance(res, int):
             return res
         try:
             loaded_res = json.loads(res)
         except json.decoder.JSONDecodeError:
```

### Comparing `getajob-0.4.2/pyproject.toml` & `getajob-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "getajob"
-version = "0.4.2"
+version = "0.5.0"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 aiohttp = "3.8.4"
```

### Comparing `getajob-0.4.2/PKG-INFO` & `getajob-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getajob
-Version: 0.4.2
+Version: 0.5.0
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiocron (>=1.8,<2.0)
```

