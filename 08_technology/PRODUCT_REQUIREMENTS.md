# Technology MVP — Human-First
## Phase 0 (pilot)
Avoid building software prematurely. Use secure, access-controlled tools for guardian inquiries, consent status, attendance, anonymized feedback and financial reporting.
## Minimal data model
Guardian ID/contact; child pseudonymous enrollment ID, age band, attendance; emergency contact stored in restricted operational system; optional guardian feedback; incident data separately restricted. Do not create behavioral scores.
## Capabilities
Public landing page; guardian interest form; staff dashboard with role permissions; attendance; curriculum content library; anonymized cohort metrics; deletion/export workflow.
## Explicit exclusions
Child-facing unrestricted LLM; facial recognition; automated child ranking; emotional inference; targeted advertising to children; unnecessary geolocation; recording by default.
## Security
MFA for staff; least privilege; encrypted storage and transport; audit logs; backups; retention schedule; data breach playbook; third-party processor contracts reviewed by counsel.
## AI support
Adult-facing draft generator for lesson alternatives and parent updates, with human approval and no identifiable child data.


---
## Detailed implementation supplement

## Functional product contract
**Visitor:** sees program, schedule status and safeguarding contact without tracking children. **Guardian:** obtains reviewed terms and optional consent using secure adult-only system. **Admissions staff:** handles eligible inquiry and fee without full child observations. **Facilitator:** reads minimum attendance/accommodation information. **Safeguarding lead:** holds restricted incident records, separate from ordinary dashboards. **Finance:** sees payment references without unnecessary child PII.

**Must-pass tests:** an unauthorized account cannot see guardian data; pickup authorizations are auditable; refund and consent revisions are versioned; offline emergency roster is securely available to designated people; withdrawal and deletion follow reviewed retention policy; restore test succeeds; public pages contain no real child data.

**Nonfunctional:** encrypted network and storage, role-based access, secure credentials, consent-logging, change approvals, backups, minimal third-party analytics, accessible mobile UX, and human review for any AI-produced educational output.

**Scope decision:** marketing prototype first; no custom child accounts or direct AI chatbot in pilot. Deploy real enrollment/payments only after privacy, legal and security gates.