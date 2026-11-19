# Impact assessment: Larkie billing assistant (fictional)

> General information only, not legal advice. Larkspur Utilities Ltd is a fictional company and every entry in this file is invented. It is the filled-in version of [the impact assessment template](../../templates/ai-impact-assessment.md).

Supports controls TK-RSK-03, TK-RSK-04, TK-RSK-05, TK-INV-03 and TK-USE-03. The system is LE-AI-001 in the [inventory](ai-system-inventory.csv), and the risks below are in the [risk register](ai-risk-register.csv).

### 0. Details

| Field | Entry |
|---|---|
| Assessment reference | LE-IA-001 |
| System ID | LE-AI-001 |
| System name | Larkie billing assistant |
| Assessment owner | Head of Customer Operations |
| Contributors | Data protection officer, Contact Centre Manager, Digital Channels Manager, Compliance lead, one customer advice volunteer |
| Date | 2026-04-14 |
| Version | 1.0 |
| Trigger | New system |

### 1. Screening

| Question | Yes / No |
|---|---|
| Influences a decision about a person | No (it answers questions; staff make account decisions) |
| Processes personal data | Yes |
| Used with children or vulnerable people | Yes (customers in vulnerable circumstances use the service) |
| Annex III area or banned practice | No (not an Annex III use; see section 3 for the banned practice check) |
| Direct interaction or generated content | Yes |

Three answers are yes, so the full form was completed.

### 2. Purpose and context

- **Intended purpose:** Answer routine questions about bills, meter readings and tariffs in the customer app and on the website, and hand over to a person when the assistant is unsure or the customer asks.
- **Who will use it:** Domestic and small business customers, about 9,000 chats a month expected.
- **Who will be affected by outputs:** The same customers, and contact centre agents who receive handovers.
- **Without the system:** Customers wait on the phone or by email. The average phone wait last winter was 11 minutes.
- **Why AI is needed:** Questions are phrased in many ways, so a fixed menu resolves fewer queries. A rules-only option was trialled and handled about a third of queries.

### 3. Prohibited practice check

| Practice considered | Conclusion | Evidence |
|---|---|---|
| Manipulative or deceptive techniques (Art 5(1)(a)) | Not engaged | The assistant cannot make offers or upsell, and its prompts forbid pressure or urgency language. Reviewed by the compliance lead |
| Exploiting vulnerabilities (Art 5(1)(b)) | Not engaged, with a control | Priority services customers are always routed to staff; reviewed monthly under risk LE-R-002 |
| Emotion recognition, social scoring, biometric categorisation | Not applicable | No such function exists |

Legal advice was taken on the vulnerability point because a wrong answer would affect people who need extra care.

### 4. Impact analysis

| Affected group | Possible benefit | Possible harm | Likelihood (1 to 5) | Severity (1 to 5) | Reversible? |
|---|---|---|---|---|---|
| Customers generally | Quick answers outside office hours | Wrong tariff or balance leads to a wrong decision | 4 | 3 | Yes |
| Customers in vulnerable circumstances | Less waiting | Not recognised, so not handed to a person | 3 | 5 | Partly |
| Customers using sensitive words in chat | None specific | Payment details stored by the supplier | 3 | 4 | No |
| Contact centre agents | Fewer routine contacts | Handovers arrive without context | 2 | 2 | Yes |

### 5. Mitigations and residual impact

| Impact | Mitigation | Owner | Date | Residual level |
|---|---|---|---|---|
| Wrong tariff or balance | Live tariff service only; refuse when the feed is stale; weekly sampling | Head of Customer Operations | 2026-12-11 | Medium |
| Vulnerable customer not handed over | Priority services flag always routes to staff; distress keywords; monthly review | Head of Customer Operations | 2026-12-04 | High until the flag fix is confirmed |
| Payment details stored | Masking before storage; 30 day retention cap | Data protection officer | 2026-12-18 | Medium |
| Handover without context | Assistant sends a short summary with every handover | Digital Channels Manager | 2026-05-01 | Low |

The material impacts are in the risk register as LE-R-001, LE-R-002 and LE-R-004. Incident LE-INC-003 showed that the second one was not fully controlled, so the residual level was raised after go-live.

### 6. Transparency and redress

- **What people are told:** A banner and the first message say that the assistant is automated, and a link explains what data is kept and for how long.
- **Human review or explanation:** A "talk to a person" button is always visible. Complaints about the assistant go to the normal complaints route.
- **Workers:** Contact centre agents were briefed before launch and their representatives were told about the handover rules.

### 7. Links

- **DPIA reference:** LE-DPIA-004
- **Supplier review reference:** LE-VR-002 (ChatBridge Ltd, fictional)
- **System card reference:** LE-SC-001
- **Human oversight checklist reference:** LE-HO-001

### 8. Decision and sign-off

| Decision | Approve with conditions |
|---|---|
| Conditions | 30 day retention cap in the contract; priority services flag test passed before launch; review again after 6 months |
| Approver | Chief Operating Officer |
| Date | 2026-04-28 |
| Next review date | 2027-05-10 |
