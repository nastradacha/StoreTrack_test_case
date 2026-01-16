---
title: "verify StoreSettings row exists for that store. in the database"
story_id: "US-003"
priority: "P3"
suite: "registration"
component: "registration"
preconditions: "-  URL; https://inventory-app-qa.onrender.com/"
data: |
  SELECT * FROM store_settings
  order by id desc
steps: |
  1. click on this  URL; https://inventory-app-qa.onrender.com/
  2. click login and login with ur verify passwod
  3. go to database check for storesetting 
expected: "-  StoreSettings row exists for that store should be shown"
env: "QA"
status: "Draft"
created: "2026-01-16T23:19:57.674Z"
created_by: "yuslove123l"
---

# verify StoreSettings row exists for that store. in the database

## Story Reference
Story #US-003

## Preconditions
-  URL; https://inventory-app-qa.onrender.com/


## Test Data
SELECT * FROM store_settings
order by id desc


## Test Steps
1. click on this  URL; https://inventory-app-qa.onrender.com/
2. click login and login with ur verify passwod
3. go to database check for storesetting 

## Expected Results
-  StoreSettings row exists for that store should be shown

## Metadata
- **Priority**: P3
- **Suite**: registration
- **Component**: registration
- **Environment**: QA
