---
title: "Verify password change succeeds with valid password"
story_id: "AUTH-003"
priority: "P3"
suite: "General"
preconditions: |
  - Manager has reset password
  - User is on change-password page
data: |
  Current password
  New password
steps: |
  1. Enter current password
  2. Enter valid new password
  3. Confirm new password
  4. Click Submit
expected: |
  - Password is successfully updated
  - Success message displayed
  - User is allowed to proceed to app
status: "Draft"
created: "2026-05-18T17:33:27.509Z"
created_by: "obidiahfavour"
---

# Verify password change succeeds with valid password

## Story Reference
Story #AUTH-003

## Preconditions
- Manager has reset password
- User is on change-password page


## Test Data
Current password
New password


## Test Steps
1. Enter current password
2. Enter valid new password
3. Confirm new password
4. Click Submit

## Expected Results
- Password is successfully updated
- Success message displayed
- User is allowed to proceed to app

## Metadata
- **Priority**: P3
- **Suite**: General


