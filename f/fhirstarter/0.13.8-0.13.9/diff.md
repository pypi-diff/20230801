# Comparing `tmp/fhirstarter-0.13.8.tar.gz` & `tmp/fhirstarter-0.13.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fhirstarter-0.13.8.tar", max compression
+gzip compressed data, was "fhirstarter-0.13.9.tar", max compression
```

## Comparing `fhirstarter-0.13.8.tar` & `fhirstarter-0.13.9.tar`

### file list

```diff
@@ -1,172 +1,173 @@
--rw-r--r--   0        0        0     1071 2023-01-25 15:18:03.969523 fhirstarter-0.13.8/LICENSE.md
--rw-r--r--   0        0        0     6076 2023-01-25 16:41:17.839630 fhirstarter-0.13.8/README.md
--rw-r--r--   0        0        0      388 2023-01-19 20:28:46.227427 fhirstarter-0.13.8/fhirstarter/__init__.py
--rw-r--r--   0        0        0     3885 2023-02-09 16:08:24.236007 fhirstarter-0.13.8/fhirstarter/exceptions.py
--rw-r--r--   0        0        0      148 2022-09-02 16:13:21.196164 fhirstarter-0.13.8/fhirstarter/fhir_specification/__init__.py
--rw-r--r--   0        0        0     1216 2022-08-30 15:52:43.914830 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/account-example.json
--rw-r--r--   0        0        0     9898 2022-08-30 15:52:43.919849 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/activitydefinition-example.json
--rw-r--r--   0        0        0     3652 2022-08-30 15:52:43.924678 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/adverseevent-example.json
--rw-r--r--   0        0        0     6761 2022-08-30 15:52:43.930277 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/allergyintolerance-example.json
--rw-r--r--   0        0        0     2477 2022-08-30 15:52:43.937169 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/appointment-example.json
--rw-r--r--   0        0        0      654 2022-08-30 15:52:43.943319 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/appointmentresponse-example.json
--rw-r--r--   0        0        0     3080 2022-08-30 15:52:43.949392 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/auditevent-example.json
--rw-r--r--   0        0        0     2587 2022-08-30 15:52:43.955039 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/basic-example.json
--rw-r--r--   0        0        0   176064 2022-08-30 15:52:43.966340 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/binary-example.json
--rw-r--r--   0        0        0      409 2022-08-30 15:52:43.972693 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/biologicallyderivedproduct-example.json
--rw-r--r--   0        0        0     1459 2022-08-30 15:52:43.978291 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/bodystructure-example.json
--rw-r--r--   0        0        0     2364 2022-08-30 15:52:43.984348 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/bundle-example.json
--rw-r--r--   0        0        0     5930 2022-08-30 15:52:43.991165 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/capabilitystatement-example.json
--rw-r--r--   0        0        0     3597 2022-08-30 15:52:43.996869 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/careplan-example.json
--rw-r--r--   0        0        0     1767 2022-08-30 15:52:44.002022 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/careteam-example.json
--rw-r--r--   0        0        0      624 2022-08-30 15:52:44.008313 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/catalogentry-example.json
--rw-r--r--   0        0        0     2862 2022-08-30 15:52:44.014027 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/chargeitem-example.json
--rw-r--r--   0        0        0     3418 2022-08-30 15:52:44.019871 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/chargeitemdefinition-example.json
--rw-r--r--   0        0        0     2057 2022-08-30 15:52:44.025691 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/claim-example.json
--rw-r--r--   0        0        0     3631 2022-08-30 15:52:44.030893 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/claimresponse-example.json
--rw-r--r--   0        0        0     3774 2022-08-30 15:52:44.036000 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/clinicalimpression-example.json
--rw-r--r--   0        0        0     3970 2022-08-30 15:52:44.041990 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/codesystem-example.json
--rw-r--r--   0        0        0     1729 2022-08-30 15:52:44.047864 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/communication-example.json
--rw-r--r--   0        0        0      551 2022-08-30 15:52:44.052717 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/communicationrequest-example.json
--rw-r--r--   0        0        0     3674 2022-08-30 15:52:44.057949 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/compartmentdefinition-example.json
--rw-r--r--   0        0        0     5631 2022-08-30 15:52:44.062736 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/composition-example.json
--rw-r--r--   0        0        0     5377 2022-08-30 15:52:44.067640 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/conceptmap-example.json
--rw-r--r--   0        0        0     1798 2022-08-30 15:52:44.072541 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/condition-example.json
--rw-r--r--   0        0        0     1552 2022-08-30 15:52:44.077542 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/consent-example.json
--rw-r--r--   0        0        0     2085 2022-08-30 15:52:44.082554 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/contract-example.json
--rw-r--r--   0        0        0     4163 2022-08-30 15:52:44.087552 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/coverage-example.json
--rw-r--r--   0        0        0     1027 2022-08-30 15:52:44.092546 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/coverageeligibilityrequest-example.json
--rw-r--r--   0        0        0     1090 2022-08-30 15:52:44.098557 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/coverageeligibilityresponse-example.json
--rw-r--r--   0        0        0     2834 2022-08-30 15:52:44.103606 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/detectedissue-example.json
--rw-r--r--   0        0        0      701 2022-08-30 15:52:44.108516 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/device-example.json
--rw-r--r--   0        0        0      651 2022-08-30 15:52:44.113536 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/devicedefinition-example.json
--rw-r--r--   0        0        0     2998 2022-08-30 15:52:44.118529 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/devicemetric-example.json
--rw-r--r--   0        0        0     1050 2022-08-30 15:52:44.123489 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/devicerequest-example.json
--rw-r--r--   0        0        0     1422 2022-08-30 15:52:44.129521 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/deviceusestatement-example.json
--rw-r--r--   0        0        0     6944 2022-08-30 15:52:44.134490 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/diagnosticreport-example.json
--rw-r--r--   0        0        0     1640 2022-08-30 15:52:44.139915 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/documentmanifest-example.json
--rw-r--r--   0        0        0     8433 2022-08-30 15:52:44.144723 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/documentreference-example.json
--rw-r--r--   0        0        0      699 2022-08-30 15:52:44.149530 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/effectevidencesynthesis-example.json
--rw-r--r--   0        0        0      625 2022-08-30 15:52:44.154502 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/encounter-example.json
--rw-r--r--   0        0        0     1388 2022-08-30 15:52:44.159630 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/endpoint-example.json
--rw-r--r--   0        0        0      815 2022-08-30 15:52:44.164543 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/enrollmentrequest-example.json
--rw-r--r--   0        0        0      899 2022-08-30 15:52:44.169570 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/enrollmentresponse-example.json
--rw-r--r--   0        0        0     2332 2022-08-30 15:52:44.174554 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/episodeofcare-example.json
--rw-r--r--   0        0        0      991 2022-08-30 15:52:44.179542 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/eventdefinition-example.json
--rw-r--r--   0        0        0      487 2022-08-30 15:52:44.185247 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/evidence-example.json
--rw-r--r--   0        0        0      548 2022-08-30 15:52:44.190874 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/evidencevariable-example.json
--rw-r--r--   0        0        0    29430 2022-08-30 15:52:44.196200 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/examplescenario-example.json
--rw-r--r--   0        0        0     6629 2022-08-30 15:52:44.202041 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/explanationofbenefit-example.json
--rw-r--r--   0        0        0     1630 2022-08-30 15:52:44.207655 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/familymemberhistory-example.json
--rw-r--r--   0        0        0     1245 2022-08-30 15:52:44.212638 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/flag-example.json
--rw-r--r--   0        0        0     2154 2022-08-30 15:52:44.217647 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/goal-example.json
--rw-r--r--   0        0        0     3485 2022-08-30 15:52:44.222517 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/graphdefinition-example.json
--rw-r--r--   0        0        0     1113 2022-08-30 15:52:44.227445 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/group-example.json
--rw-r--r--   0        0        0     3182 2022-08-30 15:52:44.232442 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/guidanceresponse-example.json
--rw-r--r--   0        0        0     4747 2022-08-30 15:52:44.237476 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/healthcareservice-example.json
--rw-r--r--   0        0        0     1523 2022-08-30 15:52:44.242623 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/imagingstudy-example.json
--rw-r--r--   0        0        0     7176 2022-08-30 15:52:44.247964 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/immunization-example.json
--rw-r--r--   0        0        0     2620 2022-08-30 15:52:44.253554 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/immunizationevaluation-example.json
--rw-r--r--   0        0        0     2536 2022-08-30 15:52:44.258792 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/immunizationrecommendation-example.json
--rw-r--r--   0        0        0     9120 2022-08-30 15:52:44.263610 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/implementationguide-example.json
--rw-r--r--   0        0        0      607 2022-08-30 15:52:44.269048 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/insuranceplan-example.json
--rw-r--r--   0        0        0     1239 2022-08-30 15:52:44.274503 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/invoice-example.json
--rw-r--r--   0        0        0     9390 2022-08-30 15:52:44.280642 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/library-example.json
--rw-r--r--   0        0        0     1138 2022-08-30 15:52:44.286280 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/linkage-example.json
--rw-r--r--   0        0        0     2129 2022-08-30 15:52:44.291599 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/list-example.json
--rw-r--r--   0        0        0     1699 2022-08-30 15:52:44.296717 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/location-example.json
--rw-r--r--   0        0        0    16513 2022-08-30 15:52:44.301745 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/measure-example.json
--rw-r--r--   0        0        0    64009 2022-08-30 15:52:44.306667 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/measurereport-example.json
--rw-r--r--   0        0        0     6590 2022-08-30 15:52:44.312958 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/media-example.json
--rw-r--r--   0        0        0     2142 2022-08-30 15:52:44.318502 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medication-example.json
--rw-r--r--   0        0        0     4533 2022-08-30 15:52:44.324461 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medicationadministration-example.json
--rw-r--r--   0        0        0     4184 2022-08-30 15:52:44.329434 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medicationdispense-example.json
--rw-r--r--   0        0        0     2310 2022-08-30 15:52:44.334475 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medicationknowledge-example.json
--rw-r--r--   0        0        0     6390 2022-08-30 15:52:44.339470 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medicationrequest-example.json
--rw-r--r--   0        0        0     5865 2022-08-30 15:52:44.344399 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medicationstatement-example.json
--rw-r--r--   0        0        0     6646 2022-08-30 15:52:44.349460 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medicinalproduct-example.json
--rw-r--r--   0        0        0     5755 2022-08-30 15:52:44.354417 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medicinalproductauthorization-example.json
--rw-r--r--   0        0        0     1690 2022-08-30 15:52:44.359366 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medicinalproductcontraindication-example.json
--rw-r--r--   0        0        0     3236 2022-08-30 15:52:44.364408 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medicinalproductindication-example.json
--rw-r--r--   0        0        0     3181 2022-08-30 15:52:44.369343 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medicinalproductingredient-example.json
--rw-r--r--   0        0        0     5478 2022-08-30 15:52:44.374667 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medicinalproductinteraction-example.json
--rw-r--r--   0        0        0     2096 2022-08-30 15:52:44.379989 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medicinalproductmanufactured-example.json
--rw-r--r--   0        0        0     5966 2022-08-30 15:52:44.385555 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medicinalproductpackaged-example.json
--rw-r--r--   0        0        0     2454 2022-08-30 15:52:44.390624 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medicinalproductpharmaceutical-example.json
--rw-r--r--   0        0        0     2137 2022-08-30 15:52:44.395562 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medicinalproductundesirableeffect-example.json
--rw-r--r--   0        0        0      824 2022-08-30 15:52:44.401466 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/messagedefinition-example.json
--rw-r--r--   0        0        0     1755 2022-08-30 15:52:44.407690 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/messageheader-example.json
--rw-r--r--   0        0        0     3547 2022-08-30 15:52:44.413801 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/molecularsequence-example.json
--rw-r--r--   0        0        0     1894 2022-08-30 15:52:44.419611 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/namingsystem-example.json
--rw-r--r--   0        0        0     3554 2022-08-30 15:52:44.424809 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/nutritionorder-example.json
--rw-r--r--   0        0        0     2949 2022-11-07 16:57:04.761702 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/observation-example.json
--rw-r--r--   0        0        0      982 2022-08-30 15:52:44.436677 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/observationdefinition-example.json
--rw-r--r--   0        0        0     7234 2022-08-30 15:52:44.441379 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/operationdefinition-example.json
--rw-r--r--   0        0        0      880 2022-08-30 15:52:44.446343 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/operationoutcome-example.json
--rw-r--r--   0        0        0     1397 2022-08-30 15:52:44.451403 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/organization-example.json
--rw-r--r--   0        0        0     1748 2022-08-30 15:52:44.456447 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/organizationaffiliation-example.json
--rw-r--r--   0        0        0      847 2022-08-30 15:52:44.461895 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/parameters-example.json
--rw-r--r--   0        0        0     4270 2022-08-30 15:52:44.467481 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/patient-example.json
--rw-r--r--   0        0        0     1296 2022-08-30 15:52:44.472966 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/paymentnotice-example.json
--rw-r--r--   0        0        0     3381 2022-08-30 15:52:44.478703 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/paymentreconciliation-example.json
--rw-r--r--   0        0        0     2610 2022-08-30 15:52:44.483604 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/person-example.json
--rw-r--r--   0        0        0    53475 2022-08-30 15:52:44.488802 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/plandefinition-example.json
--rw-r--r--   0        0        0     1522 2022-08-30 15:52:44.494902 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/practitioner-example.json
--rw-r--r--   0        0        0     2403 2022-08-30 15:52:44.500378 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/practitionerrole-example.json
--rw-r--r--   0        0        0     1367 2022-08-30 15:52:44.505730 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/procedure-example.json
--rw-r--r--   0        0        0     1791 2022-08-30 15:52:44.511380 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/provenance-example.json
--rw-r--r--   0        0        0     5008 2022-08-30 15:52:44.516677 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/questionnaire-example.json
--rw-r--r--   0        0        0     3983 2022-08-30 15:52:44.521671 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/questionnaireresponse-example.json
--rw-r--r--   0        0        0     2265 2022-08-30 15:52:44.527161 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/relatedperson-example.json
--rw-r--r--   0        0        0     3201 2022-08-30 15:52:44.533564 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/requestgroup-example.json
--rw-r--r--   0        0        0      498 2022-08-30 15:52:44.538791 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/researchdefinition-example.json
--rw-r--r--   0        0        0      581 2022-08-30 15:52:44.544528 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/researchelementdefinition-example.json
--rw-r--r--   0        0        0      421 2022-08-30 15:52:44.549419 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/researchstudy-example.json
--rw-r--r--   0        0        0      704 2022-08-30 15:52:44.554478 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/researchsubject-example.json
--rw-r--r--   0        0        0     5755 2022-08-30 15:52:44.560988 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/riskassessment-example.json
--rw-r--r--   0        0        0      556 2022-08-30 15:52:44.566676 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/riskevidencesynthesis-example.json
--rw-r--r--   0        0        0     1369 2022-08-30 15:52:44.571722 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/schedule-example.json
--rw-r--r--   0        0        0     3814 2022-08-30 15:52:44.577444 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/searchparameter-example.json
--rw-r--r--   0        0        0      917 2022-08-30 15:52:44.582378 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/servicerequest-example.json
--rw-r--r--   0        0        0     1358 2022-08-30 15:52:44.587344 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/slot-example.json
--rw-r--r--   0        0        0     5623 2022-08-30 15:52:44.592354 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/specimen-example.json
--rw-r--r--   0        0        0     9978 2022-08-30 15:52:44.597498 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/specimendefinition-example.json
--rw-r--r--   0        0        0   214410 2022-08-30 15:52:44.604373 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/structureddefinition-example.json
--rw-r--r--   0        0        0     4902 2022-08-30 15:52:44.614542 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/structuremap-example.json
--rw-r--r--   0        0        0      880 2022-08-30 15:52:44.628318 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/subscription-example.json
--rw-r--r--   0        0        0     1468 2022-08-30 15:52:44.633460 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/substance-example.json
--rw-r--r--   0        0        0      536 2022-08-30 15:52:44.638798 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/substancenucleicacid-example.json
--rw-r--r--   0        0        0      536 2022-08-30 15:52:44.639220 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/substancepolymer-example.json
--rw-r--r--   0        0        0      536 2022-08-30 15:52:44.639533 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/substanceprotein-example.json
--rw-r--r--   0        0        0      536 2022-08-30 15:52:44.639838 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/substancereferenceinformation-example.json
--rw-r--r--   0        0        0      253 2022-08-30 15:52:44.645463 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/substancesourcematerial-example.json
--rw-r--r--   0        0        0      536 2022-08-30 15:52:44.645807 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/substancespecification-example.json
--rw-r--r--   0        0        0     2730 2022-08-30 15:52:44.651360 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/supplydelivery-example.json
--rw-r--r--   0        0        0     1933 2022-08-30 15:52:44.656258 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/supplyrequest-example.json
--rw-r--r--   0        0        0     5629 2022-08-30 15:52:44.661239 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/task-example.json
--rw-r--r--   0        0        0     1572 2022-08-30 15:52:44.667194 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/terminologycapabilities-example.json
--rw-r--r--   0        0        0    12159 2022-08-30 15:52:44.672226 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/testreport-example.json
--rw-r--r--   0        0        0    26297 2022-08-30 15:52:44.677517 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/testscript-example.json
--rw-r--r--   0        0        0     3483 2022-08-30 15:52:44.682322 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/valueset-example.json
--rw-r--r--   0        0        0      626 2022-08-30 15:52:44.687186 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/verificationresult-example.json
--rw-r--r--   0        0        0     1675 2022-08-30 15:52:44.692236 fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/visionprescription-example.json
--rw-r--r--   0        0        0  2143339 2022-08-30 15:52:44.696052 fhirstarter-0.13.8/fhirstarter/fhir_specification/search-parameters.json
--rw-r--r--   0        0        0     5484 2023-04-14 21:58:34.380591 fhirstarter-0.13.8/fhirstarter/fhir_specification/utils.py
--rw-r--r--   0        0        0    26504 2023-04-17 15:08:58.537605 fhirstarter-0.13.8/fhirstarter/fhirstarter.py
--rw-r--r--   0        0        0    10222 2023-01-24 20:53:50.967128 fhirstarter-0.13.8/fhirstarter/functions.py
--rw-r--r--   0        0        0     3462 2022-08-16 17:25:05.513384 fhirstarter-0.13.8/fhirstarter/interactions.py
--rw-r--r--   0        0        0     4555 2022-08-16 17:25:05.518559 fhirstarter-0.13.8/fhirstarter/providers.py
--rw-r--r--   0        0        0      151 2023-04-17 15:15:02.746821 fhirstarter-0.13.8/fhirstarter/scripts/config.toml
--rw-r--r--   0        0        0     3991 2023-04-17 15:15:02.747862 fhirstarter-0.13.8/fhirstarter/scripts/example.py
--rw-r--r--   0        0        0     8418 2023-04-14 21:58:34.387998 fhirstarter-0.13.8/fhirstarter/search_parameters.py
--rw-r--r--   0        0        0       68 2022-06-21 20:10:12.695171 fhirstarter-0.13.8/fhirstarter/testclient.py
--rw-r--r--   0        0        0        0 2022-08-30 15:52:44.718623 fhirstarter-0.13.8/fhirstarter/tests/__init__.py
--rw-r--r--   0        0        0     3332 2022-12-21 18:32:08.313039 fhirstarter-0.13.8/fhirstarter/tests/config.py
--rw-r--r--   0        0        0      814 2023-01-19 20:28:46.262143 fhirstarter-0.13.8/fhirstarter/tests/conftest.py
--rw-r--r--   0        0        0     6049 2023-01-19 20:28:46.268247 fhirstarter-0.13.8/fhirstarter/tests/test_capability_statement.py
--rw-r--r--   0        0        0     2435 2022-12-21 18:32:08.328730 fhirstarter-0.13.8/fhirstarter/tests/test_dependencies.py
--rw-r--r--   0        0        0     5531 2023-01-19 20:28:46.275371 fhirstarter-0.13.8/fhirstarter/tests/test_errors.py
--rw-r--r--   0        0        0    10467 2023-01-19 20:28:46.280291 fhirstarter-0.13.8/fhirstarter/tests/test_interactions.py
--rw-r--r--   0        0        0     1675 2022-09-26 19:04:22.813330 fhirstarter-0.13.8/fhirstarter/tests/utils.py
--rw-r--r--   0        0        0    14681 2023-03-30 15:52:16.307271 fhirstarter-0.13.8/fhirstarter/utils.py
--rw-r--r--   0        0        0     2377 2023-04-14 21:58:34.389073 fhirstarter-0.13.8/pyproject.toml
--rw-r--r--   0        0        0     7863 1970-01-01 00:00:00.000000 fhirstarter-0.13.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-01-25 15:18:03.969523 fhirstarter-0.13.9/LICENSE.md
+-rw-r--r--   0        0        0     6076 2023-01-25 16:41:17.839630 fhirstarter-0.13.9/README.md
+-rw-r--r--   0        0        0      388 2023-07-28 02:58:19.651849 fhirstarter-0.13.9/fhirstarter/__init__.py
+-rw-r--r--   0        0        0     3928 2023-08-01 20:37:57.327357 fhirstarter-0.13.9/fhirstarter/exceptions.py
+-rw-r--r--   0        0        0      148 2022-09-02 16:13:21.196164 fhirstarter-0.13.9/fhirstarter/fhir_specification/__init__.py
+-rw-r--r--   0        0        0     1216 2022-08-30 15:52:43.914830 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/account-example.json
+-rw-r--r--   0        0        0     9898 2022-08-30 15:52:43.919849 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/activitydefinition-example.json
+-rw-r--r--   0        0        0     3652 2022-08-30 15:52:43.924678 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/adverseevent-example.json
+-rw-r--r--   0        0        0     6761 2022-08-30 15:52:43.930277 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/allergyintolerance-example.json
+-rw-r--r--   0        0        0     2477 2022-08-30 15:52:43.937169 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/appointment-example.json
+-rw-r--r--   0        0        0      654 2022-08-30 15:52:43.943319 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/appointmentresponse-example.json
+-rw-r--r--   0        0        0     3080 2022-08-30 15:52:43.949392 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/auditevent-example.json
+-rw-r--r--   0        0        0     2587 2022-08-30 15:52:43.955039 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/basic-example.json
+-rw-r--r--   0        0        0   176064 2022-08-30 15:52:43.966340 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/binary-example.json
+-rw-r--r--   0        0        0      409 2022-08-30 15:52:43.972693 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/biologicallyderivedproduct-example.json
+-rw-r--r--   0        0        0     1459 2022-08-30 15:52:43.978291 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/bodystructure-example.json
+-rw-r--r--   0        0        0     2364 2022-08-30 15:52:43.984348 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/bundle-example.json
+-rw-r--r--   0        0        0     5930 2022-08-30 15:52:43.991165 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/capabilitystatement-example.json
+-rw-r--r--   0        0        0     3597 2022-08-30 15:52:43.996869 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/careplan-example.json
+-rw-r--r--   0        0        0     1767 2022-08-30 15:52:44.002022 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/careteam-example.json
+-rw-r--r--   0        0        0      624 2022-08-30 15:52:44.008313 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/catalogentry-example.json
+-rw-r--r--   0        0        0     2862 2022-08-30 15:52:44.014027 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/chargeitem-example.json
+-rw-r--r--   0        0        0     3418 2022-08-30 15:52:44.019871 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/chargeitemdefinition-example.json
+-rw-r--r--   0        0        0     2057 2022-08-30 15:52:44.025691 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/claim-example.json
+-rw-r--r--   0        0        0     3631 2022-08-30 15:52:44.030893 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/claimresponse-example.json
+-rw-r--r--   0        0        0     3774 2022-08-30 15:52:44.036000 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/clinicalimpression-example.json
+-rw-r--r--   0        0        0     3970 2022-08-30 15:52:44.041990 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/codesystem-example.json
+-rw-r--r--   0        0        0     1729 2022-08-30 15:52:44.047864 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/communication-example.json
+-rw-r--r--   0        0        0      551 2022-08-30 15:52:44.052717 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/communicationrequest-example.json
+-rw-r--r--   0        0        0     3674 2022-08-30 15:52:44.057949 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/compartmentdefinition-example.json
+-rw-r--r--   0        0        0     5631 2022-08-30 15:52:44.062736 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/composition-example.json
+-rw-r--r--   0        0        0     5377 2022-08-30 15:52:44.067640 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/conceptmap-example.json
+-rw-r--r--   0        0        0     1798 2022-08-30 15:52:44.072541 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/condition-example.json
+-rw-r--r--   0        0        0     1552 2022-08-30 15:52:44.077542 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/consent-example.json
+-rw-r--r--   0        0        0     2085 2022-08-30 15:52:44.082554 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/contract-example.json
+-rw-r--r--   0        0        0     4163 2022-08-30 15:52:44.087552 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/coverage-example.json
+-rw-r--r--   0        0        0     1027 2022-08-30 15:52:44.092546 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/coverageeligibilityrequest-example.json
+-rw-r--r--   0        0        0     1090 2022-08-30 15:52:44.098557 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/coverageeligibilityresponse-example.json
+-rw-r--r--   0        0        0     2834 2022-08-30 15:52:44.103606 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/detectedissue-example.json
+-rw-r--r--   0        0        0      701 2022-08-30 15:52:44.108516 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/device-example.json
+-rw-r--r--   0        0        0      651 2022-08-30 15:52:44.113536 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/devicedefinition-example.json
+-rw-r--r--   0        0        0     2998 2022-08-30 15:52:44.118529 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/devicemetric-example.json
+-rw-r--r--   0        0        0     1050 2022-08-30 15:52:44.123489 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/devicerequest-example.json
+-rw-r--r--   0        0        0     1422 2022-08-30 15:52:44.129521 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/deviceusestatement-example.json
+-rw-r--r--   0        0        0     6944 2022-08-30 15:52:44.134490 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/diagnosticreport-example.json
+-rw-r--r--   0        0        0     1640 2022-08-30 15:52:44.139915 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/documentmanifest-example.json
+-rw-r--r--   0        0        0     8433 2022-08-30 15:52:44.144723 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/documentreference-example.json
+-rw-r--r--   0        0        0      699 2022-08-30 15:52:44.149530 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/effectevidencesynthesis-example.json
+-rw-r--r--   0        0        0      625 2022-08-30 15:52:44.154502 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/encounter-example.json
+-rw-r--r--   0        0        0     1388 2022-08-30 15:52:44.159630 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/endpoint-example.json
+-rw-r--r--   0        0        0      815 2022-08-30 15:52:44.164543 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/enrollmentrequest-example.json
+-rw-r--r--   0        0        0      899 2022-08-30 15:52:44.169570 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/enrollmentresponse-example.json
+-rw-r--r--   0        0        0     2332 2022-08-30 15:52:44.174554 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/episodeofcare-example.json
+-rw-r--r--   0        0        0      991 2022-08-30 15:52:44.179542 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/eventdefinition-example.json
+-rw-r--r--   0        0        0      487 2022-08-30 15:52:44.185247 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/evidence-example.json
+-rw-r--r--   0        0        0      548 2022-08-30 15:52:44.190874 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/evidencevariable-example.json
+-rw-r--r--   0        0        0    29430 2022-08-30 15:52:44.196200 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/examplescenario-example.json
+-rw-r--r--   0        0        0     6629 2022-08-30 15:52:44.202041 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/explanationofbenefit-example.json
+-rw-r--r--   0        0        0     1630 2022-08-30 15:52:44.207655 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/familymemberhistory-example.json
+-rw-r--r--   0        0        0     1245 2022-08-30 15:52:44.212638 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/flag-example.json
+-rw-r--r--   0        0        0     2154 2022-08-30 15:52:44.217647 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/goal-example.json
+-rw-r--r--   0        0        0     3485 2022-08-30 15:52:44.222517 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/graphdefinition-example.json
+-rw-r--r--   0        0        0     1113 2022-08-30 15:52:44.227445 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/group-example.json
+-rw-r--r--   0        0        0     3182 2022-08-30 15:52:44.232442 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/guidanceresponse-example.json
+-rw-r--r--   0        0        0     4747 2022-08-30 15:52:44.237476 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/healthcareservice-example.json
+-rw-r--r--   0        0        0     1523 2022-08-30 15:52:44.242623 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/imagingstudy-example.json
+-rw-r--r--   0        0        0     7176 2022-08-30 15:52:44.247964 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/immunization-example.json
+-rw-r--r--   0        0        0     2620 2022-08-30 15:52:44.253554 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/immunizationevaluation-example.json
+-rw-r--r--   0        0        0     2536 2022-08-30 15:52:44.258792 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/immunizationrecommendation-example.json
+-rw-r--r--   0        0        0     9120 2022-08-30 15:52:44.263610 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/implementationguide-example.json
+-rw-r--r--   0        0        0      607 2022-08-30 15:52:44.269048 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/insuranceplan-example.json
+-rw-r--r--   0        0        0     1239 2022-08-30 15:52:44.274503 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/invoice-example.json
+-rw-r--r--   0        0        0     9390 2022-08-30 15:52:44.280642 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/library-example.json
+-rw-r--r--   0        0        0     1138 2022-08-30 15:52:44.286280 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/linkage-example.json
+-rw-r--r--   0        0        0     2129 2022-08-30 15:52:44.291599 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/list-example.json
+-rw-r--r--   0        0        0     1699 2022-08-30 15:52:44.296717 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/location-example.json
+-rw-r--r--   0        0        0    16513 2022-08-30 15:52:44.301745 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/measure-example.json
+-rw-r--r--   0        0        0    64009 2022-08-30 15:52:44.306667 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/measurereport-example.json
+-rw-r--r--   0        0        0     6590 2022-08-30 15:52:44.312958 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/media-example.json
+-rw-r--r--   0        0        0     2142 2022-08-30 15:52:44.318502 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medication-example.json
+-rw-r--r--   0        0        0     4533 2022-08-30 15:52:44.324461 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicationadministration-example.json
+-rw-r--r--   0        0        0     4184 2022-08-30 15:52:44.329434 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicationdispense-example.json
+-rw-r--r--   0        0        0     2310 2022-08-30 15:52:44.334475 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicationknowledge-example.json
+-rw-r--r--   0        0        0     6390 2022-08-30 15:52:44.339470 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicationrequest-example.json
+-rw-r--r--   0        0        0     5865 2022-08-30 15:52:44.344399 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicationstatement-example.json
+-rw-r--r--   0        0        0     6646 2022-08-30 15:52:44.349460 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicinalproduct-example.json
+-rw-r--r--   0        0        0     5755 2022-08-30 15:52:44.354417 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicinalproductauthorization-example.json
+-rw-r--r--   0        0        0     1690 2022-08-30 15:52:44.359366 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicinalproductcontraindication-example.json
+-rw-r--r--   0        0        0     3236 2022-08-30 15:52:44.364408 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicinalproductindication-example.json
+-rw-r--r--   0        0        0     3181 2022-08-30 15:52:44.369343 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicinalproductingredient-example.json
+-rw-r--r--   0        0        0     5478 2022-08-30 15:52:44.374667 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicinalproductinteraction-example.json
+-rw-r--r--   0        0        0     2096 2022-08-30 15:52:44.379989 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicinalproductmanufactured-example.json
+-rw-r--r--   0        0        0     5966 2022-08-30 15:52:44.385555 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicinalproductpackaged-example.json
+-rw-r--r--   0        0        0     2454 2022-08-30 15:52:44.390624 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicinalproductpharmaceutical-example.json
+-rw-r--r--   0        0        0     2137 2022-08-30 15:52:44.395562 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicinalproductundesirableeffect-example.json
+-rw-r--r--   0        0        0      824 2022-08-30 15:52:44.401466 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/messagedefinition-example.json
+-rw-r--r--   0        0        0     1755 2022-08-30 15:52:44.407690 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/messageheader-example.json
+-rw-r--r--   0        0        0     3547 2022-08-30 15:52:44.413801 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/molecularsequence-example.json
+-rw-r--r--   0        0        0     1894 2022-08-30 15:52:44.419611 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/namingsystem-example.json
+-rw-r--r--   0        0        0     3554 2022-08-30 15:52:44.424809 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/nutritionorder-example.json
+-rw-r--r--   0        0        0     2949 2022-11-07 16:57:04.761702 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/observation-example.json
+-rw-r--r--   0        0        0      982 2022-08-30 15:52:44.436677 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/observationdefinition-example.json
+-rw-r--r--   0        0        0     7234 2022-08-30 15:52:44.441379 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/operationdefinition-example.json
+-rw-r--r--   0        0        0      880 2022-08-30 15:52:44.446343 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/operationoutcome-example.json
+-rw-r--r--   0        0        0     1397 2022-08-30 15:52:44.451403 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/organization-example.json
+-rw-r--r--   0        0        0     1748 2022-08-30 15:52:44.456447 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/organizationaffiliation-example.json
+-rw-r--r--   0        0        0      847 2022-08-30 15:52:44.461895 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/parameters-example.json
+-rw-r--r--   0        0        0     4270 2022-08-30 15:52:44.467481 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/patient-example.json
+-rw-r--r--   0        0        0     1296 2022-08-30 15:52:44.472966 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/paymentnotice-example.json
+-rw-r--r--   0        0        0     3381 2022-08-30 15:52:44.478703 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/paymentreconciliation-example.json
+-rw-r--r--   0        0        0     2610 2022-08-30 15:52:44.483604 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/person-example.json
+-rw-r--r--   0        0        0    53475 2022-08-30 15:52:44.488802 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/plandefinition-example.json
+-rw-r--r--   0        0        0     1522 2022-08-30 15:52:44.494902 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/practitioner-example.json
+-rw-r--r--   0        0        0     2403 2022-08-30 15:52:44.500378 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/practitionerrole-example.json
+-rw-r--r--   0        0        0     1367 2022-08-30 15:52:44.505730 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/procedure-example.json
+-rw-r--r--   0        0        0     1791 2022-08-30 15:52:44.511380 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/provenance-example.json
+-rw-r--r--   0        0        0     5008 2022-08-30 15:52:44.516677 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/questionnaire-example.json
+-rw-r--r--   0        0        0     3983 2022-08-30 15:52:44.521671 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/questionnaireresponse-example.json
+-rw-r--r--   0        0        0     2265 2022-08-30 15:52:44.527161 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/relatedperson-example.json
+-rw-r--r--   0        0        0     3201 2022-08-30 15:52:44.533564 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/requestgroup-example.json
+-rw-r--r--   0        0        0      498 2022-08-30 15:52:44.538791 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/researchdefinition-example.json
+-rw-r--r--   0        0        0      581 2022-08-30 15:52:44.544528 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/researchelementdefinition-example.json
+-rw-r--r--   0        0        0      421 2022-08-30 15:52:44.549419 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/researchstudy-example.json
+-rw-r--r--   0        0        0      704 2022-08-30 15:52:44.554478 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/researchsubject-example.json
+-rw-r--r--   0        0        0     5755 2022-08-30 15:52:44.560988 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/riskassessment-example.json
+-rw-r--r--   0        0        0      556 2022-08-30 15:52:44.566676 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/riskevidencesynthesis-example.json
+-rw-r--r--   0        0        0     1369 2022-08-30 15:52:44.571722 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/schedule-example.json
+-rw-r--r--   0        0        0     3814 2022-08-30 15:52:44.577444 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/searchparameter-example.json
+-rw-r--r--   0        0        0      917 2022-08-30 15:52:44.582378 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/servicerequest-example.json
+-rw-r--r--   0        0        0     1358 2022-08-30 15:52:44.587344 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/slot-example.json
+-rw-r--r--   0        0        0     5623 2022-08-30 15:52:44.592354 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/specimen-example.json
+-rw-r--r--   0        0        0     9978 2022-08-30 15:52:44.597498 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/specimendefinition-example.json
+-rw-r--r--   0        0        0   214410 2022-08-30 15:52:44.604373 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/structureddefinition-example.json
+-rw-r--r--   0        0        0     4902 2022-08-30 15:52:44.614542 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/structuremap-example.json
+-rw-r--r--   0        0        0      880 2022-08-30 15:52:44.628318 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/subscription-example.json
+-rw-r--r--   0        0        0     1468 2022-08-30 15:52:44.633460 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/substance-example.json
+-rw-r--r--   0        0        0      536 2022-08-30 15:52:44.638798 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/substancenucleicacid-example.json
+-rw-r--r--   0        0        0      536 2022-08-30 15:52:44.639220 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/substancepolymer-example.json
+-rw-r--r--   0        0        0      536 2022-08-30 15:52:44.639533 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/substanceprotein-example.json
+-rw-r--r--   0        0        0      536 2022-08-30 15:52:44.639838 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/substancereferenceinformation-example.json
+-rw-r--r--   0        0        0      253 2022-08-30 15:52:44.645463 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/substancesourcematerial-example.json
+-rw-r--r--   0        0        0      536 2022-08-30 15:52:44.645807 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/substancespecification-example.json
+-rw-r--r--   0        0        0     2730 2022-08-30 15:52:44.651360 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/supplydelivery-example.json
+-rw-r--r--   0        0        0     1933 2022-08-30 15:52:44.656258 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/supplyrequest-example.json
+-rw-r--r--   0        0        0     5629 2022-08-30 15:52:44.661239 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/task-example.json
+-rw-r--r--   0        0        0     1572 2022-08-30 15:52:44.667194 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/terminologycapabilities-example.json
+-rw-r--r--   0        0        0    12159 2022-08-30 15:52:44.672226 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/testreport-example.json
+-rw-r--r--   0        0        0    26297 2022-08-30 15:52:44.677517 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/testscript-example.json
+-rw-r--r--   0        0        0     3483 2022-08-30 15:52:44.682322 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/valueset-example.json
+-rw-r--r--   0        0        0      626 2022-08-30 15:52:44.687186 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/verificationresult-example.json
+-rw-r--r--   0        0        0     1675 2022-08-30 15:52:44.692236 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/visionprescription-example.json
+-rw-r--r--   0        0        0  2143339 2022-08-30 15:52:44.696052 fhirstarter-0.13.9/fhirstarter/fhir_specification/search-parameters.json
+-rw-r--r--   0        0        0     5484 2023-04-17 15:18:28.275081 fhirstarter-0.13.9/fhirstarter/fhir_specification/utils.py
+-rw-r--r--   0        0        0    26608 2023-08-01 20:37:57.329562 fhirstarter-0.13.9/fhirstarter/fhirstarter.py
+-rw-r--r--   0        0        0    10222 2023-01-24 20:53:50.967128 fhirstarter-0.13.9/fhirstarter/functions.py
+-rw-r--r--   0        0        0     3462 2022-08-16 17:25:05.513384 fhirstarter-0.13.9/fhirstarter/interactions.py
+-rw-r--r--   0        0        0     4555 2022-08-16 17:25:05.518559 fhirstarter-0.13.9/fhirstarter/providers.py
+-rw-r--r--   0        0        0      151 2023-04-17 15:15:02.746821 fhirstarter-0.13.9/fhirstarter/scripts/config.toml
+-rw-r--r--   0        0        0     3991 2023-07-31 15:56:50.467585 fhirstarter-0.13.9/fhirstarter/scripts/example.py
+-rw-r--r--   0        0        0     8419 2023-08-01 20:37:57.352997 fhirstarter-0.13.9/fhirstarter/search_parameters.py
+-rw-r--r--   0        0        0       68 2022-06-21 20:10:12.695171 fhirstarter-0.13.9/fhirstarter/testclient.py
+-rw-r--r--   0        0        0        0 2022-08-30 15:52:44.718623 fhirstarter-0.13.9/fhirstarter/tests/__init__.py
+-rw-r--r--   0        0        0     3332 2023-07-31 14:50:49.081727 fhirstarter-0.13.9/fhirstarter/tests/config.py
+-rw-r--r--   0        0        0      814 2023-07-31 14:50:49.054804 fhirstarter-0.13.9/fhirstarter/tests/conftest.py
+-rw-r--r--   0        0        0     6049 2023-07-31 14:50:49.077560 fhirstarter-0.13.9/fhirstarter/tests/test_capability_statement.py
+-rw-r--r--   0        0        0     2435 2023-07-31 14:50:49.085971 fhirstarter-0.13.9/fhirstarter/tests/test_dependencies.py
+-rw-r--r--   0        0        0     5531 2023-07-31 14:50:49.091215 fhirstarter-0.13.9/fhirstarter/tests/test_errors.py
+-rw-r--r--   0        0        0    10467 2023-07-31 14:50:49.060925 fhirstarter-0.13.9/fhirstarter/tests/test_interactions.py
+-rw-r--r--   0        0        0     5315 2023-08-01 20:37:57.356357 fhirstarter-0.13.9/fhirstarter/tests/test_utils.py
+-rw-r--r--   0        0        0     2363 2023-08-01 20:37:57.359406 fhirstarter-0.13.9/fhirstarter/tests/utils.py
+-rw-r--r--   0        0        0    17019 2023-08-01 20:37:57.363539 fhirstarter-0.13.9/fhirstarter/utils.py
+-rw-r--r--   0        0        0     2397 2023-08-01 20:45:04.714000 fhirstarter-0.13.9/pyproject.toml
+-rw-r--r--   0        0        0     7812 1970-01-01 00:00:00.000000 fhirstarter-0.13.9/PKG-INFO
```

### Comparing `fhirstarter-0.13.8/LICENSE.md` & `fhirstarter-0.13.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/README.md` & `fhirstarter-0.13.9/README.md`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/exceptions.py` & `fhirstarter-0.13.9/fhirstarter/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from abc import ABC, abstractmethod
 
 from fastapi import Request, status
 from fastapi.exceptions import HTTPException
 from fhir.resources.operationoutcome import OperationOutcome
 
-from .utils import make_operation_outcome
+from .utils import make_operation_outcome, parse_fhir_request
 
 
 class FHIRException(HTTPException, ABC):
     """
     Abstract base class for all FHIR exceptions.
 
     This class provides a set_request method that provides concrete subclasses with the request
@@ -100,19 +100,20 @@
     """FHIR exception class for 404 not found errors."""
 
     def __init__(self) -> None:
         super().__init__(status.HTTP_404_NOT_FOUND)
 
     def operation_outcome(self) -> OperationOutcome:
         try:
-            _, resource_type_str, id_ = self._request.url.components.path.split("/")  # type: ignore
+            interaction_info = parse_fhir_request(self._request)
         except Exception as exception:
             raise AssertionError(
-                "Unable to get resource type and resource ID from request; request must be set"
+                "Unable to get resource type and resource ID from request; request must be set "
                 "before the response is created"
             ) from exception
         else:
             return make_operation_outcome(
                 "error",
                 "not-found",
-                f"Unknown {resource_type_str} resource '{id_}'",
+                f"Unknown {interaction_info.resource_type} resource "
+                f"'{interaction_info.resource_id}'",
             )
```

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/account-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/account-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/activitydefinition-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/activitydefinition-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/adverseevent-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/adverseevent-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/allergyintolerance-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/allergyintolerance-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/appointment-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/appointment-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/appointmentresponse-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/appointmentresponse-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/auditevent-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/auditevent-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/basic-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/basic-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/binary-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/binary-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/bodystructure-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/bodystructure-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/bundle-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/bundle-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/capabilitystatement-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/capabilitystatement-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/careplan-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/careplan-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/careteam-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/careteam-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/catalogentry-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/catalogentry-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/chargeitem-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/chargeitem-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/chargeitemdefinition-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/chargeitemdefinition-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/claim-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/claim-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/claimresponse-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/claimresponse-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/clinicalimpression-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/clinicalimpression-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/codesystem-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/codesystem-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/communication-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/communication-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/communicationrequest-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/communicationrequest-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/compartmentdefinition-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/compartmentdefinition-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/composition-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/composition-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/conceptmap-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/conceptmap-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/condition-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/condition-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/consent-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/consent-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/contract-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/contract-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/coverage-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/coverage-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/coverageeligibilityrequest-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/coverageeligibilityrequest-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/coverageeligibilityresponse-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/coverageeligibilityresponse-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/detectedissue-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/detectedissue-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/device-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/device-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/devicedefinition-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/devicedefinition-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/devicemetric-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/devicemetric-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/devicerequest-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/devicerequest-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/deviceusestatement-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/deviceusestatement-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/diagnosticreport-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/diagnosticreport-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/documentmanifest-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/documentmanifest-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/documentreference-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/documentreference-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/effectevidencesynthesis-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/effectevidencesynthesis-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/encounter-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/encounter-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/endpoint-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/endpoint-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/enrollmentrequest-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/enrollmentrequest-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/enrollmentresponse-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/enrollmentresponse-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/episodeofcare-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/episodeofcare-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/eventdefinition-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/eventdefinition-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/evidencevariable-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/evidencevariable-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/examplescenario-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/examplescenario-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/explanationofbenefit-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/explanationofbenefit-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/familymemberhistory-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/familymemberhistory-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/flag-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/flag-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/goal-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/goal-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/graphdefinition-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/graphdefinition-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/group-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/group-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/guidanceresponse-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/guidanceresponse-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/healthcareservice-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/healthcareservice-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/imagingstudy-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/imagingstudy-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/immunization-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/immunization-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/immunizationevaluation-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/immunizationevaluation-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/immunizationrecommendation-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/immunizationrecommendation-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/implementationguide-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/implementationguide-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/insuranceplan-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/insuranceplan-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/invoice-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/invoice-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/library-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/library-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/linkage-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/linkage-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/list-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/list-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/location-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/location-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/measure-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/measure-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/measurereport-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/measurereport-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/media-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/media-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medication-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medication-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medicationadministration-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicationadministration-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medicationdispense-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicationdispense-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medicationknowledge-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicationknowledge-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medicationrequest-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicationrequest-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medicationstatement-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicationstatement-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medicinalproduct-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicinalproduct-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medicinalproductauthorization-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicinalproductauthorization-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medicinalproductcontraindication-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicinalproductcontraindication-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medicinalproductindication-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicinalproductindication-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medicinalproductingredient-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicinalproductingredient-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medicinalproductinteraction-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicinalproductinteraction-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medicinalproductmanufactured-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicinalproductmanufactured-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medicinalproductpackaged-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicinalproductpackaged-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medicinalproductpharmaceutical-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicinalproductpharmaceutical-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/medicinalproductundesirableeffect-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicinalproductundesirableeffect-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/messagedefinition-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/messagedefinition-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/messageheader-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/messageheader-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/molecularsequence-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/molecularsequence-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/namingsystem-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/namingsystem-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/nutritionorder-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/nutritionorder-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/observation-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/observation-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/observationdefinition-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/observationdefinition-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/operationdefinition-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/operationdefinition-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/operationoutcome-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/operationoutcome-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/organization-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/organization-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/organizationaffiliation-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/organizationaffiliation-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/parameters-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/parameters-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/patient-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/patient-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/paymentnotice-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/paymentnotice-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/paymentreconciliation-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/paymentreconciliation-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/person-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/person-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/plandefinition-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/plandefinition-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/practitioner-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/practitioner-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/practitionerrole-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/practitionerrole-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/procedure-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/procedure-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/provenance-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/provenance-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/questionnaire-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/questionnaire-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/questionnaireresponse-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/questionnaireresponse-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/relatedperson-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/relatedperson-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/requestgroup-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/requestgroup-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/researchelementdefinition-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/researchelementdefinition-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/researchsubject-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/researchsubject-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/riskassessment-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/riskassessment-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/riskevidencesynthesis-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/riskevidencesynthesis-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/schedule-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/schedule-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/searchparameter-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/searchparameter-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/servicerequest-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/servicerequest-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/slot-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/slot-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/specimen-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/specimen-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/specimendefinition-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/specimendefinition-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/structureddefinition-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/structureddefinition-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/structuremap-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/structuremap-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/subscription-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/subscription-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/substance-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/substance-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/substancenucleicacid-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/substancenucleicacid-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/substancepolymer-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/substancepolymer-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/substanceprotein-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/substanceprotein-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/substancereferenceinformation-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/substancereferenceinformation-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/substancespecification-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/substancespecification-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/supplydelivery-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/supplydelivery-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/supplyrequest-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/supplyrequest-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/task-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/task-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/terminologycapabilities-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/terminologycapabilities-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/testreport-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/testreport-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/testscript-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/testscript-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/valueset-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/valueset-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/verificationresult-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/verificationresult-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/examples/visionprescription-example.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/visionprescription-example.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/search-parameters.json` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/search-parameters.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhir_specification/utils.py` & `fhirstarter-0.13.9/fhirstarter/fhir_specification/utils.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/fhirstarter.py` & `fhirstarter-0.13.9/fhirstarter/fhirstarter.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     var_name_to_qp_name,
 )
 from .utils import (
     FormatParameters,
     create_route_args,
     format_response,
     make_operation_outcome,
+    parse_fhir_request,
     read_route_args,
     search_type_route_args,
     update_route_args,
 )
 
 # Suppress warnings from base fhir.resources class
 logging.getLogger("fhir.resources.core.fhirabstractmodel").setLevel(logging.WARNING + 1)
@@ -554,16 +555,18 @@
 
     There is an obscure requirement in the FHIR specification stipulating that for search POST
     requests, both query string parameters and parameters in the body are to be considered when
     calculating search results. This is difficult to achieve in FastAPI due to how the body stream
     is consumed when it parses the body to pass the values down to the handlers. Catching the
     request here allows for the body parameters to be merged with the query string parameters.
     """
+    interaction_info = parse_fhir_request(request)
+
     if (
-        request.url.path.endswith("/_search")
+        interaction_info.interaction_type == "search-type"
         and request.method == "POST"
         and request.headers.get("Content-Type") == "application/x-www-form-urlencoded"
     ):
         scope = request.scope
         scope["method"] = "GET"
         scope["path"] = scope["path"].removesuffix("/_search")
         scope["raw_path"] = scope["raw_path"].removesuffix(b"/_search")
@@ -636,15 +639,15 @@
 
 
 def _exception_response(
     request: Request, severity: str, code: str, details_text: str, status_code: int
 ) -> Response:
     """Create a JSONResponse with an OperationOutcome and an HTTP status code."""
     operation_outcome = make_operation_outcome(
-        severity=severity, code=code, details_text=details_text
+        severity=severity, code=code, details_text=details_text or "Exception"
     )
 
     return format_response(
         resource=operation_outcome,
         status_code=status_code,
         format_parameters=FormatParameters.from_request(request, raise_exception=False),
     )
```

### Comparing `fhirstarter-0.13.8/fhirstarter/functions.py` & `fhirstarter-0.13.9/fhirstarter/functions.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/interactions.py` & `fhirstarter-0.13.9/fhirstarter/interactions.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/providers.py` & `fhirstarter-0.13.9/fhirstarter/providers.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/scripts/example.py` & `fhirstarter-0.13.9/fhirstarter/scripts/example.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/search_parameters.py` & `fhirstarter-0.13.9/fhirstarter/search_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 
 def search_parameter_sort_key(
     name: str,
     search_parameter_metadata: dict[str, dict[str, str]],
     parameter_annotation: type | None = None,
 ) -> tuple[bool, bool, bool, bool, bool, str]:
     """
-    Return a sort key for a search paramter.
+    Return a sort key for a search parameter.
 
     This function allows for consistent sorting of search parameters throughout the package.
 
     Sort order is:
     1. Request and response annotations
     2. Parameters that do not start with underscore
     3. Parameters that are search or search result parameters (i.e. _format and _pretty go to the
```

### Comparing `fhirstarter-0.13.8/fhirstarter/tests/config.py` & `fhirstarter-0.13.9/fhirstarter/tests/config.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/tests/conftest.py` & `fhirstarter-0.13.9/fhirstarter/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/tests/test_capability_statement.py` & `fhirstarter-0.13.9/fhirstarter/tests/test_capability_statement.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/tests/test_dependencies.py` & `fhirstarter-0.13.9/fhirstarter/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/tests/test_errors.py` & `fhirstarter-0.13.9/fhirstarter/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/tests/test_interactions.py` & `fhirstarter-0.13.9/fhirstarter/tests/test_interactions.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.8/fhirstarter/utils.py` & `fhirstarter-0.13.9/fhirstarter/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Utility functions for creation of routes and responses."""
 
+import logging
 from collections.abc import Callable
 from dataclasses import dataclass
-from typing import Any, ClassVar
+from typing import Any, ClassVar, Literal
 
 from fastapi import Request
 from fastapi.responses import JSONResponse, Response
 from fhir.resources.bundle import Bundle
 from fhir.resources.operationoutcome import OperationOutcome
 from fhir.resources.resource import Resource
 
@@ -14,32 +15,40 @@
 from .fhir_specification.utils import is_resource_type
 from .interactions import ResourceType, SearchTypeInteraction, TypeInteraction
 
 
 @dataclass
 class InteractionInfo:
     resource_type: str | None
-    interaction_type: str | None
+    interaction_type: Literal[
+        "create", "read", "update", "search-type", "capabilities"
+    ] | None
+    resource_id: str | None
 
 
 def categorize_fhir_request(request: Request) -> InteractionInfo:
     """
     Return the resource type and interaction type for a request.
 
     Note: This function is currently oriented around specific use cases for this framework.
     Specifically, it will correctly categorize create, read, search-type, update, and capabilities
     interactions. Further enhancement is needed to support more cases.
     """
+    logging.warning(
+        "fhirstarter.utils.categorize_fhir_request has been deprecated and will be "
+        "removed in a future release"
+    )
+
     _, first_part, *rest = request.url.path.split("/")
 
     if request.method == "GET" and first_part == "metadata":
-        return InteractionInfo(resource_type=None, interaction_type="capabilities")  # type: ignore
+        return InteractionInfo(resource_type=None, interaction_type="capabilities", resource_id=None)  # type: ignore
 
     if not is_resource_type(first_part):
-        return InteractionInfo(resource_type=None, interaction_type=None)  # type: ignore
+        return InteractionInfo(resource_type=None, interaction_type=None, resource_id=None)  # type: ignore
 
     resource_type = first_part
     second_part = rest[0] if rest else None
     id_ = second_part if request.method != "POST" else None
 
     interaction_type = None
     match request.method, second_part == "_search", not id_:
@@ -52,15 +61,74 @@
         case "POST", True, True:
             interaction_type = "search-type"
         case "PUT", _, False:
             interaction_type = "update"
         case _:
             assert "Unexpected request format"
 
-    return InteractionInfo(resource_type, interaction_type)  # type: ignore
+    return InteractionInfo(resource_type, interaction_type, resource_id=id_)  # type: ignore
+
+
+def parse_fhir_request(request: Request) -> InteractionInfo:
+    """
+    Parse a FHIR request into its component parts, and determine an interaction type.
+
+    Note: This function is currently oriented around specific use cases for this framework.
+    Specifically, it will correctly categorize create, read, search-type, update, and capabilities
+    interactions. Further enhancement is needed to support more use cases.
+    """
+    no_info = InteractionInfo(  # type: ignore
+        resource_type=None, interaction_type=None, resource_id=None
+    )
+
+    split_path = request.url.path.split("/")
+    if not split_path:
+        return no_info
+
+    resource_id = None
+
+    if request.method == "GET":
+        if split_path[-1] == "metadata":
+            return InteractionInfo(  # type: ignore
+                resource_type=None, interaction_type="capabilities", resource_id=None
+            )
+        elif is_resource_type(split_path[-1]):
+            resource_type = split_path[-1]
+            interaction_type = "search-type"
+        elif len(split_path) >= 3:
+            resource_type, resource_id = split_path[-2:]
+            interaction_type = "read"
+        else:
+            return no_info
+    elif request.method == "POST":
+        if is_resource_type(split_path[-1]):
+            resource_type = split_path[-1]
+            interaction_type = "create"
+        elif split_path[-1] == "_search":
+            resource_type = split_path[-2]
+            interaction_type = "search-type"
+        else:
+            return no_info
+    elif request.method == "PUT":
+        if len(split_path) >= 3:
+            resource_type, resource_id = split_path[-2:]
+            interaction_type = "update"
+        else:
+            return no_info
+    else:
+        return no_info
+
+    if not is_resource_type(resource_type):
+        return no_info
+
+    return InteractionInfo(  # type: ignore
+        resource_type=resource_type,
+        interaction_type=interaction_type,
+        resource_id=resource_id,
+    )
 
 
 def make_operation_outcome(
     severity: str, code: str, details_text: str
 ) -> OperationOutcome:
     """Create a simple OperationOutcome given a severity, code, and details."""
     return OperationOutcome(
```

### Comparing `fhirstarter-0.13.8/pyproject.toml` & `fhirstarter-0.13.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fhirstarter"
-version = "0.13.8"
+version = "0.13.9"
 description = "An ASGI FHIR API framework built on top of FastAPI and FHIR Resources"
 authors = ["Christopher Sande <christopher.sande@canvasmedical.com>"]
 maintainers = ["Canvas Medical Engineering <engineering@canvasmedical.com>"]
 readme = "README.md"
 homepage = "https://github.com/canvas-medical/fhirstarter"
 repository = "https://github.com/canvas-medical/fhirstarter"
 keywords = ["fhir", "api", "resources", "framework", "fastapi", "healthcare", "hl7"]
@@ -36,22 +36,22 @@
 "fhir.resources" = "~6.4.0"
 lxml = "^4.9.2"
 python-multipart = "^0.0.6"
 uvloop = "^0.17.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
-funcy = "^1.18"
-httpx = "^0.23.3"
+funcy = ">=1.18,<3.0"
+httpx = ">=0.23.3,<0.25.0"
 isort = "^5.12.0"
 mypy = "^0.991"
 pytest = "^7.2.2"
 requests = "^2.28.2"
 types-requests = "^2.28.11.15"
-uvicorn = {version = "^0.21.0", extras = ["standard"]}
+uvicorn = {version = ">=0.21,<0.24", extras = ["standard"]}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 check_untyped_defs = true
```

### Comparing `fhirstarter-0.13.8/PKG-INFO` & `fhirstarter-0.13.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fhirstarter
-Version: 0.13.8
+Version: 0.13.9
 Summary: An ASGI FHIR API framework built on top of FastAPI and FHIR Resources
 Home-page: https://github.com/canvas-medical/fhirstarter
 Keywords: fhir,api,resources,framework,fastapi,healthcare,hl7
 Author: Christopher Sande
 Author-email: christopher.sande@canvasmedical.com
 Maintainer: Canvas Medical Engineering
 Maintainer-email: engineering@canvasmedical.com
@@ -17,15 +17,14 @@
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

#### html2text {}

```diff
@@ -1,32 +1,31 @@
-Metadata-Version: 2.1 Name: fhirstarter Version: 0.13.8 Summary: An ASGI FHIR
+Metadata-Version: 2.1 Name: fhirstarter Version: 0.13.9 Summary: An ASGI FHIR
 API framework built on top of FastAPI and FHIR Resources Home-page: https://
 github.com/canvas-medical/fhirstarter Keywords:
 fhir,api,resources,framework,fastapi,healthcare,hl7 Author: Christopher Sande
 Author-email: christopher.sande@canvasmedical.com Maintainer: Canvas Medical
 Engineering Maintainer-email: engineering@canvasmedical.com Requires-Python:
 >=3.11,<4.0 Classifier: Development Status :: 4 - Beta Classifier: Environment
 :: Web Environment Classifier: Framework :: AsyncIO Classifier: Framework ::
 FastAPI Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Healthcare Industry Classifier: Intended Audience :: Information
 Technology Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Topic :: Internet Classifier: Topic :: Internet ::
-WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers Classifier:
-Topic :: Software Development Classifier: Topic :: Software Development ::
-Libraries Classifier: Topic :: Software Development :: Libraries :: Application
-Frameworks Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Classifier: Typing :: Typed Requires-Dist: fastapi (>=0.94.1,<0.95.0)
-Requires-Dist: fhir.resources (>=6.4.0,<6.5.0) Requires-Dist: lxml
-(>=4.9.2,<5.0.0) Requires-Dist: python-multipart (>=0.0.6,<0.0.7) Requires-
-Dist: uvloop (>=0.17.0,<0.18.0) Project-URL: Repository, https://github.com/
-canvas-medical/fhirstarter Description-Content-Type: text/markdown #
-fhirstarter
+Programming Language :: Python :: 3.11 Classifier: Topic :: Internet
+Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/
+HTTP :: HTTP Servers Classifier: Topic :: Software Development Classifier:
+Topic :: Software Development :: Libraries Classifier: Topic :: Software
+Development :: Libraries :: Application Frameworks Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Classifier: Typing :: Typed
+Requires-Dist: fastapi (>=0.94.1,<0.95.0) Requires-Dist: fhir.resources
+(>=6.4.0,<6.5.0) Requires-Dist: lxml (>=4.9.2,<5.0.0) Requires-Dist: python-
+multipart (>=0.0.6,<0.0.7) Requires-Dist: uvloop (>=0.17.0,<0.18.0) Project-
+URL: Repository, https://github.com/canvas-medical/fhirstarter Description-
+Content-Type: text/markdown # fhirstarter
 [https://github.com/canvas-medical/fhirstarter/actions/workflows/test.yml/
 badge.svg] [https://img.shields.io/pypi/v/fhirstarter] [https://img.shields.io/
 pypi/pyversions/fhirstarter] [https://img.shields.io/pypi/l/fhirstarter]
 [https://img.shields.io/badge/code%20style-black-000000]
 An ASGI FHIR API framework built on top of [FastAPI](https://
 fastapi.tiangolo.com) and [FHIR Resources](https://pypi.org/project/
 fhir.resources/). The only version of FHIR that is currently supported is
```

