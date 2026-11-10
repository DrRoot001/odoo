# Module: iap_crm

- **Module ID:** MOD-109
- **Path:** `addons/iap_crm`
- **Manifest:** `addons/iap_crm/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Bridge between IAP and CRM

Bridge between IAP and CRM

Declared dependencies: `crm`, `iap_mail`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "crm",
    "iap_mail"
  ]
}
```

### Representative source files

- `addons/iap_crm/__init__.py` (4 lines)
- `addons/iap_crm/__manifest__.py` (16 lines)
- `addons/iap_crm/i18n/ar.po` (58 lines)
- `addons/iap_crm/i18n/az.po` (55 lines)
- `addons/iap_crm/i18n/bg.po` (55 lines)
- `addons/iap_crm/i18n/bs.po` (57 lines)
- `addons/iap_crm/i18n/ca.po` (56 lines)
- `addons/iap_crm/i18n/cs.po` (56 lines)
- `addons/iap_crm/i18n/da.po` (55 lines)
- `addons/iap_crm/i18n/de.po` (57 lines)
- `addons/iap_crm/i18n/el.po` (56 lines)
- `addons/iap_crm/i18n/es.po` (58 lines)
- `addons/iap_crm/i18n/es_419.po` (58 lines)
- `addons/iap_crm/i18n/et.po` (55 lines)
- `addons/iap_crm/i18n/fa.po` (55 lines)
- `addons/iap_crm/i18n/fi.po` (57 lines)
- `addons/iap_crm/i18n/fr.po` (57 lines)
- `addons/iap_crm/i18n/he.po` (56 lines)
- `addons/iap_crm/i18n/hi.po` (55 lines)
- `addons/iap_crm/i18n/hr.po` (56 lines)
- `addons/iap_crm/i18n/hu.po` (56 lines)
- `addons/iap_crm/i18n/iap_crm.pot` (52 lines)
- `addons/iap_crm/i18n/id.po` (57 lines)
- `addons/iap_crm/i18n/it.po` (57 lines)
- `addons/iap_crm/i18n/ja.po` (57 lines)
- `addons/iap_crm/i18n/kab.po` (56 lines)
- `addons/iap_crm/i18n/ko.po` (57 lines)
- `addons/iap_crm/i18n/ku.po` (55 lines)
- `addons/iap_crm/i18n/lo.po` (55 lines)
- `addons/iap_crm/i18n/lt.po` (57 lines)
- `addons/iap_crm/i18n/lv.po` (56 lines)
- `addons/iap_crm/i18n/mn.po` (55 lines)
- `addons/iap_crm/i18n/my.po` (55 lines)
- `addons/iap_crm/i18n/nb.po` (55 lines)
- `addons/iap_crm/i18n/nl.po` (57 lines)
- `addons/iap_crm/i18n/pl.po` (58 lines)
- `addons/iap_crm/i18n/pt.po` (56 lines)
- `addons/iap_crm/i18n/pt_BR.po` (58 lines)
- `addons/iap_crm/i18n/ro.po` (57 lines)
- `addons/iap_crm/i18n/ru.po` (59 lines)
- `addons/iap_crm/i18n/sk.po` (55 lines)
- `addons/iap_crm/i18n/sl.po` (57 lines)
- `addons/iap_crm/i18n/sr@latin.po` (56 lines)
- `addons/iap_crm/i18n/sv.po` (57 lines)
- `addons/iap_crm/i18n/th.po` (57 lines)
- `addons/iap_crm/i18n/tr.po` (56 lines)
- `addons/iap_crm/i18n/uk.po` (56 lines)
- `addons/iap_crm/i18n/uz.po` (68 lines)
- `addons/iap_crm/i18n/vi.po` (57 lines)
- `addons/iap_crm/i18n/zh_CN.po` (57 lines)
- `addons/iap_crm/i18n/zh_TW.po` (59 lines)
- `addons/iap_crm/models/__init__.py` (4 lines)
- `addons/iap_crm/models/crm_lead.py` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
