# Flight Booking Test Scenarios

This document contains the high-level test scenarios created for the Flight Booking demo application.

**Application Under Test:** https://travel.agileway.net/login

---

# Flight Booking

## Valid Scenarios

- Validate booking a Return trip with valid travel details.
- Validate booking a One Way trip with valid travel details.
- Validate booking with the same Departure and Return date (if supported).
- Validate booking a One Way trip with today's date.
- Validate changing the trip type from Return to One Way before booking.
- Validate changing the trip type from One Way to Return before booking.

## Invalid Scenarios

- Validate booking without selecting an Origin.
- Validate booking without selecting a Destination.
- Validate booking with identical Origin and Destination locations.
- Validate a Return trip booking without a Return date.
- Validate booking with a Return date earlier than the Departure date.
- Validate booking with a Departure date in the past.
- Validate booking with all mandatory fields left empty.
- Validate booking with an invalid calendar date (if applicable).

---

# Passenger Details

## Invalid Scenarios

- Validate leaving fields empty in passenger details.

---

# Payment

## Valid Scenarios

- Validate payment using a valid Visa credit card.
- Validate payment using a valid Master credit card.
- Validate changing the card type before submitting the payment.

## Invalid Scenarios

- Validate payment without selecting a card type (if applicable).
- Validate payment without entering the card holder's name.
- Validate payment without entering the card number.
- Validate payment with all mandatory fields left empty.
- Validate payment with an invalid credit card number.
- Validate payment with a credit card number shorter than the minimum allowed length.
- Validate payment with a credit card number longer than the maximum allowed length.
- Validate payment with alphabetic characters in the credit card number.
- Validate payment with special characters in the credit card number.
- Validate payment with an expired credit card.
- Validate payment with an invalid card holder name.
- Validate payment with an expiry month earlier than the current month in the current year.
- Validate payment with an invalid card number for the selected card type.
- Validate payment when the payment gateway declines the transaction.
- Validate payment when the payment gateway is unavailable.
- Validate application behavior when the payment request times out.
