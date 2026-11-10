# Module: project_hr_expense

- **Module ID:** MOD-477
- **Path:** `addons/project_hr_expense`
- **Manifest:** `addons/project_hr_expense/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Project expenses

Bridge created to add the number of expenses linked to an AA to a project form

Declared dependencies: `project_account`, `hr_expense`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "project_account",
    "hr_expense"
  ],
  "data": [
    "views/project_project_views.xml"
  ],
  "demo": [
    "data/project_hr_expense_demo.xml"
  ]
}
```

### Representative source files

- `addons/project_hr_expense/__init__.py` (4 lines)
- `addons/project_hr_expense/__manifest__.py` (19 lines)
- `addons/project_hr_expense/data/project_hr_expense_demo.xml` (37 lines)
- `addons/project_hr_expense/i18n/ar.po` (69 lines)
- `addons/project_hr_expense/i18n/az.po` (66 lines)
- `addons/project_hr_expense/i18n/bg.po` (66 lines)
- `addons/project_hr_expense/i18n/bs.po` (68 lines)
- `addons/project_hr_expense/i18n/ca.po` (67 lines)
- `addons/project_hr_expense/i18n/cs.po` (68 lines)
- `addons/project_hr_expense/i18n/da.po` (68 lines)
- `addons/project_hr_expense/i18n/de.po` (70 lines)
- `addons/project_hr_expense/i18n/el.po` (67 lines)
- `addons/project_hr_expense/i18n/es.po` (71 lines)
- `addons/project_hr_expense/i18n/es_419.po` (69 lines)
- `addons/project_hr_expense/i18n/et.po` (67 lines)
- `addons/project_hr_expense/i18n/fa.po` (66 lines)
- `addons/project_hr_expense/i18n/fi.po` (68 lines)
- `addons/project_hr_expense/i18n/fr.po` (68 lines)
- `addons/project_hr_expense/i18n/he.po` (67 lines)
- `addons/project_hr_expense/i18n/hi.po` (66 lines)
- `addons/project_hr_expense/i18n/hr.po` (67 lines)
- `addons/project_hr_expense/i18n/hu.po` (67 lines)
- `addons/project_hr_expense/i18n/id.po` (68 lines)
- `addons/project_hr_expense/i18n/it.po` (68 lines)
- `addons/project_hr_expense/i18n/ja.po` (68 lines)
- `addons/project_hr_expense/i18n/kab.po` (67 lines)
- `addons/project_hr_expense/i18n/ko.po` (68 lines)
- `addons/project_hr_expense/i18n/ku.po` (66 lines)
- `addons/project_hr_expense/i18n/lo.po` (66 lines)
- `addons/project_hr_expense/i18n/lt.po` (68 lines)
- `addons/project_hr_expense/i18n/lv.po` (67 lines)
- `addons/project_hr_expense/i18n/mn.po` (66 lines)
- `addons/project_hr_expense/i18n/my.po` (67 lines)
- `addons/project_hr_expense/i18n/nb.po` (67 lines)
- `addons/project_hr_expense/i18n/nl.po` (68 lines)
- `addons/project_hr_expense/i18n/pl.po` (69 lines)
- `addons/project_hr_expense/i18n/project_hr_expense.pot` (63 lines)
- `addons/project_hr_expense/i18n/pt.po` (67 lines)
- `addons/project_hr_expense/i18n/pt_BR.po` (74 lines)
- `addons/project_hr_expense/i18n/ro.po` (68 lines)
- `addons/project_hr_expense/i18n/ru.po` (71 lines)
- `addons/project_hr_expense/i18n/sk.po` (66 lines)
- `addons/project_hr_expense/i18n/sl.po` (68 lines)
- `addons/project_hr_expense/i18n/sr@latin.po` (67 lines)
- `addons/project_hr_expense/i18n/sv.po` (68 lines)
- `addons/project_hr_expense/i18n/th.po` (68 lines)
- `addons/project_hr_expense/i18n/tr.po` (68 lines)
- `addons/project_hr_expense/i18n/uk.po` (67 lines)
- `addons/project_hr_expense/i18n/uz.po` (79 lines)
- `addons/project_hr_expense/i18n/vi.po` (68 lines)
- `addons/project_hr_expense/i18n/zh_CN.po` (68 lines)
- `addons/project_hr_expense/i18n/zh_TW.po` (71 lines)
- `addons/project_hr_expense/models/__init__.py` (2 lines)
- `addons/project_hr_expense/models/hr_expense.py` (27 lines)
- `addons/project_hr_expense/models/project_project.py` (28 lines)
- `addons/project_hr_expense/tests/__init__.py` (3 lines)
- `addons/project_hr_expense/tests/test_analytics.py` (50 lines)
- `addons/project_hr_expense/views/project_project_views.xml` (22 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
