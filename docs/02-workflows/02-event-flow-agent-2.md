# Event Flow – Agent 2

## Objective

Agent 2 contacts applicants who have completed payment but have not booked an interview.

## Workflow

### Step 1

Razorpay sends the `payment.captured` webhook.

↓

2Care updates:

payment_status = completed

↓

Starts a 30-minute grace period.

---

### Step 2

If the applicant books an interview:

Calendly sends an `invitee.created` webhook.

↓

2Care updates:

interview_scheduled = true

↓

Pending Agent 2 job is cancelled.

---

### Step 3

If 30 minutes pass without an interview booking:

↓

2Care triggers the AI API.

↓

Agent 2 places an outbound call.

---

### Step 4

Agent 2 helps the applicant complete interview booking.

The AI:

- Explains the interview process.
- Answers interview questions.
- Encourages booking.

---

### Step 5

After the call:

AI sends the call result back to 2Care.

↓

Dashboard is updated.