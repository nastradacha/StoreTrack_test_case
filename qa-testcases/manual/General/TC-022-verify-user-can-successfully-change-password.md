---
title: "Verify user can successfully change password"
story_id: "AUTH-003"
priority: "P3"
suite: "General"
preconditions: |
  - User account exists in the system
  - Manager has reset cashier password to default reset password
  - User is logged in with reset password
  - User is redirected to change-password page
data: |
  Username 
  Password
steps: |
  1. Open the login page
  2. Enter username/Email
  3. Enter reset password
  4. Click Login
  5. System redirects user to change-password page
  6. Enter current password (reset password)
  7. Enter a new strong password
  8. Confirm new password
  9. Click Submit 
  10. System updates password successfully
  11. Log out
  12. Login again using the new password
expected: |
  - Password is successfully updated
  - User is redirected to dashboard or login
status: "Draft"
created: "2026-05-18T17:17:50.405Z"
created_by: "obidiahfavour"
---

# Verify user can successfully change password

## Story Reference
Story #AUTH-003

## Preconditions
- User account exists in the system
- Manager has reset cashier password to default reset password
- User is logged in with reset password
- User is redirected to change-password page


## Test Data
Username 
Password


## Test Steps
1. Open the login page
2. Enter username/Email
3. Enter reset password
4. Click Login
5. System redirects user to change-password page
6. Enter current password (reset password)
7. Enter a new strong password
8. Confirm new password
9. Click Submit 
10. System updates password successfully
11. Log out
12. Login again using the new password

## Expected Results
- Password is successfully updated
- User is redirected to dashboard or login

## Metadata
- **Priority**: P3
- **Suite**: General


