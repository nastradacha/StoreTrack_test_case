---
title: "TC-001- Verify User login activity is recorded"
story_id: "US-AUTH-002"
priority: "P3"
suite: "General"
component: "Login"
preconditions: "- account already created, tester has access to DB"
data: "test username: mikeDtester , test password:  I dont have it, will ask developer when app is ready"
verification_sql: "SELECT id, name, last_activity_at FROM store"
steps: |
  1. Login to  StoreTrack
  2. record time at login
  3. Verify last_activity_at in DB matches time recorded in step 2
expected: "- Time recorded in step 2 matches last_activity_at in DB"
env: "QA"
status: "Draft"
created: "2026-05-06T15:34:25.149Z"
created_by: "nastradacha"
updated_by: "nastradacha"
updated: "2026-05-06T15:37:55.637Z"
---

# TC-001- Verify User login activity is recorded

## Story Reference
Story #US-AUTH-002

## Preconditions
- account already created, tester has access to DB

## Test Data
test username: mikeDtester , test password:  I dont have it, will ask developer when app is ready

## Test Steps
1. Login to  StoreTrack
2. record time at login
3. Verify last_activity_at in DB matches time recorded in step 2

## Expected Results
- Time recorded in step 2 matches last_activity_at in DB

## Metadata
- **Priority**: P3
- **Suite**: General
- **Component**: Login
- **Environment**: QA
