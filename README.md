# FUTURE_CS_03 — API Security Risk Analysis

## Project Overview
This project focuses on understanding common API security risks and documenting potential weaknesses that should be considered when securing web applications.

A locally hosted OWASP Juice Shop application was used as an educational reference. Browser Developer Tools were used to observe network requests, and the findings were documented as a preliminary API security risk analysis.

## Objectives
- Understand the role of APIs in web applications.
- Observe application network requests and responses.
- Identify potential API security risks for further investigation.
- Recommend security controls and testing practices.
- Prepare a report with supporting evidence.

## Tools Used
- **OWASP Juice Shop** — Local educational web application.
- **Browser Developer Tools** — Inspect network requests and responses.
- **Docker Desktop** — Run the application locally.
- **PDF report and screenshots** — Document observations and recommendations.

## Methodology
1. Start the local OWASP Juice Shop application.
2. Open the application in a web browser.
3. Use the Network tab in Developer Tools to observe requests.
4. Review visible request details and response information.
5. Map general observations to relevant API security risks.
6. Document recommendations for additional authorized testing.

## API Security Risks Considered
- **Broken Object Level Authorization (BOLA):** Users accessing objects they are not authorized to view or modify.
- **Broken Authentication:** Weaknesses in verifying user identity.
- **Broken Function Level Authorization:** Users accessing functions beyond their permissions.
- **Unrestricted Resource Consumption:** Insufficient limits on requests or resource usage.
- **Security Misconfiguration:** Insecure headers, settings, or error handling.
- **Sensitive Data Exposure:** APIs returning more sensitive information than necessary.

These are general risk categories considered during the analysis, not confirmed vulnerabilities in the tested application.

## Key Observations
- Browser Developer Tools showed network activity associated with the local application.
- The observed requests provided a starting point for understanding how the frontend communicates with application endpoints.
- Network observation alone does not establish that an API vulnerability exists.
- Further authorized testing would be needed to verify authentication, authorization, input validation, rate limiting, and data exposure controls.

## Recommendations
- Enforce server-side authentication and authorization checks on every protected endpoint.
- Verify that users can access only the objects and functions permitted to them.
- Validate inputs and apply appropriate output handling.
- Apply rate limits and resource-consumption controls.
- Avoid returning unnecessary sensitive data or detailed internal errors.
- Configure security headers and cross-origin policies appropriately.
- Log relevant security events and review them for suspicious activity.
- Retest identified risks and document reproducible evidence before reporting confirmed vulnerabilities.

## Deliverables
- `report/API_Security_Risk_Analysis_Report.pdf` — Project report
- Browser network activity screenshot
- API observation notes
- Supporting evidence

## Limitations
This was a preliminary educational risk analysis based on observed browser network activity. No confirmed API vulnerability is claimed, and comprehensive authorization, authentication, or penetration testing was not performed.

## Disclaimer
This project was conducted for educational cybersecurity purposes using a locally hosted application. Only test systems for which you have explicit authorization.

## Author
**V. Karthik**  
Cybersecurity Student
