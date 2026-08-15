---
name: Phone Team
description: Optional communications team that staffs a voice front desk on Speko: a lead agent that sets up the phone line behind board approvals, answers and places disclosed calls, and files every call as a ticket with recording and transcript.
schema: agentcompanies/v1
slug: phone-team
category: comms
key: paperclipai/optional/comms/phone-team
manager: agents/front-desk-lead/AGENTS.md
includes:
  - projects/phone-operations/PROJECT.md
requiredSkills:
  - paperclipai/optional/comms/speko
defaultInstall: false
recommendedForCompanyTypes:
  - startup
  - agency
  - services
tags:
  - voice
  - phone
  - comms
---

# Phone Team

This optional team gives a company a phone. It staffs a voice front desk on Speko: one lead
agent stands up the phone line behind Paperclip board approvals, answers inbound calls,
places approved outbound calls with the AI disclosure intact, and files every call back into
Paperclip as a ticket with the recording and transcript attached.

## Contents

- `FrontDeskLead` - front desk lead responsible for line setup, inbound call triage, and
  approved outbound calling through the `paperclipai/optional/comms/speko` catalog skill.
- `phone-operations` project - rolling queue for call tickets, callback follow-ups, and
  phone-line maintenance work.
- `work-the-call-queue` routine - recurring front desk check-in to triage new call tickets
  and chase approved callbacks.
