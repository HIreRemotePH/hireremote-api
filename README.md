# HireRemote API

This repository documents the API and integrations used by HireRemote.ph.

HireRemote connects Filipino professionals with companies hiring remotely worldwide.

Website
https://hireremote.ph

## API Overview

The HireRemote API powers integrations between the HireRemote.ph platform and external systems.

Core API capabilities include:

- Job listing retrieval
- Employer posting endpoints
- Candidate discovery tools
- Salary data access
- Platform analytics integrations

- ## Future Integrations

The HireRemote API will support integrations with:

- Applicant Tracking Systems (ATS)
- HR platforms
- Remote hiring marketplaces
- Recruitment automation tools

## Example Endpoint

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
