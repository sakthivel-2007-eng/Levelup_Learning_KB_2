# Trigger Timing

## Overview

This document defines when each AI agent should be triggered after specific user actions.

---

## Agent 1 Trigger

### Event

Application form submitted.

### Condition

Payment has not been completed.

### Trigger Delay

5 minutes after successful form submission.

### Cancellation Condition

If payment is completed before the 5-minute timer expires:

- Cancel Agent 1 trigger.
- No outbound call is placed.

---

## Agent 2 Trigger

### Event

Application fee payment completed.

### Condition

Interview has not been booked.

### Trigger Delay

30 minutes after successful payment.

### Cancellation Condition

If the interview is booked before the timer expires:

- Cancel Agent 2 trigger.
- No outbound call is placed.

---

## Trigger Priority

1. Agent 1
2. Agent 2

Only one active trigger should exist for the same applicant at a time.