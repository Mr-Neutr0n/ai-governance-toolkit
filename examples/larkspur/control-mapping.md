# Control mapping: Larkspur example (fictional)

> General information only, not legal advice. Larkspur Utilities Ltd is fictional and every entry is invented.

This table shows how the fictional organisation evidences some controls from the toolkit's [control matrix](../../docs/control-matrix.md). It covers the controls the example material touches, not the whole library. Every control ID is checked against the matrix by the tests.

| Control | Name | What Larkspur did | Where the evidence is |
|---|---|---|---|
| TK-INV-01 | AI system inventory | LE-AI-001 to LE-AI-004 are listed with owners, tier and review dates | [Inventory](ai-system-inventory.csv) |
| TK-INV-02 | Risk classification and role check | Assistant classed as transparency; the proposed flag model is left as not assessed until reviewed | Inventory columns `eu_risk_tier`, `eu_ai_act_role` |
| TK-INV-03 | Prohibited practice screening | Art 5 points considered and recorded for the assistant | [Impact assessment](ai-impact-assessment.md), section 3 |
| TK-RSK-03 | AI system impact assessment | Full assessment LE-IA-001 completed before launch and signed off with conditions | [Impact assessment](ai-impact-assessment.md) |
| TK-RSK-04 | Fundamental rights and data protection check | DPIA LE-DPIA-004 linked from the assessment; the proposed flag model is blocked until its DPIA is done | Impact assessment section 7; risk LE-R-010 |
| TK-LIF-06 | Operational monitoring | Weekly transcript sampling; stale-feed block on tariff answers | Risk LE-R-001; incident LE-INC-001 |
| TK-LIF-09 | Human oversight | Handover rules, agent confirmation of call summaries, handler confirmation of triage bands | Inventory column `human_oversight`; risks LE-R-002, LE-R-007, LE-R-009 |
| TK-DAT-03 | Privacy review of AI use | Masking of card details in chat; recording paused during payment | Risks LE-R-004 and LE-R-006; incident LE-INC-002 |
| TK-USE-02 | Disclosure of AI interaction and content | Banner and first message identify the assistant as AI | Risk LE-R-003 (closed) |
| TK-USE-04 | Appeals complaints and redress | Talk to a person button; normal complaints route | Impact assessment section 6 |
| TK-THR-02 | Contract terms and shared responsibility | 30 day retention cap and change-notice clause with ChatBridge Ltd (fictional) | Risks LE-R-004 and LE-R-005 |
| TK-INC-01 | Incident detection and response | Three incidents logged with corrective actions; one under investigation | [Incident log](ai-incident-log.csv) |
| TK-INC-02 | External reporting and authority liaison | Reporting decision for LE-INC-003 is under assessment, with an owner | Incident LE-INC-003 |

Controls with no row here, such as the management system scope (TK-GOV-04) or internal audit (TK-GOV-10), are not evidenced by this example. A real organisation would need evidence for them too.
