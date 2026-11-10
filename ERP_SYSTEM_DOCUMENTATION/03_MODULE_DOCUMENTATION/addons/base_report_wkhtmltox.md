# Module: base_report_wkhtmltox

- **Module ID:** MOD-041
- **Path:** `addons/base_report_wkhtmltox`
- **Manifest:** `addons/base_report_wkhtmltox/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

wkhtmltopdf rendering engine


This module is the implementation of the wkhtmltopdf and
wlhtmltoimage rendering engine for Odoo.

learn more about it here:
https://wkhtmltopdf.org/
    

Declared dependencies: None declared.

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
{}
```

### Representative source files

- `addons/base_report_wkhtmltox/__init__.py` (7 lines)
- `addons/base_report_wkhtmltox/__manifest__.py` (18 lines)
- `addons/base_report_wkhtmltox/i18n/ar.po` (108 lines)
- `addons/base_report_wkhtmltox/i18n/az.po` (107 lines)
- `addons/base_report_wkhtmltox/i18n/base_report_wkhtmltox.pot` (104 lines)
- `addons/base_report_wkhtmltox/i18n/bg.po` (107 lines)
- `addons/base_report_wkhtmltox/i18n/bs.po` (108 lines)
- `addons/base_report_wkhtmltox/i18n/ca.po` (107 lines)
- `addons/base_report_wkhtmltox/i18n/cs.po` (107 lines)
- `addons/base_report_wkhtmltox/i18n/da.po` (119 lines)
- `addons/base_report_wkhtmltox/i18n/de.po` (128 lines)
- `addons/base_report_wkhtmltox/i18n/el.po` (107 lines)
- `addons/base_report_wkhtmltox/i18n/es.po` (108 lines)
- `addons/base_report_wkhtmltox/i18n/es_419.po` (126 lines)
- `addons/base_report_wkhtmltox/i18n/et.po` (107 lines)
- `addons/base_report_wkhtmltox/i18n/fa.po` (107 lines)
- `addons/base_report_wkhtmltox/i18n/fi.po` (114 lines)
- `addons/base_report_wkhtmltox/i18n/fr.po` (126 lines)
- `addons/base_report_wkhtmltox/i18n/he.po` (108 lines)
- `addons/base_report_wkhtmltox/i18n/hi.po` (107 lines)
- `addons/base_report_wkhtmltox/i18n/hr.po` (108 lines)
- `addons/base_report_wkhtmltox/i18n/hu.po` (107 lines)
- `addons/base_report_wkhtmltox/i18n/id.po` (107 lines)
- `addons/base_report_wkhtmltox/i18n/it.po` (124 lines)
- `addons/base_report_wkhtmltox/i18n/ja.po` (124 lines)
- `addons/base_report_wkhtmltox/i18n/kab.po` (107 lines)
- `addons/base_report_wkhtmltox/i18n/ko.po` (107 lines)
- `addons/base_report_wkhtmltox/i18n/ku.po` (107 lines)
- `addons/base_report_wkhtmltox/i18n/lo.po` (107 lines)
- `addons/base_report_wkhtmltox/i18n/lt.po` (109 lines)
- `addons/base_report_wkhtmltox/i18n/lv.po` (108 lines)
- `addons/base_report_wkhtmltox/i18n/mn.po` (107 lines)
- `addons/base_report_wkhtmltox/i18n/my.po` (107 lines)
- `addons/base_report_wkhtmltox/i18n/nb.po` (107 lines)
- `addons/base_report_wkhtmltox/i18n/nl.po` (118 lines)
- `addons/base_report_wkhtmltox/i18n/pl.po` (108 lines)
- `addons/base_report_wkhtmltox/i18n/pt.po` (107 lines)
- `addons/base_report_wkhtmltox/i18n/pt_BR.po` (124 lines)
- `addons/base_report_wkhtmltox/i18n/ro.po` (108 lines)
- `addons/base_report_wkhtmltox/i18n/ru.po` (108 lines)
- `addons/base_report_wkhtmltox/i18n/sk.po` (107 lines)
- `addons/base_report_wkhtmltox/i18n/sl.po` (108 lines)
- `addons/base_report_wkhtmltox/i18n/sr@latin.po` (108 lines)
- `addons/base_report_wkhtmltox/i18n/sv.po` (108 lines)
- `addons/base_report_wkhtmltox/i18n/th.po` (107 lines)
- `addons/base_report_wkhtmltox/i18n/tr.po` (118 lines)
- `addons/base_report_wkhtmltox/i18n/uk.po` (108 lines)
- `addons/base_report_wkhtmltox/i18n/uz.po` (107 lines)
- `addons/base_report_wkhtmltox/i18n/vi.po` (107 lines)
- `addons/base_report_wkhtmltox/i18n/zh_CN.po` (119 lines)
- `addons/base_report_wkhtmltox/i18n/zh_TW.po` (108 lines)
- `addons/base_report_wkhtmltox/models/__init__.py` (3 lines)
- `addons/base_report_wkhtmltox/models/ir_actions_report.py` (509 lines)
- `addons/base_report_wkhtmltox/tests/__init__.py` (3 lines)
- `addons/base_report_wkhtmltox/tests/test_split_table.py` (38 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
