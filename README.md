# Employee Control 2026
## Employee Control 2026 is a lightweight internal portal for employee registration and consultation.

<img width="800" height="700" alt="Employee Control" src="https://github.com/user-attachments/assets/191e9804-acc6-4c05-86d4-64943f4c2e24" />



## Hosting

This project is hosted on **Cloudflare**.

## Overview

The application is a single-page interface built with HTML, Tailwind CSS (CDN), and vanilla JavaScript. It allows teams to:

- Register employee records
- Search and filter existing records
- Import employee data from CSV files
- Track import audit information (user and timestamp)
- Use light/dark theme modes

## Main Modules

- **Register**: Add new employee records with key fields such as CPF, employee ID, name, region, admission date, and termination date.
- **Consult**: Search, sort, paginate, and filter records by region and admission period.
- **Import CSV**: Bulk import data using a CSV file with required headers.

## Tech Stack

- HTML5
- Tailwind CSS (via CDN)
- Vanilla JavaScript
- LocalStorage for client-side persistence

## Project Structure

```text
  User
   |
   v
Cloudflare Pages (Frontend)
   |
   v
Cloudflare Workers (API)
   |
   v
Cloudflare D1 (Database)
```
"`n## Feature`nAdiciona autenticação local no Employee Control"
