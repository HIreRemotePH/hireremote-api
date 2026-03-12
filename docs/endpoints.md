# API Endpoints

The HireRemote API provides access to job listings, companies, and salary insights available on HireRemote.ph.

---

## Base URL

```
https://api.hireremote.ph
```

All API requests should be made to the base URL above.

Example:

```
GET https://api.hireremote.ph/api/jobs
```

---

## Retrieve Jobs

```
GET /api/jobs
```

Returns available remote job listings.

### Example Request

```
GET https://api.hireremote.ph/api/jobs?location=philippines&remote=true
```

### Headers

```
Content-Type: application/json
```

### Example Response

```json
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
```

### Response Fields

title — job title  
company — hiring company  
location — job location (Remote / Hybrid / On-site)  
salary_range — estimated compensation range

---

## Retrieve Companies

```
GET /api/companies
```

Returns companies currently hiring remote workers.

### Example Request

```
GET https://api.hireremote.ph/api/companies
```

### Headers

```
Content-Type: application/json
```

---

## Salary Data

```
GET /api/salary-data
```

Returns salary insights for remote positions.

### Example Request

```
GET https://api.hireremote.ph/api/salary-data
```

### Headers

```
Content-Type: application/json
```

---

## Employer Job Posting

```
POST /api/employer/job-post
```

Allows employers to post remote job opportunities.

### Headers

```
Content-Type: application/json
```

### Required Fields

- job_title
- company
- location
- salary_range
- job_description

### Example Request Body

```json
{
  "job_title": "Remote UX Designer",
  "company": "Example Company",
  "location": "Remote",
  "salary_range": "$60,000 - $90,000",
  "job_description": "Design user interfaces for remote products."
}
```
