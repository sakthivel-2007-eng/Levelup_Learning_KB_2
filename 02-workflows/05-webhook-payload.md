# Webhook Payload

## Purpose

This document defines the minimum fields required from the Tally webhook.

---

## Required Fields

### phone

Used for:

- Outbound AI calls.

---

### program

Used for:

- Selecting the correct course knowledge base.

---

### product

Used for:

- Selecting the appropriate payment link.
- Choosing the correct email template.

---

### user_type

Possible values:

- Student
- Professional
- Founder

Used for:

- Persona-based conversation.

---

### why_join

Used for:

- Objection handling.
- Personalizing the conversation.

---

### email

Used for:

- Payment link delivery.
- Follow-up communication.

---

### submission_id

Used for:

- Deduplication.
- Preventing duplicate outbound jobs.

---

## Validation

The AI workflow should verify that all required fields are present before processing the request.