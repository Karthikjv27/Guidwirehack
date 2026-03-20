# Guidwirehack
# GigZo

Income protection for gig delivery workers during disruptions

---

## The Problem

Gig delivery workers earn on a daily basis. There is no fixed salary, no paid leave, and no backup when work stops.

When disruptions happen — like heavy rain, floods, pollution, strikes, or even platform outages — workers are unable to work, and their income drops immediately.

Even after the disruption ends, earnings don’t recover instantly. That gap is also not supported by any system.

---

## Coverage Scope

GigZo focuses only on:

**Income loss caused by external disruptions**

It does not cover:
- health or medical issues  
- accidents  
- vehicle damage  

The goal is to keep the system simple and focused on earning stability.

---

## Our Approach

GigZo is designed to handle the full timeline of a disruption.

### Before disruption
The system monitors signals like weather forecasts, air quality, and public events.  
If risk is high, coverage is adjusted in advance.

### During disruption
When a trigger condition is met, payout starts automatically.  
If the situation becomes more severe, the payout increases.

### After disruption
Income does not return to normal immediately.  
The system estimates this delay and provides temporary support.

---

## Example Scenario

A delivery partner is working in an area where heavy rain is expected.

- Rain is predicted → system prepares in advance  
- Rain crosses threshold → payout starts  
- Rain increases → payout increases  
- Flood confirmed → full payout given  
- After rain stops → recovery delay estimated  
- Additional support provided  

No manual claim is required.

---

## Application Workflow

1. Worker registers and sets payout details  
2. System evaluates risk based on location and history  
3. Weekly coverage is activated  
4. Real-time monitoring runs in the background  
5. Disruption is detected  
6. Validation and fraud checks are performed  
7. Payout is sent instantly  

---

## Key Features

- automatic payouts  
- no claim process  
- real-time monitoring  
- covers income loss (not assets)  
- supports recovery period  
- simple onboarding  

---

## Tech Stack

- Frontend: React Native (PWA)  
- Backend: Node.js (NestJS)  
- Database: PostgreSQL, Redis  
- ML Models: Python (prediction, time-series, recovery)  
- Blockchain: Hyperledger Fabric  
- Payments: UPI  

---

## Models Used

- Prediction model → estimates disruption probability  
- Time-series model → adjusts payout during event  
- Recovery model → estimates income recovery time  

---

## Transparency

All major system actions such as predictions, payouts, and decisions can be logged and verified if required.

---

## Why This Matters

Gig workers depend on consistent daily income.

Even short disruptions can affect their financial stability.

GigZo is designed to reduce that impact in a simple and automated way.

---

## Status

- concept defined  
- architecture planned  
- prototype in progress  

---

## Team

[Add your team details]

---

## Summary

GigZo helps gig workers maintain income stability when disruptions make it impossible to work.
