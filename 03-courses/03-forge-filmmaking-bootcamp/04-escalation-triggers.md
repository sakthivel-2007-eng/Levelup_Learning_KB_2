# Escalation Triggers

The AI agent should stop attempting to answer independently and transfer the conversation to a human admissions or sales representative whenever any of the following situations occur.

---

## 1. Current Cohort Information

Escalate if the caller asks for:

- Exact current cohort dates
- City or venue
- Mentor names
- Fee slab
- Grant slab
- Payment deadline
- Seat availability

**Reason:** The agent does not have access to live cohort data.

---

## 2. Pricing Negotiation

Escalate if the caller requests:

- Special discounts
- Custom scholarships
- Pricing exceptions
- Negotiated offers beyond documented pricing

---

## 3. Refunds and Legal Policies

Escalate if the caller asks about:

- Refund policy
- Cancellation policy
- Transfer policy
- Legal terms
- Contract wording

---

## 4. Payment Issues

Escalate if the caller reports:

- Payment failure
- Receipt issue
- Confirmation issue
- Already completed payment

---

## 5. Custom Payment Plans

Escalate if the caller requests:

- Payment extensions
- Non-standard installment plans

---

## 6. Parent, Sponsor, or Family Discussion

Escalate if:

- A parent
- A spouse
- A sponsor

wants to speak directly with someone from the admissions team.

---

## 7. Business or Institutional Payments

Escalate if the caller asks about:

- GST invoices
- Company sponsorship
- Institutional payment
- Bulk enrollment

---

## 8. Medical or Accessibility Requirements

Escalate if the caller has questions about:

- Medical requirements
- Accessibility needs
- Dietary requirements
- Safety concerns
- Accommodation requests

These require human confirmation.

---

## 9. Minor Applicants

Escalate if:

- The applicant is a minor
- Guardian approval handling is required

---

## 10. Travel and Logistics

Escalate if the caller asks about:

- Travel booking support
- Visa support
- Airport transfers
- Special logistics not covered in the knowledge base

---

## 11. Complaints or Trust Concerns

Escalate if the caller raises:

- Serious complaints
- Trust issues
- Negative previous experiences
- Reputational concerns

and requests reassurance from the team.

---

## 12. Emotional or Financial Distress

Escalate if the caller sounds:

- Emotionally distressed
- Financially overwhelmed
- Highly pressured

These situations require a more sensitive human conversation.

---

## 13. Previous Special Cases

Escalate if the caller says they:

- Already attended an interview
- Already received a grant
- Were previously selected
- Have a previous special case

---

## 14. Immediate Human Assistance

Escalate if the caller requests:

- Brochure
- Payment link
- Callback
- WhatsApp follow-up
- Immediate consultation with a human

---

## 15. Questions Requiring Human Judgment

Escalate whenever the caller asks anything that requires:

- Human discretion
- Personal judgment
- Cohort-specific interpretation
- Information unavailable in the knowledge base

---

# Agent Rule

When the requested information depends on live, cohort-specific, commercial, or sensitive information, **do not guess**.

Always transfer the conversation to the admissions team for accurate assistance.