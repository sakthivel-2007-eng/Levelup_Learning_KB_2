# Event Flow – Agent 1

## Objective

Agent 1 contacts applicants who submitted the application form but have not completed the application fee payment.

## Workflow

### Step 1

User submits the Tally application form.

↓

Tally sends a `form.submission.created` webhook.

---

### Step 2

2Care receives the webhook.

- Creates the lead.
- Stores applicant information.
- Starts a 5-minute countdown.

---

### Step 3

If payment is completed within 5 minutes:

Razorpay sends a `payment.captured` webhook.

↓

2Care updates:

payment_status = completed

↓

The countdown is cancelled.

---

### Step 4

If the countdown finishes and payment is still pending:

↓

2Care triggers the AI API.

↓

Agent 1 places an outbound call.

---

### Step 5

Agent 1 speaks with the applicant.

The AI:

- Explains the payment step.
- Answers questions.
- Encourages payment.

---

### Step 6

After the call:

AI sends the call outcome to 2Care.

Possible outcomes include:

- Payment link sent
- Escalation requested
- Retry required

---

### Step 7

2Care updates the Tally CRM.

---

### Step 8

Dashboard is updated.