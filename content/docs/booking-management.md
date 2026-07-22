---
title: "Booking Management"
weight: 5
---

**URL:** https://app.fleetros.com/bookings

## Viewing Bookings

Click Bookings in the sidebar to see all customer reservations. The table lists the Booking ID, Customer, Vehicle, Dates, Pickup location, Amount (with balance due), and Status.

Use the filter tabs: All Bookings, By ID, By Customer, By Date Range, By Status, By Payment, or Advanced Search. Set Page Size and Sort By/Order, then click Search, or click Reset to clear filters.

## Creating a New Booking

**URL:** https://app.fleetros.com/bookings/new

1. Click the + New Booking button to open the 4-step wizard.
2. Under Booking Window, set the Start and End Date using the date picker (with Quick Select options like Today, Start/End of Month or Year, or Open Calendar). Add an optional Guest Name, and provide a Guest Email and/or Phone (at least one is required to check discount eligibility).
3. Under Reservation Details, check which vehicles, add-ons, and discounts are available for your dates. Search and select up to 5 vehicles, optionally apply a Discount, set the Status (e.g. Pending, Confirmed, Active), and choose any Optional Offerings (you can adjust quantities afterward).
4. Under Logistic Coverage, enter the Pickup and Drop-off Locations (both required, previously used locations are suggested as you type). You can also add an optional Insurance Policy description and select a Liability Reduction Option if any are configured.
5. Under Pricing Overview, click Preview Pricing to calculate the total cost before finalising the booking. Review the breakdown, then click Create Booking to confirm.

## Managing an Existing Booking

Click View on any booking row to open its detail page. The page has four tabs:

### Details Tab

Shows Booking Images by category (e.g. Rental Agreement, Delivery Inspection, Delivery/Retrieval Handover, Fuel Receipt, Toll Receipt), a Reservation Summary (vehicle, package, discount, status, dates, pickup/drop-off locations), and Financial Details (rate breakdown, fees, tax, deposit, grand total, and amounts due at booking, pickup, and any remaining balance).

### Hand-over Tab

Shows the Car Hand-over status, with Mark as Delivered and Mark as Retrieved actions. Each stage records a timestamp and an Inspection Checklist covering exterior and interior condition, tyres and wheels, fuel level, odometer, and lights and signals. Each item is marked OK or Issue, with supporting photos.

### Payments Tab

Shows the Payment Summary (Total, Paid, Balance) and Payment History, with actions to Record Payment, Write Off, or Close Settlement. A Simple View toggle hides non-cash entries such as write-offs and manual adjustments.

### History Tab

Shows a complete audit trail of status changes and payment adjustments, including who made each change and when.

At the top of the booking detail page you can also click Record Payment, Print Receipt, Modify Booking, or Delete.

> **Tip:** Use the Modify Booking feature to change dates, vehicles, or offerings on an existing reservation. The system will show a cost preview before you confirm any changes.

## Pricing Calculation Examples

Every booking total follows the same structure:

1. The **vehicle rate** (multiplied by the number of days or hours) is added to any selected offerings to form the **Subtotal**.
2. Any **discounts** are subtracted from the Subtotal.
3. **Tax (10%)** is calculated on the discounted amount, and a **Service Fee (5%)** is calculated on the original Subtotal.
4. The sum of these gives the **Grand Total**. A refundable **Deposit** is shown as the amount **Due at Booking**, with the remainder **Due at Pickup**.

---

### Example A — Daily Rate Only

> A vehicle is set with a Daily rate of RM 120.00. The customer books it for 2 days and adds a GPS offering at RM 50.00.

| Line Item | Calculation | Amount |
|---|---|---|
| Vehicle rental | 2 days × RM 120.00 | RM 240.00 |
| GPS offering | — | RM 50.00 |
| **Subtotal** | | **RM 290.00** |
| Tax (10%) | 10% × RM 290.00 | RM 29.00 |
| Service Fee (5%) | 5% × RM 290.00 | RM 14.50 |
| **Grand Total** | | **RM 333.50** |
| Due at Booking (deposit) | | RM 66.70 |
| Due at Pickup (balance) | | RM 266.80 |

---

### Example B — Daily Rate with Discounts

> A vehicle is set with a Daily rate of RM 180.00 and booked for 3 days. Two discounts are applied: SAVE10 (10% off) and SAVE20 (fixed RM 20.00 off). Discounts are subtracted before Tax is calculated, while the Service Fee is based on the original Subtotal.

| Line Item | Calculation | Amount |
|---|---|---|
| Vehicle rental | 3 days × RM 180.00 | RM 540.00 |
| **Subtotal** | | **RM 540.00** |
| Discount — SAVE10 (10%) | 10% × RM 540.00 | −RM 54.00 |
| Discount — SAVE20 (fixed) | — | −RM 20.00 |
| **Discounted amount** | | **RM 466.00** |
| Tax (10%) | 10% × RM 466.00 | RM 46.60 |
| Service Fee (5%) | 5% × RM 540.00 | RM 27.00 |
| **Grand Total** | | **RM 539.60** |

---

### Example C — Daily + Hourly Rate Combined

> A vehicle is set with a Daily rate of RM 250.00 and an Hourly rate of RM 10.15. The customer books it for 30 hours. When both rates exist, the system charges full days at the daily rate and bills only the leftover hours at the hourly rate.

| Line Item | Calculation | Amount |
|---|---|---|
| Vehicle rental (full day) | 1 day × RM 250.00 | RM 250.00 |
| Vehicle rental (extra hours) | 6 hours × RM 10.15 | RM 60.90 |
| **Subtotal** | | **RM 310.90** |
| Tax (10%) | 10% × RM 310.90 | RM 31.09 |
| Service Fee (5%) | 5% × RM 310.90 | RM 15.55 |
| **Grand Total** | | **RM 357.54** |

---

### How Single Rate Types Are Handled

| Scenario | Behaviour |
|---|---|
| **Daily rate only** | Any partial day is rounded up to a full day. For example, a 9-hour booking on a vehicle priced at RM 120.00/day is billed as 1 full day (RM 120.00), because there is no hourly rate. |
| **Hourly rate only** | The booking is billed purely by the number of hours. If the duration is shorter than the vehicle's Minimum Rental Hours setting, the minimum number of hours is charged. |