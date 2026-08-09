# Public Architecture Overview

This is a product-level architecture description and intentionally omits source-level implementation details.

## Product workflow

GoPilot organizes the driver workflow around a Saved Trip.

A Saved Trip can connect:
- permit records
- route review
- load/trip details
- mileage
- receipts / expenses
- invoice records
- documents / notes
- workflow completion state

## Permit processing

The Permit Reader uses OCR-assisted document review. OCR output is treated as extracted text that requires driver verification.

Original OCR text is preserved separately from cleaned route-oriented text so the driver can compare the result.

## Local record model

GoPilot is designed around local trip organization with explicit export/share actions when the user chooses to use them.

## Public safety boundary

This repository deliberately excludes:
- storage schema details
- entitlement implementation
- API/service configuration
- signing and release internals
- source code
