# Case Study: QuickVal

## Project Overview
**Client:** Internal project  
**Timeline:** 3 days  
**Budget:** N/A (internal build)

## The Challenge
Needed to validate email lists before sending cold outreach campaigns. Existing services charge per-email fees that add up fast when validating thousands of leads.

## The Solution
Built QuickVal - an email validation API + dashboard:

- Single email validation
- Bulk CSV upload (1000+ emails)
- Validation API for integrations
- Dashboard with history and stats
- Export validated lists

## Tech Stack
- **Frontend:** React + Tailwind CSS
- **Backend:** Node.js / Express
- **Validation:** DNS MX lookup, SMTP check, syntax validation
- **Hosting:** Vercel (frontend) + Railway (API)

## Timeline Breakdown

| Day | Work Completed |
|-----|----------------|
| 1 | API setup, single email validation, MX checks |
| 2 | Bulk upload, CSV parsing, async processing |
| 3 | Dashboard UI, history, export functionality |

## Validation Checks
1. **Syntax** - Valid email format
2. **Domain** - Domain exists
3. **MX Records** - Has mail server configured
4. **Disposable** - Not a temp email service
5. **Role-based** - Flags info@, admin@, etc.

## Results
- Working in 3 days
- Validates 1000 emails in ~30 seconds
- Saved hours of manual list cleaning

## Key Learnings
1. DNS lookups are fast; SMTP checks are slow
2. Rate limiting is crucial for bulk operations
3. Simple UI wins - just show valid/invalid

---

*Built fast, works great, solves a real problem.*
