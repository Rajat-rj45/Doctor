# MarizFirst Booking Rules

## Core Booking Model

MarizFirst uses a hybrid booking model.

Patients can select a preferred visible slot, but this is only an appointment request until confirmed by admin or partner.

## Initial Appointment Status

Every new appointment must start with:

PENDING_CONFIRMATION

## Allowed Statuses

- PENDING_CONFIRMATION
- CONFIRMED
- RESCHEDULED
- CANCELLED
- COMPLETED
- NO_SHOW
- LOST

## Patient-Facing Rule

Never show "Appointment Confirmed" immediately after form submission.

Show:

"Your appointment request has been received. MarizFirst or the healthcare provider will confirm shortly."

## Slot Rule

Only AVAILABLE slots with remaining capacity can be selected.

Slot must be validated twice:

1. When displayed
2. Again during appointment creation

## Admin/Partner Rule

Only admin or authorized partner can confirm, reschedule, cancel, complete, mark no-show, or mark lost.

## Audit Rule

Every sensitive appointment status change must create an audit log.

This follows the appointment state machine from the App Flow Document: every patient-facing appointment starts as Pending Confirmation, and only admin or authorized partner can change it to Confirmed.
