# Retry Logic

## Purpose

This document defines the retry strategy for outbound AI calls.

---

## Agent 1 Retry Strategy

### Attempt 1

- Trigger after the initial 5-minute timer.

### Attempt 2

- Retry after 1 minute if the first call is unanswered.

### Attempt 3

- Retry the next day.
- Preferred calling window:
  - Between 7:00 PM and 9:00 PM IST.

### Retry Exhausted

After three unsuccessful attempts:

- Mark the lead as Retry Exhausted.
- Export the lead for manual follow-up.

---

## Retry Cancellation

Cancel all remaining retries immediately if:

- Payment is completed.
- Lead requests no further calls.
- Lead is closed.

---

## Agent 2 Retry Strategy

The retry strategy follows the same process unless modified by business rules.