# Module: sale_project_margin

- **Module ID:** MOD-525
- **Path:** `addons/sale_project_margin`
- **Manifest:** `addons/sale_project_margin/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Bridge module between Sales Margin and Project


Allows to compute accurate margin for Service sales.
======================================================


Declared dependencies: `sale_margin`, `sale_project`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sale_margin",
    "sale_project"
  ],
  "data": [
    "views/project_task_views.xml",
    "views/project_menus.xml",
    "report/sale_report_views.xml"
  ]
}
```

### Representative source files

- `addons/sale_project_margin/__init__.py` (1 lines)
- `addons/sale_project_margin/__manifest__.py` (18 lines)
- `addons/sale_project_margin/i18n/ar.po` (87 lines)
- `addons/sale_project_margin/i18n/az.po` (86 lines)
- `addons/sale_project_margin/i18n/bg.po` (86 lines)
- `addons/sale_project_margin/i18n/bs.po` (87 lines)
- `addons/sale_project_margin/i18n/ca.po` (86 lines)
- `addons/sale_project_margin/i18n/cs.po` (86 lines)
- `addons/sale_project_margin/i18n/da.po` (86 lines)
- `addons/sale_project_margin/i18n/de.po` (92 lines)
- `addons/sale_project_margin/i18n/el.po` (86 lines)
- `addons/sale_project_margin/i18n/es.po` (90 lines)
- `addons/sale_project_margin/i18n/es_419.po` (94 lines)
- `addons/sale_project_margin/i18n/et.po` (86 lines)
- `addons/sale_project_margin/i18n/fa.po` (86 lines)
- `addons/sale_project_margin/i18n/fi.po` (90 lines)
- `addons/sale_project_margin/i18n/fr.po` (88 lines)
- `addons/sale_project_margin/i18n/he.po` (87 lines)
- `addons/sale_project_margin/i18n/hi.po` (86 lines)
- `addons/sale_project_margin/i18n/hr.po` (87 lines)
- `addons/sale_project_margin/i18n/hu.po` (86 lines)
- `addons/sale_project_margin/i18n/id.po` (87 lines)
- `addons/sale_project_margin/i18n/it.po` (87 lines)
- `addons/sale_project_margin/i18n/ja.po` (93 lines)
- `addons/sale_project_margin/i18n/kab.po` (86 lines)
- `addons/sale_project_margin/i18n/ko.po` (87 lines)
- `addons/sale_project_margin/i18n/ku.po` (86 lines)
- `addons/sale_project_margin/i18n/lo.po` (86 lines)
- `addons/sale_project_margin/i18n/lt.po` (88 lines)
- `addons/sale_project_margin/i18n/lv.po` (87 lines)
- `addons/sale_project_margin/i18n/mn.po` (86 lines)
- `addons/sale_project_margin/i18n/my.po` (87 lines)
- `addons/sale_project_margin/i18n/nb.po` (86 lines)
- `addons/sale_project_margin/i18n/nl.po` (91 lines)
- `addons/sale_project_margin/i18n/pl.po` (87 lines)
- `addons/sale_project_margin/i18n/pt.po` (86 lines)
- `addons/sale_project_margin/i18n/pt_BR.po` (104 lines)
- `addons/sale_project_margin/i18n/ro.po` (87 lines)
- `addons/sale_project_margin/i18n/ru.po` (87 lines)
- `addons/sale_project_margin/i18n/sale_project_margin.pot` (83 lines)
- `addons/sale_project_margin/i18n/sk.po` (86 lines)
- `addons/sale_project_margin/i18n/sl.po` (87 lines)
- `addons/sale_project_margin/i18n/sr@latin.po` (87 lines)
- `addons/sale_project_margin/i18n/sv.po` (87 lines)
- `addons/sale_project_margin/i18n/th.po` (87 lines)
- `addons/sale_project_margin/i18n/tr.po` (86 lines)
- `addons/sale_project_margin/i18n/uk.po` (87 lines)
- `addons/sale_project_margin/i18n/uz.po` (86 lines)
- `addons/sale_project_margin/i18n/vi.po` (86 lines)
- `addons/sale_project_margin/i18n/zh_CN.po` (94 lines)
- `addons/sale_project_margin/i18n/zh_TW.po` (87 lines)
- `addons/sale_project_margin/models/__init__.py` (1 lines)
- `addons/sale_project_margin/models/project_project.py` (28 lines)
- `addons/sale_project_margin/report/sale_report_views.xml` (68 lines)
- `addons/sale_project_margin/views/project_menus.xml` (11 lines)
- `addons/sale_project_margin/views/project_task_views.xml` (34 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
