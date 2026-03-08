Voucher Generator PRO+

A lightweight browser-based voucher generator designed to create mass promotional vouchers with unique codes and QR validation — without requiring a backend server.

This tool allows businesses, marketers, and event organizers to generate, design, and print voucher campaigns instantly using only a browser.

Built with a pure front-end stack, Voucher Generator PRO+ leverages LocalStorage as a lightweight database, enabling fast deployment with zero infrastructure.

Key Highlights

Mass voucher generation

Automatic QR Code creation

Unique voucher code system

Drag & drop layout customization

Print-ready A4 voucher sheets

Built-in voucher redeem validation

No backend required

Lightweight and portable

Preview Workflow
Create Voucher Campaign
│
▼
Generate Unique Codes
│
▼
QR Code Attached to Voucher
│
▼
Print Voucher Sheet (A4)
│
▼
User Scans QR Code
│
▼
System Validates Voucher
│
├── Valid → Redeemed
└── Invalid / Used → Rejected
Main Features

1. Bulk Voucher Generation

Generate hundreds of vouchers in seconds by defining:

number of pages

vouchers per page

code prefix

layout orientation

Example generated codes:

DMT-3K7L9X
DMT-A9F2QW
DMT-ZL8P1H

Each code is automatically guaranteed to be unique during generation.

2. Automatic QR Code Validation

Every voucher includes a QR Code pointing to a validation URL.

Example:

https://yourdomain.com/voucher.html?redeem=DMT-A9F2QW

When scanned:

system checks the voucher code

if valid → marked as redeemed

if used → rejected

Powered by:

QRCode.js

3. Drag & Drop Layout Builder

All voucher elements are fully draggable, enabling custom design layouts without editing code.

Editable elements include:

logo

voucher title

subtitle

price

discount price

voucher code

issuer label

QR code

Drag engine powered by:

Interact.js

4. Flexible Voucher Configuration

The generator interface supports customizable parameters:

Field Description
Issuer Brand or company issuing the voucher
Title Voucher promotion title
Subtitle Additional promotion detail
Price Promotional price
Old Price Original price before discount
Code Prefix Prefix for voucher codes
Page Count Number of pages to generate
Vouchers per Page Density of vouchers
Orientation Landscape or Portrait
Logo Upload Brand logo
WhatsApp Number Optional contact QR 5. Print-Ready A4 Layout

Generated vouchers are automatically formatted for A4 printing.

CSS print rules dynamically adjust layout:

@media print

Default print layout:

2 columns per page

consistent spacing

printer-friendly margins

Perfect for:

voucher campaigns

coupons

event tickets

course access vouchers

Technology Stack

This project intentionally uses a minimalistic front-end stack.

Technology Role
HTML5 Application structure
CSS3 Layout and print styling
JavaScript Voucher generation logic
QRCode.js QR code generation
Interact.js Drag-and-drop layout
LocalStorage Lightweight voucher database

No dependencies on:

backend frameworks

server APIs

external databases

Project Structure
voucher-generator-pro
│
├── index.html
├── README.md
│
├── assets
│ ├── logo
│ └── screenshots
│
└── libraries
├── qrcode.js
└── interact.js
Installation

Clone the repository:

git clone https://github.com/yourusername/voucher-generator-pro.git

Open the application:

index.html

Run directly in any modern browser.

No build tools required.

How to Use

1. Configure Voucher Settings

Fill the generator form:

voucher title

price

issuer name

code prefix

page count

2. Generate Vouchers

Click:

Generate Voucher

The system will automatically create all voucher cards.

3. Adjust Layout (Optional)

Drag elements to customize voucher appearance.

4. Print Vouchers

Click:

Print A4

Your vouchers will be printed in a sheet layout.

Voucher Redemption System

Voucher redemption works via URL parameter validation.

Example URL:

?redeem=DMT-9KLX3F

Validation logic:

Condition Result
Code exists Voucher redeemed
Already used Rejected
Not found Invalid voucher

Database example:

{
"DMT-9KLX3F": {
"redeemed": true
}
}

Stored locally in:

localStorage
Limitations

Because the system uses LocalStorage, it has several constraints:

voucher data stored only on one device

not synchronized across browsers

not suitable for high-scale voucher campaigns

For production-grade deployments consider:

REST API backend

cloud database

centralized validation server

Roadmap

Planned improvements:

PDF export generator

voucher analytics dashboard

admin management panel

multi-device database sync

template marketplace

WhatsApp auto redemption

Firebase integration

SaaS deployment version

Contribution

Contributions are welcome.

Typical improvements include:

UI enhancements

additional voucher templates

improved QR redemption system

export features

Workflow:

Fork → Create Branch → Commit → Pull Request
License

This project is released under the MIT License.

You are free to use it for:

commercial projects

educational purposes

marketing tools

promotional campaigns

Author

Developed by Diamant Digital

Focused on building marketing automation tools and lightweight web systems.
