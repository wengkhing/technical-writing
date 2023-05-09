# Problem statement

Currently, talents would only be able to login using email/password pair.

# Reference

Trello card

# Goals

- Able to login/sign up via Facebook button in app
- Email is verified if login via Facebook
- Reduce user friction on verifying email

# Non-goals

- Send transactional notification messages to talents, for example: daily job recommendations, notify talent that he/she has been confirmed for a role etc.
- Messenger integration
- Tie with facebook account (TBD)

# Proposed solution

using Cognito’s Identity Provider

## What are the high level architectural changes?

Diagrams can be very helpful here.

## What are the high level data model changes?

These should include any database schema changes, or any changes to structured fields, e.g. an existing JSON column.

## What are the main changes to the UI?

- Having a Login with Facebook button in login page
- Having a Sign up with Facebook button in registration page

# Risks / Blockers

| Risk / Blocker | Mitigation Plan | Status | Stakeholder |
|--|--|--|--|
| Facebook review might take some time to process as they need to review us | Apply review earlier even before any implementation started | | |
| Talent who already signed up with their email might sign in with fb | Prompt warning | | |

# Implementation Details

| Tasks | Details | Effort (Story Points) |
|--|--|--|
| Setup facebook developer account | Need a fb dev account for further integration | 1 |
