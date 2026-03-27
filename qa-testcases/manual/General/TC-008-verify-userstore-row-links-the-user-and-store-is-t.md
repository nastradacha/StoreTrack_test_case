---
title: "verify  UserStore row links the user and store. is the database"
story_id: "US-003"
priority: "P2"
suite: "registration"
component: "registration"
preconditions: "- URL; https://inventory-app-qa.onrender.com/"
data: |
  SELECT * FROM user_store
  order by id desc
steps: |
  1. click on this  URL; https://inventory-app-qa.onrender.com/
  2. login with your verify password
  3. check database for 
expected: "- userstore link should be shown in database"
env: "QA"
status: "Draft"
created: "2026-01-16T23:28:02.772Z"
created_by: "yuslove123l"
---

# verify  UserStore row links the user and store. is the database

## Story Reference
Story #US-003

## Preconditions
- URL; https://inventory-app-qa.onrender.com/


## Test Data
SELECT * FROM user_store
order by id desc


## Test Steps
1. click on this  URL; https://inventory-app-qa.onrender.com/
2. login with your verify password
3. check database for 

## Expected Results
- userstore link should be shown in database

## Metadata
- **Priority**: P2
- **Suite**: registration
- **Component**: registration
- **Environment**: QA
