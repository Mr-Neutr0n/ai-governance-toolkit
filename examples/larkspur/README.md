# Larkspur Utilities example

A second worked example, next to [Fernhill](../fernhill/). Larkspur Utilities Ltd is a fictional energy supplier, and everything here is invented. It focuses on AI in customer service, so a reader in a contact centre can see the templates filled in for their own setting.

| File | What it shows |
|---|---|
| [ai-system-inventory.csv](ai-system-inventory.csv) | Four systems: a billing chat assistant, a call summary tool, a complaint triage pilot and a proposed model that is not yet classified |
| [ai-risk-register.csv](ai-risk-register.csv) | Eleven risks, including a high residual risk that is still being treated |
| [ai-incident-log.csv](ai-incident-log.csv) | Three incidents, one of them still under investigation with a reporting decision pending |
| [ai-impact-assessment.md](ai-impact-assessment.md) | The impact assessment template completed for the billing assistant |
| [control-mapping.md](control-mapping.md) | Which toolkit controls the example evidences, and where |

The validator checks these CSV files with the same rules as Fernhill, and the register health report can be run on them:

```bash
python tools/validate_and_report.py
python tools/register_health.py --registers examples/larkspur --as-of 2026-11-19
```

The EU AI Act tier labels are used as a common reference. Whether the Act applies to a real supplier like this depends on its facts, so check before relying on any label here.
