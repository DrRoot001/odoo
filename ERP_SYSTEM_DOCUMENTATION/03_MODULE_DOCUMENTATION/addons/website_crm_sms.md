# Module: website_crm_sms

- **Module ID:** MOD-604
- **Path:** `addons/website_crm_sms`
- **Manifest:** `addons/website_crm_sms/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Allows to send sms to website visitor that have lead

Allows to send sms to website visitor if the visitor is linked to a lead.

Declared dependencies: `website_sms`, `crm`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website_sms",
    "crm"
  ]
}
```

### Representative source files

- `addons/website_crm_sms/__init__.py` (4 lines)
- `addons/website_crm_sms/__manifest__.py` (12 lines)
- `addons/website_crm_sms/i18n/ar.po` (52 lines)
- `addons/website_crm_sms/i18n/az.po` (50 lines)
- `addons/website_crm_sms/i18n/bg.po` (50 lines)
- `addons/website_crm_sms/i18n/bs.po` (52 lines)
- `addons/website_crm_sms/i18n/ca.po` (52 lines)
- `addons/website_crm_sms/i18n/cs.po` (51 lines)
- `addons/website_crm_sms/i18n/da.po` (52 lines)
- `addons/website_crm_sms/i18n/de.po` (54 lines)
- `addons/website_crm_sms/i18n/el.po` (50 lines)
- `addons/website_crm_sms/i18n/es.po` (55 lines)
- `addons/website_crm_sms/i18n/es_419.po` (51 lines)
- `addons/website_crm_sms/i18n/et.po` (50 lines)
- `addons/website_crm_sms/i18n/fa.po` (50 lines)
- `addons/website_crm_sms/i18n/fi.po` (51 lines)
- `addons/website_crm_sms/i18n/fr.po` (51 lines)
- `addons/website_crm_sms/i18n/he.po` (51 lines)
- `addons/website_crm_sms/i18n/hi.po` (50 lines)
- `addons/website_crm_sms/i18n/hr.po` (51 lines)
- `addons/website_crm_sms/i18n/hu.po` (51 lines)
- `addons/website_crm_sms/i18n/id.po` (51 lines)
- `addons/website_crm_sms/i18n/it.po` (51 lines)
- `addons/website_crm_sms/i18n/ja.po` (51 lines)
- `addons/website_crm_sms/i18n/kab.po` (51 lines)
- `addons/website_crm_sms/i18n/ko.po` (51 lines)
- `addons/website_crm_sms/i18n/ku.po` (50 lines)
- `addons/website_crm_sms/i18n/lo.po` (50 lines)
- `addons/website_crm_sms/i18n/lt.po` (52 lines)
- `addons/website_crm_sms/i18n/lv.po` (51 lines)
- `addons/website_crm_sms/i18n/mn.po` (50 lines)
- `addons/website_crm_sms/i18n/my.po` (50 lines)
- `addons/website_crm_sms/i18n/nb.po` (51 lines)
- `addons/website_crm_sms/i18n/nl.po` (51 lines)
- `addons/website_crm_sms/i18n/pl.po` (53 lines)
- `addons/website_crm_sms/i18n/pt.po` (52 lines)
- `addons/website_crm_sms/i18n/pt_BR.po` (54 lines)
- `addons/website_crm_sms/i18n/ro.po` (52 lines)
- `addons/website_crm_sms/i18n/ru.po` (54 lines)
- `addons/website_crm_sms/i18n/sk.po` (50 lines)
- `addons/website_crm_sms/i18n/sl.po` (52 lines)
- `addons/website_crm_sms/i18n/sr@latin.po` (51 lines)
- `addons/website_crm_sms/i18n/sv.po` (52 lines)
- `addons/website_crm_sms/i18n/th.po` (51 lines)
- `addons/website_crm_sms/i18n/tr.po` (52 lines)
- `addons/website_crm_sms/i18n/uk.po` (51 lines)
- `addons/website_crm_sms/i18n/uz.po` (61 lines)
- `addons/website_crm_sms/i18n/vi.po` (51 lines)
- `addons/website_crm_sms/i18n/website_crm_sms.pot` (47 lines)
- `addons/website_crm_sms/i18n/zh_CN.po` (51 lines)
- `addons/website_crm_sms/i18n/zh_TW.po` (53 lines)
- `addons/website_crm_sms/models/__init__.py` (4 lines)
- `addons/website_crm_sms/models/website_visitor.py` (28 lines)
- `addons/website_crm_sms/tests/__init__.py` (1 lines)
- `addons/website_crm_sms/tests/test_website_visitor.py` (46 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
