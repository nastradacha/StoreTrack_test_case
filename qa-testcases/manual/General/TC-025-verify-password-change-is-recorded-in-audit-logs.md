---
title: "Force password change after manager reset Priority"
story_id: "AUTH-003"
priority: "P3"
suite: "General"
preconditions: |
  - A cashier account exists and can normally log in
  - A manager resets the cashier password to the configured default reset password
  - The forced-change flag is set after the reset
  - You have the reset password and a new valid password ready
data: |
  Username: <cashier_username>
  Reset password: <configured default reset password>
  New password: <new valid password>
steps: |
  1. A cashier account exists and can normally log in
  2. A manager resets the cashier password to the configured default reset password
  3. The forced-change flag is set after the reset
  4. You have the reset password and a new valid password ready
expected: |
  - User lands on /change-password and cannot reach Dashboard or Products until the change is done
  - The new password is accepted and Dashboard loads
  - The original reset password no longer works at login
  - The new password works on the next login
status: "Draft"
created: "2026-05-18T17:38:28.576Z"
created_by: "obidiahfavour"
updated_by: "obidiahfavour"
updated: "2026-06-01T22:03:20.878Z"
---

# Force password change after manager reset Priority

## Story Reference
Story #AUTH-003

## Preconditions
- A cashier account exists and can normally log in
- A manager resets the cashier password to the configured default reset password
- The forced-change flag is set after the reset
- You have the reset password and a new valid password ready

## Test Data
Username: <cashier_username>
Reset password: <configured default reset password>
New password: <new valid password>

## Test Steps
1. A cashier account exists and can normally log in
2. A manager resets the cashier password to the configured default reset password
3. The forced-change flag is set after the reset
4. You have the reset password and a new valid password ready

## Expected Results
- User lands on /change-password and cannot reach Dashboard or Products until the change is done
- The new password is accepted and Dashboard loads
- The original reset password no longer works at login
- The new password works on the next login

## Metadata
- **Priority**: P3
- **Suite**: General
