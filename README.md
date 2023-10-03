# Intake24 Survey Integration REDCap External Module

## Description
This module enables the REDCap survey instrument to trigger the intake24 survey and create a new user at intake24 based on the record ID as the user name.
The module will then save the generated unique intake24 URL in the REDCap record.

## External Module Configurable Variables
### Intake24.com Survey URL
The URL of your intake24 survey, e.g. https://intake24.com/surveys/LEHS_Survey
### Intake24 Secret Key for signing the JSON payload
This value should be the same as the 'JWT secret for user generation' configured at admin.intake24.com of your survey
### Intake24 Redirect URL stored in the JSON payload
When the intake24 survey is completed, the user will be directed to this URL.
### Intake24 User ID stored in the JSON payload
Which REDCap field will be used as the user ID in intake24, this should be a unique ID in your REDCap project, e.g. record_id
### The instrument/form name that will trigger the creation of the intake24 URL
Which REDCap instrument upon clicking 'Submit' will take the user to the intake24 survey.
### The field name that stores the generated intake24 URL with the JSON payload
The REDCap text field will store the generated intake24 URL, this could be used to send a reminder to complete the survey.
