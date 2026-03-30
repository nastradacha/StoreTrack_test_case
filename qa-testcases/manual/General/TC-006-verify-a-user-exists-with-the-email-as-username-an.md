---
title: "verify A User exists with the email as username and role manager. in database"
story_id: "US-003"
priority: "P3"
suite: "registration"
component: "registration"
preconditions: "-  URL; https://inventory-app-qa.onrender.com/"
data: "SELECT * FROM public.user"
steps: |
  1. click on this URL; https://inventory-app-qa.onrender.com/
  2. login your verify password and username
  3. check database for username role of manager
expected: "- username and role manager should be shown"
env: "QA"
status: "Draft"
created: "2026-01-16T23:04:52.366Z"
created_by: "yuslove123l"
---

# verify A User exists with the email as username and role manager. in database

## Story Reference
Story #US-003

## Preconditions
-  URL; https://inventory-app-qa.onrender.com/


## Test Data
SELECT * FROM public.user


## Test Steps
1. click on this URL; https://inventory-app-qa.onrender.com/
2. login your verify password and username
3. check database for username role of manager

## Expected Results
- username and role manager should be shown

## Metadata
- **Priority**: P3
- **Suite**: registration
- **Component**: registration
- **Environment**: QA
