# Module: website_timesheet

- **Module ID:** MOD-647
- **Path:** `addons/website_timesheet`
- **Manifest:** `addons/website_timesheet/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Allow hiding timesheet information in the portal


When hiding the timesheets in the portal, this module allows also hiding timesheet information on other records.
    

Declared dependencies: `website`, `hr_timesheet`.

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
    "website",
    "hr_timesheet"
  ]
}
```

### Representative source files

- `addons/website_timesheet/__init__.py` (1 lines)
- `addons/website_timesheet/__manifest__.py` (12 lines)
- `addons/website_timesheet/i18n/ar.po` (55 lines)
- `addons/website_timesheet/i18n/az.po` (53 lines)
- `addons/website_timesheet/i18n/bg.po` (53 lines)
- `addons/website_timesheet/i18n/bs.po` (54 lines)
- `addons/website_timesheet/i18n/ca.po` (54 lines)
- `addons/website_timesheet/i18n/cs.po` (53 lines)
- `addons/website_timesheet/i18n/da.po` (54 lines)
- `addons/website_timesheet/i18n/de.po` (57 lines)
- `addons/website_timesheet/i18n/el.po` (53 lines)
- `addons/website_timesheet/i18n/es.po` (57 lines)
- `addons/website_timesheet/i18n/es_419.po` (57 lines)
- `addons/website_timesheet/i18n/et.po` (53 lines)
- `addons/website_timesheet/i18n/fa.po` (53 lines)
- `addons/website_timesheet/i18n/fi.po` (54 lines)
- `addons/website_timesheet/i18n/fr.po` (53 lines)
- `addons/website_timesheet/i18n/he.po` (54 lines)
- `addons/website_timesheet/i18n/hi.po` (53 lines)
- `addons/website_timesheet/i18n/hr.po` (54 lines)
- `addons/website_timesheet/i18n/hu.po` (53 lines)
- `addons/website_timesheet/i18n/id.po` (53 lines)
- `addons/website_timesheet/i18n/it.po` (56 lines)
- `addons/website_timesheet/i18n/ja.po` (53 lines)
- `addons/website_timesheet/i18n/kab.po` (53 lines)
- `addons/website_timesheet/i18n/ko.po` (53 lines)
- `addons/website_timesheet/i18n/ku.po` (53 lines)
- `addons/website_timesheet/i18n/lo.po` (52 lines)
- `addons/website_timesheet/i18n/lt.po` (55 lines)
- `addons/website_timesheet/i18n/lv.po` (53 lines)
- `addons/website_timesheet/i18n/mn.po` (53 lines)
- `addons/website_timesheet/i18n/my.po` (53 lines)
- `addons/website_timesheet/i18n/nb.po` (53 lines)
- `addons/website_timesheet/i18n/nl.po` (55 lines)
- `addons/website_timesheet/i18n/pl.po` (54 lines)
- `addons/website_timesheet/i18n/pt.po` (53 lines)
- `addons/website_timesheet/i18n/pt_BR.po` (60 lines)
- `addons/website_timesheet/i18n/ro.po` (54 lines)
- `addons/website_timesheet/i18n/ru.po` (54 lines)
- `addons/website_timesheet/i18n/sk.po` (52 lines)
- `addons/website_timesheet/i18n/sl.po` (54 lines)
- `addons/website_timesheet/i18n/sr@latin.po` (54 lines)
- `addons/website_timesheet/i18n/sv.po` (55 lines)
- `addons/website_timesheet/i18n/th.po` (53 lines)
- `addons/website_timesheet/i18n/tr.po` (53 lines)
- `addons/website_timesheet/i18n/uk.po` (54 lines)
- `addons/website_timesheet/i18n/uz.po` (63 lines)
- `addons/website_timesheet/i18n/vi.po` (54 lines)
- `addons/website_timesheet/i18n/website_timesheet.pot` (48 lines)
- `addons/website_timesheet/i18n/zh_CN.po` (53 lines)
- `addons/website_timesheet/i18n/zh_TW.po` (54 lines)
- `addons/website_timesheet/models/__init__.py` (1 lines)
- `addons/website_timesheet/models/account_analytic_line.py` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
