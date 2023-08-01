# Comparing `tmp/feedancy-0.1.4.tar.gz` & `tmp/feedancy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feedancy-0.1.4.tar", max compression
+gzip compressed data, was "feedancy-0.1.5.tar", max compression
```

## Comparing `feedancy-0.1.4.tar` & `feedancy-0.1.5.tar`

### file list

```diff
@@ -1,139 +1,139 @@
--rw-r--r--   0        0        0      615 2023-07-24 11:54:07.532272 feedancy-0.1.4/README.md
--rw-r--r--   0        0        0      126 2023-07-24 11:54:07.528272 feedancy-0.1.4/feedancy/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 11:54:07.456270 feedancy-0.1.4/feedancy/apis/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 11:54:07.456270 feedancy-0.1.4/feedancy/apis/api/__init__.py
--rw-r--r--   0        0        0    13072 2023-07-24 11:54:07.460270 feedancy-0.1.4/feedancy/apis/api/api.py
--rw-r--r--   0        0        0      896 2023-07-24 11:54:07.472271 feedancy-0.1.4/feedancy/apis/api/api_v1_activitysphere_create.py
--rw-r--r--   0        0        0      820 2023-07-24 11:54:07.476271 feedancy-0.1.4/feedancy/apis/api/api_v1_activitysphere_destroy.py
--rw-r--r--   0        0        0      853 2023-07-24 11:54:07.472271 feedancy-0.1.4/feedancy/apis/api/api_v1_activitysphere_retrieve.py
--rw-r--r--   0        0        0      908 2023-07-24 11:54:07.472271 feedancy-0.1.4/feedancy/apis/api/api_v1_activitysphere_retrieve_2.py
--rw-r--r--   0        0        0      950 2023-07-24 11:54:07.472271 feedancy-0.1.4/feedancy/apis/api/api_v1_activitysphere_update.py
--rw-r--r--   0        0        0      863 2023-07-24 11:54:07.476271 feedancy-0.1.4/feedancy/apis/api/api_v1_city_create.py
--rw-r--r--   0        0        0      810 2023-07-24 11:54:07.476271 feedancy-0.1.4/feedancy/apis/api/api_v1_city_destroy.py
--rw-r--r--   0        0        0      830 2023-07-24 11:54:07.476271 feedancy-0.1.4/feedancy/apis/api/api_v1_city_retrieve.py
--rw-r--r--   0        0        0      885 2023-07-24 11:54:07.476271 feedancy-0.1.4/feedancy/apis/api/api_v1_city_retrieve_2.py
--rw-r--r--   0        0        0      917 2023-07-24 11:54:07.476271 feedancy-0.1.4/feedancy/apis/api/api_v1_city_update.py
--rw-r--r--   0        0        0     1258 2023-07-24 11:54:07.476271 feedancy-0.1.4/feedancy/apis/api/api_v1_company_create.py
--rw-r--r--   0        0        0      813 2023-07-24 11:54:07.480271 feedancy-0.1.4/feedancy/apis/api/api_v1_company_destroy.py
--rw-r--r--   0        0        0     1222 2023-07-24 11:54:07.476271 feedancy-0.1.4/feedancy/apis/api/api_v1_company_retrieve.py
--rw-r--r--   0        0        0     1277 2023-07-24 11:54:07.476271 feedancy-0.1.4/feedancy/apis/api/api_v1_company_retrieve_2.py
--rw-r--r--   0        0        0     1312 2023-07-24 11:54:07.480271 feedancy-0.1.4/feedancy/apis/api/api_v1_company_update.py
--rw-r--r--   0        0        0      899 2023-07-24 11:54:07.480271 feedancy-0.1.4/feedancy/apis/api/api_v1_companycity_create.py
--rw-r--r--   0        0        0      817 2023-07-24 11:54:07.480271 feedancy-0.1.4/feedancy/apis/api/api_v1_companycity_destroy.py
--rw-r--r--   0        0        0      859 2023-07-24 11:54:07.480271 feedancy-0.1.4/feedancy/apis/api/api_v1_companycity_retrieve.py
--rw-r--r--   0        0        0      914 2023-07-24 11:54:07.480271 feedancy-0.1.4/feedancy/apis/api/api_v1_companycity_retrieve_2.py
--rw-r--r--   0        0        0      953 2023-07-24 11:54:07.480271 feedancy-0.1.4/feedancy/apis/api/api_v1_companycity_update.py
--rw-r--r--   0        0        0      935 2023-07-24 11:54:07.480271 feedancy-0.1.4/feedancy/apis/api/api_v1_contact_create.py
--rw-r--r--   0        0        0      813 2023-07-24 11:54:07.484271 feedancy-0.1.4/feedancy/apis/api/api_v1_contact_destroy.py
--rw-r--r--   0        0        0      899 2023-07-24 11:54:07.480271 feedancy-0.1.4/feedancy/apis/api/api_v1_contact_retrieve.py
--rw-r--r--   0        0        0      954 2023-07-24 11:54:07.480271 feedancy-0.1.4/feedancy/apis/api/api_v1_contact_retrieve_2.py
--rw-r--r--   0        0        0      989 2023-07-24 11:54:07.484271 feedancy-0.1.4/feedancy/apis/api/api_v1_contact_update.py
--rw-r--r--   0        0        0      876 2023-07-24 11:54:07.484271 feedancy-0.1.4/feedancy/apis/api/api_v1_country_create.py
--rw-r--r--   0        0        0      813 2023-07-24 11:54:07.484271 feedancy-0.1.4/feedancy/apis/api/api_v1_country_destroy.py
--rw-r--r--   0        0        0      840 2023-07-24 11:54:07.484271 feedancy-0.1.4/feedancy/apis/api/api_v1_country_retrieve.py
--rw-r--r--   0        0        0      895 2023-07-24 11:54:07.484271 feedancy-0.1.4/feedancy/apis/api/api_v1_country_retrieve_2.py
--rw-r--r--   0        0        0      930 2023-07-24 11:54:07.484271 feedancy-0.1.4/feedancy/apis/api/api_v1_country_update.py
--rw-r--r--   0        0        0      881 2023-07-24 11:54:07.484271 feedancy-0.1.4/feedancy/apis/api/api_v1_currency_create.py
--rw-r--r--   0        0        0      814 2023-07-24 11:54:07.484271 feedancy-0.1.4/feedancy/apis/api/api_v1_currency_destroy.py
--rw-r--r--   0        0        0      844 2023-07-24 11:54:07.484271 feedancy-0.1.4/feedancy/apis/api/api_v1_currency_retrieve.py
--rw-r--r--   0        0        0      899 2023-07-24 11:54:07.484271 feedancy-0.1.4/feedancy/apis/api/api_v1_currency_retrieve_2.py
--rw-r--r--   0        0        0      935 2023-07-24 11:54:07.484271 feedancy-0.1.4/feedancy/apis/api/api_v1_currency_update.py
--rw-r--r--   0        0        0     1922 2023-07-24 11:54:07.488271 feedancy-0.1.4/feedancy/apis/api/api_v1_internship_create.py
--rw-r--r--   0        0        0     1941 2023-07-24 11:54:07.492271 feedancy-0.1.4/feedancy/apis/api/api_v1_internship_destroy.py
--rw-r--r--   0        0        0     1883 2023-07-24 11:54:07.488271 feedancy-0.1.4/feedancy/apis/api/api_v1_internship_retrieve.py
--rw-r--r--   0        0        0     1938 2023-07-24 11:54:07.488271 feedancy-0.1.4/feedancy/apis/api/api_v1_internship_retrieve_2.py
--rw-r--r--   0        0        0     1976 2023-07-24 11:54:07.492271 feedancy-0.1.4/feedancy/apis/api/api_v1_internship_update.py
--rw-r--r--   0        0        0      917 2023-07-24 11:54:07.492271 feedancy-0.1.4/feedancy/apis/api/api_v1_internshipcity_create.py
--rw-r--r--   0        0        0      820 2023-07-24 11:54:07.492271 feedancy-0.1.4/feedancy/apis/api/api_v1_internshipcity_destroy.py
--rw-r--r--   0        0        0      874 2023-07-24 11:54:07.492271 feedancy-0.1.4/feedancy/apis/api/api_v1_internshipcity_retrieve.py
--rw-r--r--   0        0        0      929 2023-07-24 11:54:07.492271 feedancy-0.1.4/feedancy/apis/api/api_v1_internshipcity_retrieve_2.py
--rw-r--r--   0        0        0      971 2023-07-24 11:54:07.492271 feedancy-0.1.4/feedancy/apis/api/api_v1_internshipcity_update.py
--rw-r--r--   0        0        0      935 2023-07-24 11:54:07.496271 feedancy-0.1.4/feedancy/apis/api/api_v1_internshipcontact_create.py
--rw-r--r--   0        0        0      823 2023-07-24 11:54:07.496271 feedancy-0.1.4/feedancy/apis/api/api_v1_internshipcontact_destroy.py
--rw-r--r--   0        0        0      889 2023-07-24 11:54:07.492271 feedancy-0.1.4/feedancy/apis/api/api_v1_internshipcontact_retrieve.py
--rw-r--r--   0        0        0      944 2023-07-24 11:54:07.496271 feedancy-0.1.4/feedancy/apis/api/api_v1_internshipcontact_retrieve_2.py
--rw-r--r--   0        0        0      989 2023-07-24 11:54:07.496271 feedancy-0.1.4/feedancy/apis/api/api_v1_internshipcontact_update.py
--rw-r--r--   0        0        0      923 2023-07-24 11:54:07.496271 feedancy-0.1.4/feedancy/apis/api/api_v1_internshipskill_create.py
--rw-r--r--   0        0        0      821 2023-07-24 11:54:07.496271 feedancy-0.1.4/feedancy/apis/api/api_v1_internshipskill_destroy.py
--rw-r--r--   0        0        0      879 2023-07-24 11:54:07.496271 feedancy-0.1.4/feedancy/apis/api/api_v1_internshipskill_retrieve.py
--rw-r--r--   0        0        0      934 2023-07-24 11:54:07.496271 feedancy-0.1.4/feedancy/apis/api/api_v1_internshipskill_retrieve_2.py
--rw-r--r--   0        0        0      977 2023-07-24 11:54:07.496271 feedancy-0.1.4/feedancy/apis/api/api_v1_internshipskill_update.py
--rw-r--r--   0        0        0     1627 2023-07-24 11:54:07.500271 feedancy-0.1.4/feedancy/apis/api/api_v1_jobmixin_create.py
--rw-r--r--   0        0        0      814 2023-07-24 11:54:07.500271 feedancy-0.1.4/feedancy/apis/api/api_v1_jobmixin_destroy.py
--rw-r--r--   0        0        0     1590 2023-07-24 11:54:07.496271 feedancy-0.1.4/feedancy/apis/api/api_v1_jobmixin_retrieve.py
--rw-r--r--   0        0        0     1645 2023-07-24 11:54:07.500271 feedancy-0.1.4/feedancy/apis/api/api_v1_jobmixin_retrieve_2.py
--rw-r--r--   0        0        0     1681 2023-07-24 11:54:07.500271 feedancy-0.1.4/feedancy/apis/api/api_v1_jobmixin_update.py
--rw-r--r--   0        0        0      874 2023-07-24 11:54:07.500271 feedancy-0.1.4/feedancy/apis/api/api_v1_region_create.py
--rw-r--r--   0        0        0      812 2023-07-24 11:54:07.504271 feedancy-0.1.4/feedancy/apis/api/api_v1_region_destroy.py
--rw-r--r--   0        0        0      839 2023-07-24 11:54:07.500271 feedancy-0.1.4/feedancy/apis/api/api_v1_region_retrieve.py
--rw-r--r--   0        0        0      894 2023-07-24 11:54:07.504271 feedancy-0.1.4/feedancy/apis/api/api_v1_region_retrieve_2.py
--rw-r--r--   0        0        0      928 2023-07-24 11:54:07.504271 feedancy-0.1.4/feedancy/apis/api/api_v1_region_update.py
--rw-r--r--   0        0        0      988 2023-07-24 11:54:07.504271 feedancy-0.1.4/feedancy/apis/api/api_v1_salary_create.py
--rw-r--r--   0        0        0      812 2023-07-24 11:54:07.504271 feedancy-0.1.4/feedancy/apis/api/api_v1_salary_destroy.py
--rw-r--r--   0        0        0      953 2023-07-24 11:54:07.504271 feedancy-0.1.4/feedancy/apis/api/api_v1_salary_retrieve.py
--rw-r--r--   0        0        0     1008 2023-07-24 11:54:07.504271 feedancy-0.1.4/feedancy/apis/api/api_v1_salary_retrieve_2.py
--rw-r--r--   0        0        0     1042 2023-07-24 11:54:07.504271 feedancy-0.1.4/feedancy/apis/api/api_v1_salary_update.py
--rw-r--r--   0        0        0      966 2023-07-24 11:54:07.504271 feedancy-0.1.4/feedancy/apis/api/api_v1_searchandstopkeywords_create.py
--rw-r--r--   0        0        0      827 2023-07-24 11:54:07.508272 feedancy-0.1.4/feedancy/apis/api/api_v1_searchandstopkeywords_destroy.py
--rw-r--r--   0        0        0      916 2023-07-24 11:54:07.504271 feedancy-0.1.4/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve.py
--rw-r--r--   0        0        0      971 2023-07-24 11:54:07.504271 feedancy-0.1.4/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve_2.py
--rw-r--r--   0        0        0     1020 2023-07-24 11:54:07.508272 feedancy-0.1.4/feedancy/apis/api/api_v1_searchandstopkeywords_update.py
--rw-r--r--   0        0        0      896 2023-07-24 11:54:07.508272 feedancy-0.1.4/feedancy/apis/api/api_v1_searchkeywords_create.py
--rw-r--r--   0        0        0      820 2023-07-24 11:54:07.508272 feedancy-0.1.4/feedancy/apis/api/api_v1_searchkeywords_destroy.py
--rw-r--r--   0        0        0      890 2023-07-24 11:54:07.508272 feedancy-0.1.4/feedancy/apis/api/api_v1_searchkeywords_retrieve.py
--rw-r--r--   0        0        0      945 2023-07-24 11:54:07.508272 feedancy-0.1.4/feedancy/apis/api/api_v1_searchkeywords_retrieve_2.py
--rw-r--r--   0        0        0      950 2023-07-24 11:54:07.508272 feedancy-0.1.4/feedancy/apis/api/api_v1_searchkeywords_update.py
--rw-r--r--   0        0        0      851 2023-07-24 11:54:07.508272 feedancy-0.1.4/feedancy/apis/api/api_v1_skill_create.py
--rw-r--r--   0        0        0      811 2023-07-24 11:54:07.508272 feedancy-0.1.4/feedancy/apis/api/api_v1_skill_destroy.py
--rw-r--r--   0        0        0      817 2023-07-24 11:54:07.508272 feedancy-0.1.4/feedancy/apis/api/api_v1_skill_retrieve.py
--rw-r--r--   0        0        0      872 2023-07-24 11:54:07.508272 feedancy-0.1.4/feedancy/apis/api/api_v1_skill_retrieve_2.py
--rw-r--r--   0        0        0      905 2023-07-24 11:54:07.508272 feedancy-0.1.4/feedancy/apis/api/api_v1_skill_update.py
--rw-r--r--   0        0        0      856 2023-07-24 11:54:07.512272 feedancy-0.1.4/feedancy/apis/api/api_v1_source_create.py
--rw-r--r--   0        0        0      812 2023-07-24 11:54:07.512272 feedancy-0.1.4/feedancy/apis/api/api_v1_source_destroy.py
--rw-r--r--   0        0        0      821 2023-07-24 11:54:07.512272 feedancy-0.1.4/feedancy/apis/api/api_v1_source_retrieve.py
--rw-r--r--   0        0        0      876 2023-07-24 11:54:07.512272 feedancy-0.1.4/feedancy/apis/api/api_v1_source_retrieve_2.py
--rw-r--r--   0        0        0      910 2023-07-24 11:54:07.512272 feedancy-0.1.4/feedancy/apis/api/api_v1_source_update.py
--rw-r--r--   0        0        0      886 2023-07-24 11:54:07.512272 feedancy-0.1.4/feedancy/apis/api/api_v1_stopkeywords_create.py
--rw-r--r--   0        0        0      818 2023-07-24 11:54:07.512272 feedancy-0.1.4/feedancy/apis/api/api_v1_stopkeywords_destroy.py
--rw-r--r--   0        0        0      845 2023-07-24 11:54:07.512272 feedancy-0.1.4/feedancy/apis/api/api_v1_stopkeywords_retrieve.py
--rw-r--r--   0        0        0      900 2023-07-24 11:54:07.512272 feedancy-0.1.4/feedancy/apis/api/api_v1_stopkeywords_retrieve_2.py
--rw-r--r--   0        0        0      940 2023-07-24 11:54:07.512272 feedancy-0.1.4/feedancy/apis/api/api_v1_stopkeywords_update.py
--rw-r--r--   0        0        0     2046 2023-07-24 11:54:07.516272 feedancy-0.1.4/feedancy/apis/api/api_v1_vacancy_create.py
--rw-r--r--   0        0        0     2068 2023-07-24 11:54:07.520272 feedancy-0.1.4/feedancy/apis/api/api_v1_vacancy_destroy.py
--rw-r--r--   0        0        0     3236 2023-07-24 11:54:07.516272 feedancy-0.1.4/feedancy/apis/api/api_v1_vacancy_list.py
--rw-r--r--   0        0        0     2065 2023-07-24 11:54:07.520272 feedancy-0.1.4/feedancy/apis/api/api_v1_vacancy_retrieve.py
--rw-r--r--   0        0        0     2100 2023-07-24 11:54:07.520272 feedancy-0.1.4/feedancy/apis/api/api_v1_vacancy_update.py
--rw-r--r--   0        0        0      899 2023-07-24 11:54:07.520272 feedancy-0.1.4/feedancy/apis/api/api_v1_vacancycity_create.py
--rw-r--r--   0        0        0      817 2023-07-24 11:54:07.524272 feedancy-0.1.4/feedancy/apis/api/api_v1_vacancycity_destroy.py
--rw-r--r--   0        0        0      859 2023-07-24 11:54:07.520272 feedancy-0.1.4/feedancy/apis/api/api_v1_vacancycity_retrieve.py
--rw-r--r--   0        0        0      914 2023-07-24 11:54:07.524272 feedancy-0.1.4/feedancy/apis/api/api_v1_vacancycity_retrieve_2.py
--rw-r--r--   0        0        0      953 2023-07-24 11:54:07.524272 feedancy-0.1.4/feedancy/apis/api/api_v1_vacancycity_update.py
--rw-r--r--   0        0        0      917 2023-07-24 11:54:07.524272 feedancy-0.1.4/feedancy/apis/api/api_v1_vacancycontact_create.py
--rw-r--r--   0        0        0      820 2023-07-24 11:54:07.524272 feedancy-0.1.4/feedancy/apis/api/api_v1_vacancycontact_destroy.py
--rw-r--r--   0        0        0      874 2023-07-24 11:54:07.524272 feedancy-0.1.4/feedancy/apis/api/api_v1_vacancycontact_retrieve.py
--rw-r--r--   0        0        0      929 2023-07-24 11:54:07.524272 feedancy-0.1.4/feedancy/apis/api/api_v1_vacancycontact_retrieve_2.py
--rw-r--r--   0        0        0      971 2023-07-24 11:54:07.524272 feedancy-0.1.4/feedancy/apis/api/api_v1_vacancycontact_update.py
--rw-r--r--   0        0        0      905 2023-07-24 11:54:07.524272 feedancy-0.1.4/feedancy/apis/api/api_v1_vacancyskill_create.py
--rw-r--r--   0        0        0      818 2023-07-24 11:54:07.528272 feedancy-0.1.4/feedancy/apis/api/api_v1_vacancyskill_destroy.py
--rw-r--r--   0        0        0      864 2023-07-24 11:54:07.524272 feedancy-0.1.4/feedancy/apis/api/api_v1_vacancyskill_retrieve.py
--rw-r--r--   0        0        0      919 2023-07-24 11:54:07.524272 feedancy-0.1.4/feedancy/apis/api/api_v1_vacancyskill_retrieve_2.py
--rw-r--r--   0        0        0      959 2023-07-24 11:54:07.524272 feedancy-0.1.4/feedancy/apis/api/api_v1_vacancyskill_update.py
--rw-r--r--   0        0        0      658 2023-07-24 11:54:07.528272 feedancy-0.1.4/feedancy/client.py
--rw-r--r--   0        0        0        0 2023-07-24 11:54:07.532272 feedancy-0.1.4/feedancy/lib/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 11:54:07.532272 feedancy-0.1.4/feedancy/lib/adapter/__init__.py
--rw-r--r--   0        0        0     2818 2023-07-24 11:54:07.532272 feedancy-0.1.4/feedancy/lib/adapter/aiohttp.py
--rw-r--r--   0        0        0      235 2023-07-24 11:54:07.532272 feedancy-0.1.4/feedancy/lib/adapter/base.py
--rw-r--r--   0        0        0     2680 2023-07-24 11:54:07.532272 feedancy-0.1.4/feedancy/lib/adapter/httpx.py
--rw-r--r--   0        0        0     2446 2023-07-24 11:54:07.532272 feedancy-0.1.4/feedancy/lib/adapter/params_converter.py
--rw-r--r--   0        0        0     3005 2023-07-24 11:54:07.532272 feedancy-0.1.4/feedancy/lib/adapter/requests.py
--rw-r--r--   0        0        0     2769 2023-07-24 11:54:07.532272 feedancy-0.1.4/feedancy/lib/base.py
--rw-r--r--   0        0        0      685 2023-07-24 11:54:07.532272 feedancy-0.1.4/feedancy/lib/client.py
--rw-r--r--   0        0        0      929 2023-07-24 11:54:07.532272 feedancy-0.1.4/feedancy/lib/configuration.py
--rw-r--r--   0        0        0      466 2023-07-24 11:54:07.532272 feedancy-0.1.4/feedancy/lib/exceptions.py
--rw-r--r--   0        0        0      403 2023-07-24 11:54:07.532272 feedancy-0.1.4/feedancy/lib/json.py
--rw-r--r--   0        0        0      613 2023-07-24 11:54:07.532272 feedancy-0.1.4/feedancy/lib/request.py
--rw-r--r--   0        0        0      384 2023-07-24 11:54:07.532272 feedancy-0.1.4/feedancy/lib/response.py
--rw-r--r--   0        0        0      895 2023-07-24 11:54:07.532272 feedancy-0.1.4/feedancy/lib/response_deserializer.py
--rw-r--r--   0        0        0      564 2023-07-24 11:54:07.532272 feedancy-0.1.4/feedancy/lib/types.py
--rw-r--r--   0        0        0      949 2023-07-24 12:25:24.922349 feedancy-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1120 1970-01-01 00:00:00.000000 feedancy-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      615 2023-08-01 19:37:20.963096 feedancy-0.1.5/README.md
+-rw-r--r--   0        0        0      126 2023-08-01 19:37:20.955097 feedancy-0.1.5/feedancy/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 19:37:20.875106 feedancy-0.1.5/feedancy/apis/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 19:37:20.875106 feedancy-0.1.5/feedancy/apis/api/__init__.py
+-rw-r--r--   0        0        0    13072 2023-08-01 19:37:20.879106 feedancy-0.1.5/feedancy/apis/api/api.py
+-rw-r--r--   0        0        0      896 2023-08-01 19:37:20.895104 feedancy-0.1.5/feedancy/apis/api/api_v1_activitysphere_create.py
+-rw-r--r--   0        0        0      820 2023-08-01 19:37:20.895104 feedancy-0.1.5/feedancy/apis/api/api_v1_activitysphere_destroy.py
+-rw-r--r--   0        0        0      853 2023-08-01 19:37:20.891104 feedancy-0.1.5/feedancy/apis/api/api_v1_activitysphere_retrieve.py
+-rw-r--r--   0        0        0      908 2023-08-01 19:37:20.895104 feedancy-0.1.5/feedancy/apis/api/api_v1_activitysphere_retrieve_2.py
+-rw-r--r--   0        0        0      950 2023-08-01 19:37:20.895104 feedancy-0.1.5/feedancy/apis/api/api_v1_activitysphere_update.py
+-rw-r--r--   0        0        0      863 2023-08-01 19:37:20.895104 feedancy-0.1.5/feedancy/apis/api/api_v1_city_create.py
+-rw-r--r--   0        0        0      810 2023-08-01 19:37:20.895104 feedancy-0.1.5/feedancy/apis/api/api_v1_city_destroy.py
+-rw-r--r--   0        0        0      830 2023-08-01 19:37:20.895104 feedancy-0.1.5/feedancy/apis/api/api_v1_city_retrieve.py
+-rw-r--r--   0        0        0      885 2023-08-01 19:37:20.895104 feedancy-0.1.5/feedancy/apis/api/api_v1_city_retrieve_2.py
+-rw-r--r--   0        0        0      917 2023-08-01 19:37:20.895104 feedancy-0.1.5/feedancy/apis/api/api_v1_city_update.py
+-rw-r--r--   0        0        0     1258 2023-08-01 19:37:20.899103 feedancy-0.1.5/feedancy/apis/api/api_v1_company_create.py
+-rw-r--r--   0        0        0      813 2023-08-01 19:37:20.899103 feedancy-0.1.5/feedancy/apis/api/api_v1_company_destroy.py
+-rw-r--r--   0        0        0     1222 2023-08-01 19:37:20.895104 feedancy-0.1.5/feedancy/apis/api/api_v1_company_retrieve.py
+-rw-r--r--   0        0        0     1277 2023-08-01 19:37:20.899103 feedancy-0.1.5/feedancy/apis/api/api_v1_company_retrieve_2.py
+-rw-r--r--   0        0        0     1312 2023-08-01 19:37:20.899103 feedancy-0.1.5/feedancy/apis/api/api_v1_company_update.py
+-rw-r--r--   0        0        0      899 2023-08-01 19:37:20.899103 feedancy-0.1.5/feedancy/apis/api/api_v1_companycity_create.py
+-rw-r--r--   0        0        0      817 2023-08-01 19:37:20.903103 feedancy-0.1.5/feedancy/apis/api/api_v1_companycity_destroy.py
+-rw-r--r--   0        0        0      859 2023-08-01 19:37:20.899103 feedancy-0.1.5/feedancy/apis/api/api_v1_companycity_retrieve.py
+-rw-r--r--   0        0        0      914 2023-08-01 19:37:20.899103 feedancy-0.1.5/feedancy/apis/api/api_v1_companycity_retrieve_2.py
+-rw-r--r--   0        0        0      953 2023-08-01 19:37:20.903103 feedancy-0.1.5/feedancy/apis/api/api_v1_companycity_update.py
+-rw-r--r--   0        0        0      935 2023-08-01 19:37:20.903103 feedancy-0.1.5/feedancy/apis/api/api_v1_contact_create.py
+-rw-r--r--   0        0        0      813 2023-08-01 19:37:20.903103 feedancy-0.1.5/feedancy/apis/api/api_v1_contact_destroy.py
+-rw-r--r--   0        0        0      899 2023-08-01 19:37:20.903103 feedancy-0.1.5/feedancy/apis/api/api_v1_contact_retrieve.py
+-rw-r--r--   0        0        0      954 2023-08-01 19:37:20.903103 feedancy-0.1.5/feedancy/apis/api/api_v1_contact_retrieve_2.py
+-rw-r--r--   0        0        0      989 2023-08-01 19:37:20.903103 feedancy-0.1.5/feedancy/apis/api/api_v1_contact_update.py
+-rw-r--r--   0        0        0      876 2023-08-01 19:37:20.903103 feedancy-0.1.5/feedancy/apis/api/api_v1_country_create.py
+-rw-r--r--   0        0        0      813 2023-08-01 19:37:20.907103 feedancy-0.1.5/feedancy/apis/api/api_v1_country_destroy.py
+-rw-r--r--   0        0        0      840 2023-08-01 19:37:20.903103 feedancy-0.1.5/feedancy/apis/api/api_v1_country_retrieve.py
+-rw-r--r--   0        0        0      895 2023-08-01 19:37:20.903103 feedancy-0.1.5/feedancy/apis/api/api_v1_country_retrieve_2.py
+-rw-r--r--   0        0        0      930 2023-08-01 19:37:20.903103 feedancy-0.1.5/feedancy/apis/api/api_v1_country_update.py
+-rw-r--r--   0        0        0      881 2023-08-01 19:37:20.907103 feedancy-0.1.5/feedancy/apis/api/api_v1_currency_create.py
+-rw-r--r--   0        0        0      814 2023-08-01 19:37:20.907103 feedancy-0.1.5/feedancy/apis/api/api_v1_currency_destroy.py
+-rw-r--r--   0        0        0      844 2023-08-01 19:37:20.907103 feedancy-0.1.5/feedancy/apis/api/api_v1_currency_retrieve.py
+-rw-r--r--   0        0        0      899 2023-08-01 19:37:20.907103 feedancy-0.1.5/feedancy/apis/api/api_v1_currency_retrieve_2.py
+-rw-r--r--   0        0        0      935 2023-08-01 19:37:20.907103 feedancy-0.1.5/feedancy/apis/api/api_v1_currency_update.py
+-rw-r--r--   0        0        0     1922 2023-08-01 19:37:20.911102 feedancy-0.1.5/feedancy/apis/api/api_v1_internship_create.py
+-rw-r--r--   0        0        0     1941 2023-08-01 19:37:20.915102 feedancy-0.1.5/feedancy/apis/api/api_v1_internship_destroy.py
+-rw-r--r--   0        0        0     1883 2023-08-01 19:37:20.907103 feedancy-0.1.5/feedancy/apis/api/api_v1_internship_retrieve.py
+-rw-r--r--   0        0        0     1938 2023-08-01 19:37:20.911102 feedancy-0.1.5/feedancy/apis/api/api_v1_internship_retrieve_2.py
+-rw-r--r--   0        0        0     1976 2023-08-01 19:37:20.911102 feedancy-0.1.5/feedancy/apis/api/api_v1_internship_update.py
+-rw-r--r--   0        0        0      917 2023-08-01 19:37:20.915102 feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcity_create.py
+-rw-r--r--   0        0        0      820 2023-08-01 19:37:20.915102 feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcity_destroy.py
+-rw-r--r--   0        0        0      874 2023-08-01 19:37:20.915102 feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcity_retrieve.py
+-rw-r--r--   0        0        0      929 2023-08-01 19:37:20.915102 feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcity_retrieve_2.py
+-rw-r--r--   0        0        0      971 2023-08-01 19:37:20.915102 feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcity_update.py
+-rw-r--r--   0        0        0      935 2023-08-01 19:37:20.915102 feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcontact_create.py
+-rw-r--r--   0        0        0      823 2023-08-01 19:37:20.915102 feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcontact_destroy.py
+-rw-r--r--   0        0        0      889 2023-08-01 19:37:20.915102 feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcontact_retrieve.py
+-rw-r--r--   0        0        0      944 2023-08-01 19:37:20.915102 feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcontact_retrieve_2.py
+-rw-r--r--   0        0        0      989 2023-08-01 19:37:20.915102 feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcontact_update.py
+-rw-r--r--   0        0        0      923 2023-08-01 19:37:20.919101 feedancy-0.1.5/feedancy/apis/api/api_v1_internshipskill_create.py
+-rw-r--r--   0        0        0      821 2023-08-01 19:37:20.919101 feedancy-0.1.5/feedancy/apis/api/api_v1_internshipskill_destroy.py
+-rw-r--r--   0        0        0      879 2023-08-01 19:37:20.919101 feedancy-0.1.5/feedancy/apis/api/api_v1_internshipskill_retrieve.py
+-rw-r--r--   0        0        0      934 2023-08-01 19:37:20.919101 feedancy-0.1.5/feedancy/apis/api/api_v1_internshipskill_retrieve_2.py
+-rw-r--r--   0        0        0      977 2023-08-01 19:37:20.919101 feedancy-0.1.5/feedancy/apis/api/api_v1_internshipskill_update.py
+-rw-r--r--   0        0        0     1627 2023-08-01 19:37:20.919101 feedancy-0.1.5/feedancy/apis/api/api_v1_jobmixin_create.py
+-rw-r--r--   0        0        0      814 2023-08-01 19:37:20.923101 feedancy-0.1.5/feedancy/apis/api/api_v1_jobmixin_destroy.py
+-rw-r--r--   0        0        0     1590 2023-08-01 19:37:20.919101 feedancy-0.1.5/feedancy/apis/api/api_v1_jobmixin_retrieve.py
+-rw-r--r--   0        0        0     1645 2023-08-01 19:37:20.923101 feedancy-0.1.5/feedancy/apis/api/api_v1_jobmixin_retrieve_2.py
+-rw-r--r--   0        0        0     1681 2023-08-01 19:37:20.923101 feedancy-0.1.5/feedancy/apis/api/api_v1_jobmixin_update.py
+-rw-r--r--   0        0        0      874 2023-08-01 19:37:20.923101 feedancy-0.1.5/feedancy/apis/api/api_v1_region_create.py
+-rw-r--r--   0        0        0      812 2023-08-01 19:37:20.927100 feedancy-0.1.5/feedancy/apis/api/api_v1_region_destroy.py
+-rw-r--r--   0        0        0      839 2023-08-01 19:37:20.923101 feedancy-0.1.5/feedancy/apis/api/api_v1_region_retrieve.py
+-rw-r--r--   0        0        0      894 2023-08-01 19:37:20.923101 feedancy-0.1.5/feedancy/apis/api/api_v1_region_retrieve_2.py
+-rw-r--r--   0        0        0      928 2023-08-01 19:37:20.927100 feedancy-0.1.5/feedancy/apis/api/api_v1_region_update.py
+-rw-r--r--   0        0        0      969 2023-08-01 19:37:20.927100 feedancy-0.1.5/feedancy/apis/api/api_v1_salary_create.py
+-rw-r--r--   0        0        0      812 2023-08-01 19:37:20.927100 feedancy-0.1.5/feedancy/apis/api/api_v1_salary_destroy.py
+-rw-r--r--   0        0        0      953 2023-08-01 19:37:20.927100 feedancy-0.1.5/feedancy/apis/api/api_v1_salary_retrieve.py
+-rw-r--r--   0        0        0     1008 2023-08-01 19:37:20.927100 feedancy-0.1.5/feedancy/apis/api/api_v1_salary_retrieve_2.py
+-rw-r--r--   0        0        0     1023 2023-08-01 19:37:20.927100 feedancy-0.1.5/feedancy/apis/api/api_v1_salary_update.py
+-rw-r--r--   0        0        0      966 2023-08-01 19:37:20.927100 feedancy-0.1.5/feedancy/apis/api/api_v1_searchandstopkeywords_create.py
+-rw-r--r--   0        0        0      827 2023-08-01 19:37:20.931100 feedancy-0.1.5/feedancy/apis/api/api_v1_searchandstopkeywords_destroy.py
+-rw-r--r--   0        0        0      916 2023-08-01 19:37:20.927100 feedancy-0.1.5/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve.py
+-rw-r--r--   0        0        0      971 2023-08-01 19:37:20.927100 feedancy-0.1.5/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve_2.py
+-rw-r--r--   0        0        0     1020 2023-08-01 19:37:20.931100 feedancy-0.1.5/feedancy/apis/api/api_v1_searchandstopkeywords_update.py
+-rw-r--r--   0        0        0      896 2023-08-01 19:37:20.931100 feedancy-0.1.5/feedancy/apis/api/api_v1_searchkeywords_create.py
+-rw-r--r--   0        0        0      820 2023-08-01 19:37:20.931100 feedancy-0.1.5/feedancy/apis/api/api_v1_searchkeywords_destroy.py
+-rw-r--r--   0        0        0      890 2023-08-01 19:37:20.931100 feedancy-0.1.5/feedancy/apis/api/api_v1_searchkeywords_retrieve.py
+-rw-r--r--   0        0        0      945 2023-08-01 19:37:20.931100 feedancy-0.1.5/feedancy/apis/api/api_v1_searchkeywords_retrieve_2.py
+-rw-r--r--   0        0        0      950 2023-08-01 19:37:20.931100 feedancy-0.1.5/feedancy/apis/api/api_v1_searchkeywords_update.py
+-rw-r--r--   0        0        0      851 2023-08-01 19:37:20.931100 feedancy-0.1.5/feedancy/apis/api/api_v1_skill_create.py
+-rw-r--r--   0        0        0      811 2023-08-01 19:37:20.935099 feedancy-0.1.5/feedancy/apis/api/api_v1_skill_destroy.py
+-rw-r--r--   0        0        0      817 2023-08-01 19:37:20.931100 feedancy-0.1.5/feedancy/apis/api/api_v1_skill_retrieve.py
+-rw-r--r--   0        0        0      872 2023-08-01 19:37:20.931100 feedancy-0.1.5/feedancy/apis/api/api_v1_skill_retrieve_2.py
+-rw-r--r--   0        0        0      905 2023-08-01 19:37:20.935099 feedancy-0.1.5/feedancy/apis/api/api_v1_skill_update.py
+-rw-r--r--   0        0        0      856 2023-08-01 19:37:20.935099 feedancy-0.1.5/feedancy/apis/api/api_v1_source_create.py
+-rw-r--r--   0        0        0      812 2023-08-01 19:37:20.935099 feedancy-0.1.5/feedancy/apis/api/api_v1_source_destroy.py
+-rw-r--r--   0        0        0      821 2023-08-01 19:37:20.935099 feedancy-0.1.5/feedancy/apis/api/api_v1_source_retrieve.py
+-rw-r--r--   0        0        0      876 2023-08-01 19:37:20.935099 feedancy-0.1.5/feedancy/apis/api/api_v1_source_retrieve_2.py
+-rw-r--r--   0        0        0      910 2023-08-01 19:37:20.935099 feedancy-0.1.5/feedancy/apis/api/api_v1_source_update.py
+-rw-r--r--   0        0        0      886 2023-08-01 19:37:20.935099 feedancy-0.1.5/feedancy/apis/api/api_v1_stopkeywords_create.py
+-rw-r--r--   0        0        0      818 2023-08-01 19:37:20.935099 feedancy-0.1.5/feedancy/apis/api/api_v1_stopkeywords_destroy.py
+-rw-r--r--   0        0        0      845 2023-08-01 19:37:20.935099 feedancy-0.1.5/feedancy/apis/api/api_v1_stopkeywords_retrieve.py
+-rw-r--r--   0        0        0      900 2023-08-01 19:37:20.935099 feedancy-0.1.5/feedancy/apis/api/api_v1_stopkeywords_retrieve_2.py
+-rw-r--r--   0        0        0      940 2023-08-01 19:37:20.935099 feedancy-0.1.5/feedancy/apis/api/api_v1_stopkeywords_update.py
+-rw-r--r--   0        0        0     2092 2023-08-01 19:37:20.943098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancy_create.py
+-rw-r--r--   0        0        0     2169 2023-08-01 19:37:20.947098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancy_destroy.py
+-rw-r--r--   0        0        0     3217 2023-08-01 19:37:20.939099 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancy_list.py
+-rw-r--r--   0        0        0     2166 2023-08-01 19:37:20.943098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancy_retrieve.py
+-rw-r--r--   0        0        0     2146 2023-08-01 19:37:20.947098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancy_update.py
+-rw-r--r--   0        0        0      899 2023-08-01 19:37:20.947098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycity_create.py
+-rw-r--r--   0        0        0      817 2023-08-01 19:37:20.947098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycity_destroy.py
+-rw-r--r--   0        0        0      859 2023-08-01 19:37:20.947098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycity_retrieve.py
+-rw-r--r--   0        0        0      914 2023-08-01 19:37:20.947098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycity_retrieve_2.py
+-rw-r--r--   0        0        0      953 2023-08-01 19:37:20.947098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycity_update.py
+-rw-r--r--   0        0        0      917 2023-08-01 19:37:20.951098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycontact_create.py
+-rw-r--r--   0        0        0      820 2023-08-01 19:37:20.951098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycontact_destroy.py
+-rw-r--r--   0        0        0      874 2023-08-01 19:37:20.951098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycontact_retrieve.py
+-rw-r--r--   0        0        0      929 2023-08-01 19:37:20.951098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycontact_retrieve_2.py
+-rw-r--r--   0        0        0      971 2023-08-01 19:37:20.951098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycontact_update.py
+-rw-r--r--   0        0        0      905 2023-08-01 19:37:20.951098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancyskill_create.py
+-rw-r--r--   0        0        0      818 2023-08-01 19:37:20.951098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancyskill_destroy.py
+-rw-r--r--   0        0        0      864 2023-08-01 19:37:20.951098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancyskill_retrieve.py
+-rw-r--r--   0        0        0      919 2023-08-01 19:37:20.951098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancyskill_retrieve_2.py
+-rw-r--r--   0        0        0      959 2023-08-01 19:37:20.951098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancyskill_update.py
+-rw-r--r--   0        0        0      658 2023-08-01 19:37:20.955097 feedancy-0.1.5/feedancy/client.py
+-rw-r--r--   0        0        0        0 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/adapter/__init__.py
+-rw-r--r--   0        0        0     2818 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/adapter/aiohttp.py
+-rw-r--r--   0        0        0      235 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/adapter/base.py
+-rw-r--r--   0        0        0     2680 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/adapter/httpx.py
+-rw-r--r--   0        0        0     2446 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/adapter/params_converter.py
+-rw-r--r--   0        0        0     3005 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/adapter/requests.py
+-rw-r--r--   0        0        0     2769 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/base.py
+-rw-r--r--   0        0        0      685 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/client.py
+-rw-r--r--   0        0        0      929 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/configuration.py
+-rw-r--r--   0        0        0      466 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/exceptions.py
+-rw-r--r--   0        0        0      403 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/json.py
+-rw-r--r--   0        0        0      613 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/request.py
+-rw-r--r--   0        0        0      384 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/response.py
+-rw-r--r--   0        0        0      895 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/response_deserializer.py
+-rw-r--r--   0        0        0      564 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/types.py
+-rw-r--r--   0        0        0      651 2023-08-01 19:36:14.485587 feedancy-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1120 1970-01-01 00:00:00.000000 feedancy-0.1.5/PKG-INFO
```

### Comparing `feedancy-0.1.4/README.md` & `feedancy-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api.py` & `feedancy-0.1.5/feedancy/apis/api/api.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_activitysphere_create.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_activitysphere_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_activitysphere_destroy.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_activitysphere_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_activitysphere_retrieve.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_activitysphere_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_activitysphere_retrieve_2.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_activitysphere_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_activitysphere_update.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_activitysphere_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_city_create.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_city_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_city_destroy.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_city_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_city_retrieve.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_city_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_city_retrieve_2.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_city_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_city_update.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_city_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_company_create.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_company_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_company_destroy.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_company_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_company_retrieve.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_company_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_company_retrieve_2.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_company_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_company_update.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_company_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_companycity_create.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_companycity_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_companycity_destroy.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_companycity_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_companycity_retrieve.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_companycity_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_companycity_retrieve_2.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_companycity_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_companycity_update.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_companycity_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_contact_create.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_contact_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_contact_destroy.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_contact_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_contact_retrieve.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_contact_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_contact_retrieve_2.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_contact_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_contact_update.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_contact_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_country_create.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_country_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_country_destroy.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_country_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_country_retrieve.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_country_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_country_retrieve_2.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_country_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_country_update.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_country_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_currency_create.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_currency_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_currency_destroy.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_currency_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_currency_retrieve.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_currency_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_currency_retrieve_2.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_currency_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_currency_update.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_currency_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_internship_create.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_internship_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_internship_destroy.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_internship_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_internship_retrieve.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_internship_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_internship_retrieve_2.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_internship_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_internship_update.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_internship_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_internshipcity_create.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcity_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_internshipcity_destroy.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcity_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_internshipcity_retrieve.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcity_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_internshipcity_retrieve_2.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcity_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_internshipcity_update.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcity_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_internshipcontact_create.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcontact_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_internshipcontact_destroy.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcontact_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_internshipcontact_retrieve.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcontact_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_internshipcontact_retrieve_2.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcontact_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_internshipcontact_update.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcontact_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_internshipskill_create.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_internshipskill_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_internshipskill_destroy.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_internshipskill_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_internshipskill_retrieve.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_internshipskill_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_internshipskill_retrieve_2.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_internshipskill_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_internshipskill_update.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_internshipskill_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_jobmixin_create.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_jobmixin_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_jobmixin_destroy.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_jobmixin_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_jobmixin_retrieve.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_jobmixin_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_jobmixin_retrieve_2.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_jobmixin_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_jobmixin_update.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_jobmixin_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_region_create.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_region_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_region_destroy.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_region_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_region_retrieve.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_region_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_region_retrieve_2.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_region_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_region_update.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_region_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_salary_create.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_salary_update.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,33 +6,36 @@
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
 class Salary(BaseModel):
-    currency: int 
     max_value: typing.Optional[typing.Union[int, None]]  = None
     min_value: typing.Optional[typing.Union[int, None]]  = None
 
 def make_request(self: BaseApi,
 
     __request__: Salary,
 
 
+    id: str,
+
 ) -> Salary:
     
 
     
     body = __request__
     
 
     m = ApiRequest(
-        method="POST",
-        path="/api/v1/salary/".format(
+        method="PUT",
+        path="/api/v1/salary/{id}/".format(
+            
+                id=id,
             
         ),
         content_type="application/json",
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
```

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_salary_destroy.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_salary_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_salary_retrieve.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_salary_retrieve.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
 class Salary(BaseModel):
-    currency: int 
+    currency: str 
     id: int 
     max_value: typing.Optional[typing.Union[int, None]]  = None
     min_value: typing.Optional[typing.Union[int, None]]  = None
 
 def make_request(self: BaseApi,
```

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_salary_retrieve_2.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_salary_retrieve_2.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
 class Salary(BaseModel):
-    currency: int 
+    currency: str 
     id: int 
     max_value: typing.Optional[typing.Union[int, None]]  = None
     min_value: typing.Optional[typing.Union[int, None]]  = None
 
 def make_request(self: BaseApi,
```

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_salary_update.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_salary_create.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,37 +6,32 @@
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
 class Salary(BaseModel):
-    currency: int 
     max_value: typing.Optional[typing.Union[int, None]]  = None
     min_value: typing.Optional[typing.Union[int, None]]  = None
 
 def make_request(self: BaseApi,
 
     __request__: Salary,
 
 
-    id: str,
-
 ) -> Salary:
     
 
     
     body = __request__
     
 
     m = ApiRequest(
-        method="PUT",
-        path="/api/v1/salary/{id}/".format(
-            
-                id=id,
+        method="POST",
+        path="/api/v1/salary/".format(
             
         ),
         content_type="application/json",
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
```

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_searchandstopkeywords_create.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_searchandstopkeywords_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_searchandstopkeywords_destroy.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_searchandstopkeywords_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve_2.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_searchandstopkeywords_update.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_searchandstopkeywords_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_searchkeywords_create.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_searchkeywords_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_searchkeywords_destroy.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_searchkeywords_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_searchkeywords_retrieve.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_searchkeywords_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_searchkeywords_retrieve_2.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_searchkeywords_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_searchkeywords_update.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_searchkeywords_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_skill_create.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_skill_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_skill_destroy.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_skill_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_skill_retrieve.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_skill_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_skill_retrieve_2.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_skill_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_skill_update.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_skill_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_source_create.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_source_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_source_destroy.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_source_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_source_retrieve.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_source_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_source_retrieve_2.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_source_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_source_update.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_source_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_stopkeywords_create.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_stopkeywords_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_stopkeywords_destroy.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_stopkeywords_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_stopkeywords_retrieve.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_stopkeywords_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_stopkeywords_retrieve_2.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_stopkeywords_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_stopkeywords_update.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_stopkeywords_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_vacancy_create.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancy_create.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,34 +6,37 @@
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
 class Vacancy(BaseModel):
-    company: typing.Optional[typing.Union[int, None]]  = None
     contract_type: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     employment_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     experience: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     external_id: str 
     has_insurance: typing.Optional[typing.Union[bool, None]]  = None
     has_portfolio: typing.Optional[typing.Union[bool, None]]  = None
     has_test_task: typing.Optional[typing.Union[bool, None]]  = None
     is_relocation_required: typing.Optional[typing.Union[bool, None]]  = None
     link: str 
     name: str 
     publicated_at: typing.Optional[typing.Union[datetime.datetime, None]]  = None
     raw_description: typing.Optional[typing.Union[str, None]]  = None
     requirement: typing.Optional[typing.Union[str, None]]  = None
     responsibility: typing.Optional[typing.Union[str, None]]  = None
-    salary: typing.Optional[typing.Union[int, None]]  = None
-    source: int 
     test_task_link: typing.Optional[typing.Union[str, None]]  = None
     work_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
 
+class Salary(BaseModel):
+    currency: str 
+    id: int 
+    max_value: typing.Optional[typing.Union[int, None]]  = None
+    min_value: typing.Optional[typing.Union[int, None]]  = None
+
 def make_request(self: BaseApi,
 
     __request__: Vacancy,
 
 
 ) -> Vacancy:
```

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_vacancy_destroy.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancy_destroy.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,22 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
+class Salary(BaseModel):
+    currency: str 
+    id: int 
+    max_value: typing.Optional[typing.Union[int, None]]  = None
+    min_value: typing.Optional[typing.Union[int, None]]  = None
+
 class Vacancy(BaseModel):
-    company: typing.Optional[typing.Union[int, None]]  = None
+    company: str 
     contract_type: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     employment_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     experience: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     external_id: str 
     has_insurance: typing.Optional[typing.Union[bool, None]]  = None
     has_portfolio: typing.Optional[typing.Union[bool, None]]  = None
     has_test_task: typing.Optional[typing.Union[bool, None]]  = None
@@ -22,16 +28,16 @@
     is_relocation_required: typing.Optional[typing.Union[bool, None]]  = None
     link: str 
     name: str 
     publicated_at: typing.Optional[typing.Union[datetime.datetime, None]]  = None
     raw_description: typing.Optional[typing.Union[str, None]]  = None
     requirement: typing.Optional[typing.Union[str, None]]  = None
     responsibility: typing.Optional[typing.Union[str, None]]  = None
-    salary: typing.Optional[typing.Union[int, None]]  = None
-    source: int 
+    salary: Salary 
+    source: str 
     test_task_link: typing.Optional[typing.Union[str, None]]  = None
     work_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
 
 def make_request(self: BaseApi,
 
 
     id: str,
```

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_vacancy_list.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancy_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,22 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
+class Salary(BaseModel):
+    currency: str 
+    id: int 
+    max_value: typing.Optional[typing.Union[int, None]]  = None
+    min_value: typing.Optional[typing.Union[int, None]]  = None
+
 class Vacancy(BaseModel):
-    company: typing.Optional[typing.Union[int, None]]  = None
+    company: str 
     contract_type: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     employment_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     experience: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     external_id: str 
     has_insurance: typing.Optional[typing.Union[bool, None]]  = None
     has_portfolio: typing.Optional[typing.Union[bool, None]]  = None
     has_test_task: typing.Optional[typing.Union[bool, None]]  = None
@@ -22,16 +28,16 @@
     is_relocation_required: typing.Optional[typing.Union[bool, None]]  = None
     link: str 
     name: str 
     publicated_at: typing.Optional[typing.Union[datetime.datetime, None]]  = None
     raw_description: typing.Optional[typing.Union[str, None]]  = None
     requirement: typing.Optional[typing.Union[str, None]]  = None
     responsibility: typing.Optional[typing.Union[str, None]]  = None
-    salary: typing.Optional[typing.Union[int, None]]  = None
-    source: int 
+    salary: Salary 
+    source: str 
     test_task_link: typing.Optional[typing.Union[str, None]]  = None
     work_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
 
 class PaginatedVacancyList(BaseModel):
     count: typing.Optional[int]  = None
     next: typing.Optional[typing.Union[str, None]]  = None
     previous: typing.Optional[typing.Union[str, None]]  = None
@@ -50,16 +56,14 @@
 
     is_accredited: bool = ...,
 
     is_relocation_required: bool = ...,
 
     page: int = ...,
 
-    relocation_is_required: bool = ...,
-
     search: str = ...,
 
     work_format: str = ...,
 
 ) -> PaginatedVacancyList:
     
 
@@ -87,16 +91,14 @@
             
                 "is_accredited": is_accredited,
             
                 "is_relocation_required": is_relocation_required,
             
                 "page": page,
             
-                "relocation_is_required": relocation_is_required,
-            
                 "search": search,
             
                 "work_format": work_format,
             
         }),
         cookies=self._only_provided({
         }),
```

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_vacancy_retrieve.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancy_retrieve.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,22 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
+class Salary(BaseModel):
+    currency: str 
+    id: int 
+    max_value: typing.Optional[typing.Union[int, None]]  = None
+    min_value: typing.Optional[typing.Union[int, None]]  = None
+
 class Vacancy(BaseModel):
-    company: typing.Optional[typing.Union[int, None]]  = None
+    company: str 
     contract_type: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     employment_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     experience: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     external_id: str 
     has_insurance: typing.Optional[typing.Union[bool, None]]  = None
     has_portfolio: typing.Optional[typing.Union[bool, None]]  = None
     has_test_task: typing.Optional[typing.Union[bool, None]]  = None
@@ -22,16 +28,16 @@
     is_relocation_required: typing.Optional[typing.Union[bool, None]]  = None
     link: str 
     name: str 
     publicated_at: typing.Optional[typing.Union[datetime.datetime, None]]  = None
     raw_description: typing.Optional[typing.Union[str, None]]  = None
     requirement: typing.Optional[typing.Union[str, None]]  = None
     responsibility: typing.Optional[typing.Union[str, None]]  = None
-    salary: typing.Optional[typing.Union[int, None]]  = None
-    source: int 
+    salary: Salary 
+    source: str 
     test_task_link: typing.Optional[typing.Union[str, None]]  = None
     work_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
 
 def make_request(self: BaseApi,
 
 
     id: str,
```

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_vacancy_update.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancy_update.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,34 +6,37 @@
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
 class Vacancy(BaseModel):
-    company: typing.Optional[typing.Union[int, None]]  = None
     contract_type: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     employment_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     experience: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     external_id: str 
     has_insurance: typing.Optional[typing.Union[bool, None]]  = None
     has_portfolio: typing.Optional[typing.Union[bool, None]]  = None
     has_test_task: typing.Optional[typing.Union[bool, None]]  = None
     is_relocation_required: typing.Optional[typing.Union[bool, None]]  = None
     link: str 
     name: str 
     publicated_at: typing.Optional[typing.Union[datetime.datetime, None]]  = None
     raw_description: typing.Optional[typing.Union[str, None]]  = None
     requirement: typing.Optional[typing.Union[str, None]]  = None
     responsibility: typing.Optional[typing.Union[str, None]]  = None
-    salary: typing.Optional[typing.Union[int, None]]  = None
-    source: int 
     test_task_link: typing.Optional[typing.Union[str, None]]  = None
     work_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
 
+class Salary(BaseModel):
+    currency: str 
+    id: int 
+    max_value: typing.Optional[typing.Union[int, None]]  = None
+    min_value: typing.Optional[typing.Union[int, None]]  = None
+
 def make_request(self: BaseApi,
 
     __request__: Vacancy,
 
 
     id: str,
```

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_vacancycity_create.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycity_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_vacancycity_destroy.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycity_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_vacancycity_retrieve.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycity_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_vacancycity_retrieve_2.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycity_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_vacancycity_update.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycity_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_vacancycontact_create.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycontact_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_vacancycontact_destroy.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycontact_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_vacancycontact_retrieve.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycontact_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_vacancycontact_retrieve_2.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycontact_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_vacancycontact_update.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycontact_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_vacancyskill_create.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancyskill_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_vacancyskill_destroy.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancyskill_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_vacancyskill_retrieve.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancyskill_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_vacancyskill_retrieve_2.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancyskill_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/apis/api/api_v1_vacancyskill_update.py` & `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancyskill_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/client.py` & `feedancy-0.1.5/feedancy/client.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/lib/adapter/aiohttp.py` & `feedancy-0.1.5/feedancy/lib/adapter/aiohttp.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/lib/adapter/httpx.py` & `feedancy-0.1.5/feedancy/lib/adapter/httpx.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/lib/adapter/params_converter.py` & `feedancy-0.1.5/feedancy/lib/adapter/params_converter.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/lib/adapter/requests.py` & `feedancy-0.1.5/feedancy/lib/adapter/requests.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/lib/base.py` & `feedancy-0.1.5/feedancy/lib/base.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/lib/client.py` & `feedancy-0.1.5/feedancy/lib/client.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/lib/configuration.py` & `feedancy-0.1.5/feedancy/lib/configuration.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/lib/request.py` & `feedancy-0.1.5/feedancy/lib/request.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/lib/response_deserializer.py` & `feedancy-0.1.5/feedancy/lib/response_deserializer.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/feedancy/lib/types.py` & `feedancy-0.1.5/feedancy/lib/types.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.4/PKG-INFO` & `feedancy-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feedancy
-Version: 0.1.4
+Version: 0.1.5
 Summary: сервис по сбору вакансий
 License: MIT
 Author: Alexey Ostanin
 Author-email: aostaninn@gmal.com
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

