# Test Plan: AI Smart Shopper

## 1. Objective
To validate the core functionality, security, and usability of the AI Smart Shopper web application, ensuring it meets the needs of NSFAS students managing their budgets.

## 2. Scope
*   **In Scope:** User Authentication (Login/Rate Limiting), Budget Creation rules (NSFAS warnings), Shopping List logic (Over-budget locking), API validation (Negative quantities).
*   **Out of Scope:** Admin portal, third-party API integrations, map routing, Microsoft SSO.

## 3. Test Strategy
Testing will be executed manually using a **Risk-Based Approach**, prioritizing critical business logic (Budget and Shopping List rules) and security (API input validation and Rate Limiting).

## 4. Environment
*   **Browser:** Google Chrome (v154)
*   **OS:** Windows 11
*   **Environment:** Local Development (http://127.0.0.1:5000)
