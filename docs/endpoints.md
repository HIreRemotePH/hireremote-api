# API Endpoints

The HireRemote API provides access to job listings, companies, and salary insights available on HireRemote.ph.

Base URL

https://api.hireremote.ph

---

## Retrieve Jobs

GET /api/jobs

Returns available remote job listings.

Example request:

GET /api/jobs?location=philippines&remote=true

Example response:

{
  "jobs": [
    {
      "title": "Remote Software Engineer",
      "company": "Global Tech Inc",
      "location": "Remote",
      "salary_range": "$70,000 - $100,000"
    }
  ]
}

---

## Retrieve Companies

GET /api/companies

Returns companies currently hiring remote workers.

---

## Salary Data

GET /api/salary-data

Returns salary insights for remote positions.

---

## Employer Job Posting

POST /api/employer/job-post

Allows employers to post remote job opportunities.

Required fields:

- job_title
- company
- location
- salary_range
- job_description
