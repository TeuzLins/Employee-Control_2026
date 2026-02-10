# Employee Control 2026

Employee Control 2026 is a lightweight internal portal for employee registration and consultation.

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

## Running Locally

Because this is a static app, you can run it directly in a browser:

1. Clone this repository.
2. Open `index.html` in your browser.

Or serve it with a local static server (recommended), for example:

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## Cloudflare Deployment Notes

For Cloudflare Pages:

- Set the build command to: `none` (or leave empty)
- Set the output directory to: `.`
- Ensure `index.html` is in the project root
