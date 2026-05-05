---
title: "TC-AUTH-001- Account creation - validation "
story_id: "US-AUTH-001"
priority: "P2"
suite: "General"
component: "Login"
data: |
  data: |
  SELECT s.id, s.name, s.country_code, s.currency_code, s.currency_symbol, s.timezone, s.org_id
  FROM store s
  WHERE s.name = 'QA-Store-<date>';
  SELECT id, username, role, store_id, org_id
  FROM "user"
  WHERE username = lower('<email>');
  
  
  SELECT * FROM user_store WHERE user_id = <user_id> AND store_id = <store_id>;
  SELECT * FROM store_settings WHERE store_id = <store_id>;
  SELECT * FROM org_subscription WHERE org_id = <org_id>;
steps: |
  1. Open /register
  2. Enter shop name QA-Store-<date>
  3. Select Ghana or Nigeria
  4.  Enter email and matching password/confirm password.
  5. Submit.
expected: |
  - UI - User lands on Dashboard. No error toast. Active store is the newly created store.
  - DB - One row exists in store; one row exists in "user" with role admin; one user_store row links user and store; one store_settings row exists; one organization row exists; one org_subscription row exists with status='TRIALING'.
env: "QA"
status: "Draft"
created: "2026-04-29T20:55:49.666Z"
created_by: "nastradacha"
---

# TC-AUTH-001- Account creation - validation 

## Story Reference
Story #US-AUTH-001



## Test Data
data: |
SELECT s.id, s.name, s.country_code, s.currency_code, s.currency_symbol, s.timezone, s.org_id
FROM store s
WHERE s.name = 'QA-Store-<date>';
SELECT id, username, role, store_id, org_id
FROM "user"
WHERE username = lower('<email>');


SELECT * FROM user_store WHERE user_id = <user_id> AND store_id = <store_id>;
SELECT * FROM store_settings WHERE store_id = <store_id>;
SELECT * FROM org_subscription WHERE org_id = <org_id>;


## Test Steps
1. Open /register
2. Enter shop name QA-Store-<date>
3. Select Ghana or Nigeria
4.  Enter email and matching password/confirm password.
5. Submit.

## Expected Results
- UI - User lands on Dashboard. No error toast. Active store is the newly created store.
- DB - One row exists in store; one row exists in "user" with role admin; one user_store row links user and store; one store_settings row exists; one organization row exists; one org_subscription row exists with status='TRIALING'.

## Metadata
- **Priority**: P2
- **Suite**: General
- **Component**: Login
- **Environment**: QA
