# Module: test_crm_full

- **Module ID:** MOD-570
- **Path:** `addons/test_crm_full`
- **Manifest:** `addons/test_crm_full/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This module is intended to test the main crm flows of Odoo, both frontend and
backend. It notably includes IAP bridges modules to test their impact. 

Declared dependencies: `crm`, `crm_iap_enrich`, `crm_iap_mine`, `crm_sms`, `event_crm`, `sale_crm`, `website_crm`, `website_crm_iap_reveal`, `website_crm_partner_assign`, `website_crm_livechat`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 5 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "crm",
    "crm_iap_enrich",
    "crm_iap_mine",
    "crm_sms",
    "event_crm",
    "sale_crm",
    "website_crm",
    "website_crm_iap_reveal",
    "website_crm_partner_assign",
    "website_crm_livechat"
  ]
}
```

### Representative source files

- `addons/test_crm_full/__init__.py` (2 lines)
- `addons/test_crm_full/__manifest__.py` (23 lines)
- `addons/test_crm_full/tests/__init__.py` (4 lines)
- `addons/test_crm_full/tests/common.py` (41 lines)
- `addons/test_crm_full/tests/test_performance.py` (133 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
