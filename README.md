# Electricity Bill Calculator (PHP)

A responsive web application that calculates electricity bills based on a tiered/slab-based tariff system, built using PHP and Bootstrap.

## Features

- User inputs electricity units consumed
- Bill calculated automatically using a 4-tier slab system
- Server-side input validation (rejects negative/non-numeric input)
- Client-side validation for immediate feedback
- Clean, responsive UI using Bootstrap 5
- Clear breakdown of applicable tariff slabs displayed to the user

## Tariff Structure

| Units | Rate |
|---|---|
| First 50 units | â‚¹3.50/unit |
| Next 100 units (51â€“150) | â‚¹4.00/unit |
| Next 100 units (151â€“250) | â‚¹5.20/unit |
| Above 250 units | â‚¹6.50/unit |

## Technologies Used

- PHP 8.2
- HTML5 & CSS3
- Bootstrap 5
- Apache (via XAMPP)

## Installation & Setup

1. Install [XAMPP](https://www.apachefriends.org/) with PHP 8.2+
2. Clone this repository into your XAMPP `htdocs` folder:
```bash
   cd C:\xampp\htdocs
   git clone <repository-url> electricity-bill-php
```
3. Start Apache via the XAMPP Control Panel
4. Open your browser and go to: 
## How to Use

1. Enter the number of electricity units consumed
2. Click "Calculate Bill"
3. View the calculated bill and applicable tariff breakdown

## Testing

Verified against the following boundary values:

| Units | Expected Bill |
|---|---|
| 0 | â‚¹0.00 |
| 1 | â‚¹3.50 |
| 50 | â‚¹175.00 |
| 51 | â‚¹179.00 |
| 150 | â‚¹575.00 |
| 151 | â‚¹580.20 |
| 250 | â‚¹1,095.00 |
| 251 | â‚¹1,101.50 |
| 300 | â‚¹1,420.00 |

## Future Improvements

- Store bill history in a database
- Add support for multiple tariff plans (domestic/commercial)
- PDF bill generation
- Multi-language support

## Screenshots

![Bill calculated](screenshots/bill-calculated.png)

