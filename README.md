# Brew Haven Feedback

A mobile-friendly feedback and operations app for Brew Haven, a local coffee shop. It's a single HTML page with no build step and no server.

**Live site:** https://austinnguan.github.io/brewhaven/

## What's in it

| Tab | Who uses it | What it does |
|---|---|---|
| **Feedback** | Customers | 1–5 star ratings for coffee quality, service speed, atmosphere and overall experience, plus what they ordered, their favorite item, time of visit and an optional comment. Shows a thank-you screen, then resets for the next guest. |
| **Staff** | Baristas | One-tap busy check-ins (Slow period, Moderate traffic, Very busy, Rush period) with staff on duty and notes. An order timer records how long each drink takes to make. |
| **Dashboard** | Owner | Average ratings by category, response count, recent comments, today's busy periods, peak hours, drink prep times against target, most popular items and the lowest-rated areas. |
| **Ideas** | Owner | Suggestions built from the data (staffing, prep, menu, atmosphere, rewards and loyalty) and an ROI estimate you can adjust. |

## Scenario data

The Dashboard and Ideas tabs can load an example day: 25 customer responses (coffee 4.2, service 3.8, atmosphere 3.5, Caramel Latte most popular) with peaks at 8–10 AM and 2–3 PM. It's example data for demonstration and is never saved. A copy is in [`brew-haven-scenario.json`](brew-haven-scenario.json).

## Where data is stored

On GitHub Pages the app saves responses in the browser's local storage, so data stays on the device it was entered on. That works for a single shop tablet used for both feedback and staff check-ins. Sharing data across several devices would need a backend (for example Firebase or Supabase).

## Run it locally

Open `index.html` in any browser.
