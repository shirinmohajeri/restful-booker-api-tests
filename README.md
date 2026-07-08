# RESTful Booker API Tests

## Overview

This repository contains an API testing project built with Postman, focused on validating REST API behavior using GET and POST requests against RESTful Booker, a public demo API that simulates a hotel booking system.

This project was developed to improve my skills in API testing, REST principles, and using Postman as a professional QA tool.

---

## My Role

- Designed and built a Postman collection covering GET and POST requests
- Tested happy-path scenarios (valid requests, expected data) and negative scenarios (missing fields, invalid IDs)
- Investigated and documented unexpected API behavior through structured debugging
- Created my own test data via POST to ensure stable, repeatable test conditions

---

## Technologies Used

- Postman
- REST API principles (HTTP methods, endpoints, status codes)
- JSON

---

## Key Features

- GET requests: all bookings, booking by ID, filtered by query parameters, invalid ID handling
- POST requests: create booking with valid data, create booking with missing fields
- Structured debugging approach: isolating variables to identify the true cause of unexpected results
- Documented findings on real API quirks (see below)

---

## What I Learned

- RESTful Booker returns `200 OK` for POST requests instead of the `201 Created` that REST conventions typically expect — a reminder that real APIs don't always follow textbook rules, and a tester's job is to verify actual behavior.
- Shared public test data is unreliable, since many people practice against it at once. This taught me to isolate variables when a test unexpectedly fails, and to create my own booking data so I always have stable, known records to test against.
- Query parameters require exact formatting — a missing leading zero in a date value was enough to make a filter silently return zero results with a `200 OK`, with no error message at all.

---

## Purpose

The goal of this project is to demonstrate my ability to test REST APIs methodically, debug unexpected results, and think critically about API behavior — core skills for a QA / API testing role.

---

## How to Run

1. Clone this repository
2. Open Postman
3. Import `RESTful-Booker-API-Tests.postman_collection.json` from this repo
4. Run requests individually, or use the Postman Runner to run the full collection

---

## Contact

Shirin Mohajeri
Email: shirin.mohajeri6b8@yahoo.com
GitHub: <https://github.com/shirinmohajeri/>
LinkedIn: [www.linkedin.com/in/shirin-mohajeri](http://www.linkedin.com/in/shirin-mohajeri)
