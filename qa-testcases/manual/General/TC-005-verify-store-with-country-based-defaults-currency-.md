---
title: "verify Store with country-based defaults (currency, symbol, timezone). in database"
story_id: "US-003"
priority: "P3"
suite: "registration"
component: "registration"
preconditions: "-  URL; https://inventory-app-qa.onrender.com/"
data: |
  SELECT * FROM store 
   order by id desc
steps: |
  1. click on this URL; https://inventory-app-qa.onrender.com/
  2. login with your password and username
  3. check database for store
expected: "-  Store with country-based defaults (currency, symbol, timezone). should be shown in database"
env: "QA"
status: "Draft"
created: "2026-01-16T22:49:04.187Z"
created_by: "yuslove123l"
---

# verify Store with country-based defaults (currency, symbol, timezone). in database

## Story Reference
Story #US-003

## Preconditions
-  URL; https://inventory-app-qa.onrender.com/


## Test Data
SELECT * FROM store 
 order by id desc


## Test Steps
1. click on this URL; https://inventory-app-qa.onrender.com/
2. login with your password and username
3. check database for store

## Expected Results
-  Store with country-based defaults (currency, symbol, timezone). should be shown in database

## Metadata
- **Priority**: P3
- **Suite**: registration
- **Component**: registration
- **Environment**: QA
