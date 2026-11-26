# Microfinance Business Management System

A web-based lending management system I built to run the day-to-day work of a small lending company. It handles client records, loan applications and approvals, payments and receipts, late penalties, reports, user roles, and database backups, all in one place.

## Features

- **Client management**: register clients with personal, contact and employment details, upload the front and back of a valid ID, search, update and delete records, and block duplicate IDs
- **Client portal**: clients can create their own account, apply for a loan, and check their balance, payment schedule and receipts
- **Loan applications**: choose the loan type, amount, term and purpose, with the interest, total payable and monthly installment calculated automatically
- **Approval workflow**: loan officers approve or reject applications, and every loan keeps a Pending, Approved or Rejected status
- **Interest computation**: flat rate or diminishing balance, depending on the loan type
- **Payments and receipts**: record the date, amount and mode of payment, update the remaining balance automatically, and generate a printable receipt for every transaction
- **Automatic penalties**: late installments are charged a penalty after the grace period, with no manual computing
- **Reports**: daily, weekly and monthly summaries of disbursed loans, collections and outstanding balances
- **User roles**: Admin, Loan Officer, Cashier and Client, each with their own login and access limits
- **Notifications and alerts**: payment due reminders, overdue loan alerts and system error alerts for the admin
- **Backup and recovery**: manual and daily backups, downloading a backup file, and restoring from a saved or uploaded file (deployed on pythonanywhere backup and recovery is not functional due to mysql being a paid subscription)
- **Client map**: see where clients live on an interactive map
- **REST API**: JSON endpoints for clients, loans, applications, payments and more under `/api/`
- **Admin site**: full create, read, update and delete on every table through the Django admin

## Sample admin account

+ Admin `User: rein | pass: rein`

## Tech Stack

- **Language**: Python
- **Framework**: Django
- **API**: Django REST Framework
- **Database**: MySQL, using the `mysqlclient` driver
- **Frontend**: HTML templates, CSS and vanilla JavaScript
- **Maps**: Leaflet.js with OpenStreetMap tiles
- **External API**: OpenStreetMap Nominatim, which turns client addresses into map locations
- **Other libraries**: Pillow (ID photo uploads), python-dotenv (environment settings), Faker (sample data)
- **Hosting**: PythonAnywhere, using Django's built-in SQLite database for the live demo

## About the Authors
<br>
  <table align="center" style="width: 100%; min-width: 800px; table-layout: fixed;">
    <tr>
        <td align="center" width="50%" style="padding: 0 25px;">
            <img src="https://github.com/sullezaaaron-sys.png" width="150" style="border-radius: 50%;"><br><br>
            <b>Aaron John B. Sulleza</b><br><br>
            <div align="center">
                <a href="https://github.com/sullezaaaron-sys">
                    <img src="https://raw.githubusercontent.com/gauravghongde/social-icons/master/SVG/Color/Github.svg" width="30">
                </a>
            </div>
        </td>
        <td align="center" width="50%" style="padding: 0 25px;">
            <img src="https://github.com/ShituzieKai.png" width="150" style="border-radius: 50%;"><br><br>
            <b>Kaiser Mamansag</b><br><br>
            <div align="center">
                <a href="https://github.com/ShituzieKai">
                    <img src="https://raw.githubusercontent.com/gauravghongde/social-icons/master/SVG/Color/Github.svg" width="30">
                </a>
            </div>
        </td>
        <td align="center" width="50%" style="padding: 0 25px;">
            <img src="https://media3.giphy.com/media/v1.Y2lkPTc5MGI3NjExc3AxcDVwcW91ajltd210YWtiNGdmcWpqdXY2OHE4djAyamUxczdodiZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/UDwXW80aYe6e93q53u/giphy.gif" width="150" style="border-radius: 50%;"><br><br>
            <b>Sean Reinmarc C. Broñola</b><br><br>
            <div align="center">
                <a href="https://github.com/reiinnn01">
                    <img src="https://raw.githubusercontent.com/gauravghongde/social-icons/master/SVG/Color/Github.svg" width="30">
                </a>
            </div>
        </td>
        <td align="center" width="50%" style="padding: 0 25px;">
            <img src="https://github.com/renz-202480288.png" width="150" style="border-radius: 50%;"><br><br>
            <b>Renz Bacongallo</b><br><br>
            <div align="center">
                <a href="https://github.com/renz-202480288">
                    <img src="https://raw.githubusercontent.com/gauravghongde/social-icons/master/SVG/Color/Github.svg" width="30">
                </a>
            </div>
        </td>
    </tr>
</table>
