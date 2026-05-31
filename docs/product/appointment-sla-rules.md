# Appointment SLA Rules

## Purpose

Pending appointments must be handled quickly because trust depends on clear confirmation.

## Default SLA

Pending appointments should be acted on within 15-30 minutes during working hours.

## SLA States

1. New Pending
   - Appointment just submitted
   - Status: PENDING_CONFIRMATION

2. Approaching SLA
   - Pending for more than 15 minutes
   - Show warning in admin dashboard

3. SLA Breached
   - Pending for more than 30 minutes
   - Admin must manually follow up with partner/patient

## Admin Action Rules

Admin can:

- Confirm appointment
- Reschedule appointment
- Cancel appointment
- Mark lost
- Add internal note
- Retry failed notification
- Contact partner manually

## Partner Action Rules

Partner can:

- Accept appointment
- Reject appointment
- Request reschedule
- Mark completed
- Mark no-show after appointment date

## Audit Rules

Every SLA-sensitive action must create audit log:

- Status change
- Admin note
- Partner response
- Notification retry
- Manual follow-up note

## Patient-Facing Copy

Use:

"Your appointment request has been received. MarizFirst or the healthcare provider will confirm shortly."

Do not use:

"Your appointment is confirmed."

unless status is CONFIRMED.

PRD defines the operational SLA: pending appointments should be acted on within 15-30 minutes during working hours, and admin dashboard must highlight SLA breach risk.
