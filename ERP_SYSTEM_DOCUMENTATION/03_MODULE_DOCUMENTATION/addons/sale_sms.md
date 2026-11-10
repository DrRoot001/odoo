# Module: sale_sms

- **Module ID:** MOD-532
- **Path:** `addons/sale_sms`
- **Manifest:** `addons/sale_sms/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Ease SMS integration with sales capabilities

Ease SMS integration with sales capabilities

Declared dependencies: `sale`, `sms`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 2 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sale",
    "sms"
  ],
  "data": [
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/sale_sms/__init__.py` (2 lines)
- `addons/sale_sms/__manifest__.py` (15 lines)
- `addons/sale_sms/i18n/ar.po` (27 lines)
- `addons/sale_sms/i18n/az.po` (27 lines)
- `addons/sale_sms/i18n/bg.po` (27 lines)
- `addons/sale_sms/i18n/bs.po` (27 lines)
- `addons/sale_sms/i18n/ca.po` (27 lines)
- `addons/sale_sms/i18n/cs.po` (27 lines)
- `addons/sale_sms/i18n/da.po` (27 lines)
- `addons/sale_sms/i18n/de.po` (31 lines)
- `addons/sale_sms/i18n/el.po` (27 lines)
- `addons/sale_sms/i18n/es.po` (31 lines)
- `addons/sale_sms/i18n/es_419.po` (27 lines)
- `addons/sale_sms/i18n/et.po` (27 lines)
- `addons/sale_sms/i18n/fa.po` (27 lines)
- `addons/sale_sms/i18n/fi.po` (31 lines)
- `addons/sale_sms/i18n/fr.po` (27 lines)
- `addons/sale_sms/i18n/he.po` (27 lines)
- `addons/sale_sms/i18n/hi.po` (27 lines)
- `addons/sale_sms/i18n/hr.po` (27 lines)
- `addons/sale_sms/i18n/hu.po` (27 lines)
- `addons/sale_sms/i18n/id.po` (27 lines)
- `addons/sale_sms/i18n/it.po` (27 lines)
- `addons/sale_sms/i18n/ja.po` (27 lines)
- `addons/sale_sms/i18n/kab.po` (27 lines)
- `addons/sale_sms/i18n/ko.po` (27 lines)
- `addons/sale_sms/i18n/ku.po` (27 lines)
- `addons/sale_sms/i18n/lo.po` (27 lines)
- `addons/sale_sms/i18n/lt.po` (27 lines)
- `addons/sale_sms/i18n/lv.po` (27 lines)
- `addons/sale_sms/i18n/mn.po` (27 lines)
- `addons/sale_sms/i18n/my.po` (27 lines)
- `addons/sale_sms/i18n/nb.po` (27 lines)
- `addons/sale_sms/i18n/nl.po` (27 lines)
- `addons/sale_sms/i18n/pl.po` (27 lines)
- `addons/sale_sms/i18n/pt.po` (27 lines)
- `addons/sale_sms/i18n/pt_BR.po` (31 lines)
- `addons/sale_sms/i18n/ro.po` (27 lines)
- `addons/sale_sms/i18n/ru.po` (27 lines)
- `addons/sale_sms/i18n/sale_sms.pot` (27 lines)
- `addons/sale_sms/i18n/sk.po` (27 lines)
- `addons/sale_sms/i18n/sl.po` (27 lines)
- `addons/sale_sms/i18n/sr@latin.po` (27 lines)
- `addons/sale_sms/i18n/sv.po` (31 lines)
- `addons/sale_sms/i18n/th.po` (27 lines)
- `addons/sale_sms/i18n/tr.po` (27 lines)
- `addons/sale_sms/i18n/uk.po` (27 lines)
- `addons/sale_sms/i18n/uz.po` (27 lines)
- `addons/sale_sms/i18n/vi.po` (27 lines)
- `addons/sale_sms/i18n/zh_CN.po` (27 lines)
- `addons/sale_sms/i18n/zh_TW.po` (27 lines)
- `addons/sale_sms/security/ir.access.csv` (3 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
