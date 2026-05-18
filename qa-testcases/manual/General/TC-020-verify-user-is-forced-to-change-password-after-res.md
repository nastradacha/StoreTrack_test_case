---
title: "Verify user is forced to change password after reset login"
story_id: "AUTH-003"
priority: "P3"
suite: "General"
preconditions: |
  - User password has been reset by manager
  - User is logged out
data: |
  Username: valid user
  Password: reset/default password
steps: |
  1. Go to login page
  2. Login with reset password
  3. Try to access dashboard
expected: |
  - User is redirected to change-password
  - User cannot access any app page until password is changed
status: "Draft"
created: "2026-05-18T16:43:46.160Z"
created_by: "obidiahfavour"
---

# Verify user is forced to change password after reset login

## Story Reference
Story #AUTH-003

## Preconditions
- User password has been reset by manager
- User is logged out


## Test Data
Username: valid user
Password: reset/default password


## Test Steps
1. Go to login page
2. Login with reset password
3. Try to access dashboard

## Expected Results
- User is redirected to change-password
- User cannot access any app page until password is changed

## Metadata
- **Priority**: P3
- **Suite**: General


