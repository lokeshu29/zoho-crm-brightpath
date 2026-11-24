# BrightPath Education: Requirements Document

> Independent portfolio project using fictional business and customer data. Not an official deployment for any real organization.

## 1. Client overview

BrightPath Education is a fictional coaching institute in Chennai (Anna Nagar branch) that teaches job-oriented IT and skill courses. It has about 40 admissions a month. The owner, Arun Kumar, wants to open a second branch but cannot tell which marketing channel or counsellor brings in admissions.

## 2. Team

| Person | Role | Responsibility |
|---|---|---|
| Arun Kumar | Owner | Views reports and revenue |
| Meena Raj | Sales Manager | Manages counsellors, approves fee discounts |
| Karthik S | Counsellor 1 | Python and Data Analytics enquiries |
| Divya R | Counsellor 2 | Java Full Stack, Web Development, Digital Marketing enquiries |

## 3. Courses and fees

| Course | Fee (INR) | Duration |
|---|---|---|
| Python Programming | 25,000 | 3 months |
| Data Analytics | 35,000 | 4 months |
| Java Full Stack | 45,000 | 5 months |
| Web Development | 30,000 | 3 months |
| Digital Marketing | 20,000 | 2 months |

## 4. Current problems

1. Enquiries are scattered across email, Excel, paper and phones.
2. Counsellors forget follow-up calls.
3. Two counsellors sometimes call the same student.
4. Fee discounts are given with no approval.
5. The owner cannot see conversion rates, best lead source or counsellor performance.
6. Reasons for lost students are never recorded.

## 5. Objectives

1. Centralize all student enquiries in Zoho CRM.
2. Assign leads to the right counsellor automatically.
3. Ensure every lead gets a welcome email and a follow-up task.
4. Control fee discounts through manager approval.
5. Give the owner reports on sources, conversions and counsellor performance.

## 6. Business rules

**Lead Status:** New, Contacted, Interested, Demo Scheduled, Not Interested, Junk

**Deal stages:** New Enquiry, Counselling Done, Demo Attended, Fee Quoted, Negotiation, Admission Confirmed (Won), Closed Lost

**Lost reasons:** Fees too high, Joined another institute, Not responding, Postponed, Other

**Assignment:**
- Python or Data Analytics goes to Karthik
- Java Full Stack, Web Development or Digital Marketing goes to Divya
- Budget above 40,000 also notifies Meena

**Validation:** phone number must be exactly 10 digits.

**Approval:** a discount above 10% goes to Meena for approval.

## 7. Custom fields

| Module | Field | Type |
|---|---|---|
| Leads | Course Interest | Picklist |
| Leads | Preferred Batch | Picklist |
| Leads | Budget | Currency |
| Leads | Qualification | Picklist |
| Deals | Course Fee | Currency |
| Deals | Discount % | Percent |

## 8. Reports required

- Leads by source
- Deals by stage
- Admissions per counsellor
- Lead-to-admission conversion rate
- Monthly admission revenue
- Lost deals by reason

## 9. Success criteria

- Every new lead is assigned to a counsellor automatically.
- Every lead gets a welcome email and a follow-up task.
- A discount above 10% cannot be confirmed without approval.
- A counsellor sees only their own leads; the manager sees the whole team.
- The owner can see all key numbers on one dashboard.

## 10. Assumptions and scope

- All data is fictional.
- The website form is simulated and emails are sent to a test address.
- Out of scope: payment gateway, Zoho Books, WhatsApp integration.

## 11. Deliverables

Configured Zoho CRM organization, this requirements document, configuration documentation with screenshots, sample data, counsellor user guide, troubleshooting log, and a demo video.
