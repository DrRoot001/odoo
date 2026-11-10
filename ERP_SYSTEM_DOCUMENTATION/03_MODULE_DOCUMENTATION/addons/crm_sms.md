# Module: crm_sms

- **Module ID:** MOD-060
- **Path:** `addons/crm_sms`
- **Manifest:** `addons/crm_sms/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Add SMS capabilities to CRM

No manifest description declared.

Declared dependencies: `crm`, `sms`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "crm",
    "sms"
  ],
  "data": [
    "views/crm_lead_views.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/crm_sms/__init__.py` (2 lines)
- `addons/crm_sms/__manifest__.py` (16 lines)
- `addons/crm_sms/i18n/ar.po` (44 lines)
- `addons/crm_sms/i18n/az.po` (41 lines)
- `addons/crm_sms/i18n/bg.po` (41 lines)
- `addons/crm_sms/i18n/bs.po` (42 lines)
- `addons/crm_sms/i18n/ca.po` (41 lines)
- `addons/crm_sms/i18n/crm_sms.pot` (37 lines)
- `addons/crm_sms/i18n/cs.po` (44 lines)
- `addons/crm_sms/i18n/da.po` (44 lines)
- `addons/crm_sms/i18n/de.po` (46 lines)
- `addons/crm_sms/i18n/el.po` (41 lines)
- `addons/crm_sms/i18n/es.po` (45 lines)
- `addons/crm_sms/i18n/es_419.po` (42 lines)
- `addons/crm_sms/i18n/et.po` (41 lines)
- `addons/crm_sms/i18n/fa.po` (41 lines)
- `addons/crm_sms/i18n/fi.po` (42 lines)
- `addons/crm_sms/i18n/fr.po` (45 lines)
- `addons/crm_sms/i18n/he.po` (46 lines)
- `addons/crm_sms/i18n/hi.po` (41 lines)
- `addons/crm_sms/i18n/hr.po` (44 lines)
- `addons/crm_sms/i18n/hu.po` (43 lines)
- `addons/crm_sms/i18n/id.po` (41 lines)
- `addons/crm_sms/i18n/it.po` (45 lines)
- `addons/crm_sms/i18n/ja.po` (42 lines)
- `addons/crm_sms/i18n/kab.po` (41 lines)
- `addons/crm_sms/i18n/ko.po` (41 lines)
- `addons/crm_sms/i18n/ku.po` (40 lines)
- `addons/crm_sms/i18n/lo.po` (40 lines)
- `addons/crm_sms/i18n/lt.po` (45 lines)
- `addons/crm_sms/i18n/lv.po` (43 lines)
- `addons/crm_sms/i18n/mn.po` (44 lines)
- `addons/crm_sms/i18n/my.po` (41 lines)
- `addons/crm_sms/i18n/nb.po` (44 lines)
- `addons/crm_sms/i18n/nl.po` (45 lines)
- `addons/crm_sms/i18n/pl.po` (46 lines)
- `addons/crm_sms/i18n/pt.po` (41 lines)
- `addons/crm_sms/i18n/pt_BR.po` (44 lines)
- `addons/crm_sms/i18n/ro.po` (42 lines)
- `addons/crm_sms/i18n/ru.po` (45 lines)
- `addons/crm_sms/i18n/sk.po` (42 lines)
- `addons/crm_sms/i18n/sl.po` (42 lines)
- `addons/crm_sms/i18n/sr@latin.po` (42 lines)
- `addons/crm_sms/i18n/sv.po` (42 lines)
- `addons/crm_sms/i18n/th.po` (41 lines)
- `addons/crm_sms/i18n/tr.po` (43 lines)
- `addons/crm_sms/i18n/uk.po` (46 lines)
- `addons/crm_sms/i18n/uz.po` (50 lines)
- `addons/crm_sms/i18n/vi.po` (43 lines)
- `addons/crm_sms/i18n/zh_CN.po` (45 lines)
- `addons/crm_sms/i18n/zh_TW.po` (44 lines)
- `addons/crm_sms/security/ir.access.csv` (3 lines)
- `addons/crm_sms/tests/__init__.py` (3 lines)
- `addons/crm_sms/tests/test_crm_lead.py` (27 lines)
- `addons/crm_sms/views/crm_lead_views.xml` (53 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
