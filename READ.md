# CRM Data Model (Foundry-Style Project)

This project demonstrates how I designed a CRM-style data model inspired by my work in Palantir Foundry.

## Overview
The goal was to transform messy raw datasets into a clean, explorable business model.

The system models three core entities:
- PERSON
- COMPANY
- EMPLOYMENT (relationship object)

## Key Concepts

### Data Cleaning
- Removed null values
- Standardized company names
- Generated stable identifiers

### Data Modeling
Instead of directly linking people to companies, I created an EMPLOYMENT object.
This correctly models real-world relationships:
- One person can have multiple employments
- One company can have many employees

### Identifiers Used
- person_id → unique person
- company_key → normalized company identifier
- employment_id → generated relationship identity

### Result
The final system allows:
- Exploring companies and their employees
- Viewing employment relationships
- Filtering and querying structured business data

This repository contains architecture diagrams, pipeline explanations, and example queries.  
No proprietary platform exports or real data are included.
