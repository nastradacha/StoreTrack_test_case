---
title: "Verify old reset password no longer works"
story_id: "AUTH-003"
priority: "P3"
suite: "General"
preconditions: "- User has successfully changed password"
data: |
  Username: cashier user
  Password: old reset password
steps: |
  1. Open login page
  2. Enter username
  3. Enter old password
  4. Login
expected: |
  - Login fails
  - Error message shown (Invalid credentials)
  - User not found
status: "Draft"
created: "2026-05-18T17:36:24.692Z"
created_by: "obidiahfavour"
---

# Verify old reset password no longer works

## Story Reference
Story #AUTH-003

## Preconditions
- User has successfully changed password


## Test Data
Username: cashier user
Password: old reset password


## Test Steps
1. Open login page
2. Enter username
3. Enter old password
4. Login

## Expected Results
- Login fails
- Error message shown (Invalid credentials)
- User not found

## Metadata
- **Priority**: P3
- **Suite**: General


