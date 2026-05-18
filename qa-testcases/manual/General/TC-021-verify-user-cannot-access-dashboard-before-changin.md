---
title: "Verify user cannot access dashboard before changing password"
story_id: "AUTH-003"
priority: "P3"
suite: "General"
preconditions: |
  - User account already exists
  - Manager has reset user password to reset password
  - User is logged out
data: |
  Username: valid user
  Password: reset password
steps: |
  1. Login with reset password
  2. Try opening  the dashboard
expected: |
  - Access is blocked
  - User is always redirected to change-password
status: "Draft"
created: "2026-05-18T16:58:15.177Z"
created_by: "obidiahfavour"
---

# Verify user cannot access dashboard before changing password

## Story Reference
Story #AUTH-003

## Preconditions
- User account already exists
- Manager has reset user password to reset password
- User is logged out


## Test Data
Username: valid user
Password: reset password


## Test Steps
1. Login with reset password
2. Try opening  the dashboard

## Expected Results
- Access is blocked
- User is always redirected to change-password

## Metadata
- **Priority**: P3
- **Suite**: General


