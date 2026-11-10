# Module: website_sms

- **Module ID:** MOD-646
- **Path:** `addons/website_sms`
- **Manifest:** `addons/website_sms/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Allows to send sms to website visitor

Allows to send sms to website visitor if the visitor is linked to a partner.

Declared dependencies: `website`, `sms`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website",
    "sms"
  ],
  "data": [
    "views/website_visitor_views.xml"
  ]
}
```

### Representative source files

- `addons/website_sms/__init__.py` (4 lines)
- `addons/website_sms/__manifest__.py` (15 lines)
- `addons/website_sms/i18n/ar.po` (74 lines)
- `addons/website_sms/i18n/az.po` (72 lines)
- `addons/website_sms/i18n/bg.po` (72 lines)
- `addons/website_sms/i18n/bs.po` (73 lines)
- `addons/website_sms/i18n/ca.po` (75 lines)
- `addons/website_sms/i18n/cs.po` (74 lines)
- `addons/website_sms/i18n/da.po` (75 lines)
- `addons/website_sms/i18n/de.po` (77 lines)
- `addons/website_sms/i18n/el.po` (73 lines)
- `addons/website_sms/i18n/es.po` (77 lines)
- `addons/website_sms/i18n/es_419.po` (75 lines)
- `addons/website_sms/i18n/et.po` (72 lines)
- `addons/website_sms/i18n/fa.po` (72 lines)
- `addons/website_sms/i18n/fi.po` (74 lines)
- `addons/website_sms/i18n/fr.po` (74 lines)
- `addons/website_sms/i18n/he.po` (73 lines)
- `addons/website_sms/i18n/hi.po` (72 lines)
- `addons/website_sms/i18n/hr.po` (73 lines)
- `addons/website_sms/i18n/hu.po` (75 lines)
- `addons/website_sms/i18n/id.po` (74 lines)
- `addons/website_sms/i18n/it.po` (77 lines)
- `addons/website_sms/i18n/ja.po` (75 lines)
- `addons/website_sms/i18n/kab.po` (72 lines)
- `addons/website_sms/i18n/ko.po` (72 lines)
- `addons/website_sms/i18n/ku.po` (72 lines)
- `addons/website_sms/i18n/lo.po` (71 lines)
- `addons/website_sms/i18n/lt.po` (74 lines)
- `addons/website_sms/i18n/lv.po` (72 lines)
- `addons/website_sms/i18n/mn.po` (72 lines)
- `addons/website_sms/i18n/my.po` (72 lines)
- `addons/website_sms/i18n/nb.po` (72 lines)
- `addons/website_sms/i18n/nl.po` (75 lines)
- `addons/website_sms/i18n/pl.po` (75 lines)
- `addons/website_sms/i18n/pt.po` (73 lines)
- `addons/website_sms/i18n/pt_BR.po` (75 lines)
- `addons/website_sms/i18n/ro.po` (75 lines)
- `addons/website_sms/i18n/ru.po` (76 lines)
- `addons/website_sms/i18n/sk.po` (71 lines)
- `addons/website_sms/i18n/sl.po` (73 lines)
- `addons/website_sms/i18n/sr@latin.po` (73 lines)
- `addons/website_sms/i18n/sv.po` (75 lines)
- `addons/website_sms/i18n/th.po` (72 lines)
- `addons/website_sms/i18n/tr.po` (74 lines)
- `addons/website_sms/i18n/uk.po` (75 lines)
- `addons/website_sms/i18n/uz.po` (87 lines)
- `addons/website_sms/i18n/vi.po` (74 lines)
- `addons/website_sms/i18n/website_sms.pot` (68 lines)
- `addons/website_sms/i18n/zh_CN.po` (72 lines)
- `addons/website_sms/i18n/zh_TW.po` (75 lines)
- `addons/website_sms/models/__init__.py` (4 lines)
- `addons/website_sms/models/website_visitor.py` (40 lines)
- `addons/website_sms/views/website_visitor_views.xml` (42 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
