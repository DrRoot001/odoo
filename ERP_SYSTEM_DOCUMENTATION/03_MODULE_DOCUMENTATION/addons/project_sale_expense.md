# Module: project_sale_expense

- **Module ID:** MOD-486
- **Path:** `addons/project_sale_expense`
- **Manifest:** `addons/project_sale_expense/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Adds a full traceability of reinvoice expenses on the profitability report.

Declared dependencies: `sale_project`, `sale_expense`, `project_hr_expense`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
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
    "sale_project",
    "sale_expense",
    "project_hr_expense"
  ]
}
```

### Representative source files

- `addons/project_sale_expense/__init__.py` (4 lines)
- `addons/project_sale_expense/__manifest__.py` (11 lines)
- `addons/project_sale_expense/i18n/ar.po` (81 lines)
- `addons/project_sale_expense/i18n/az.po` (77 lines)
- `addons/project_sale_expense/i18n/bg.po` (77 lines)
- `addons/project_sale_expense/i18n/bs.po` (79 lines)
- `addons/project_sale_expense/i18n/ca.po` (78 lines)
- `addons/project_sale_expense/i18n/cs.po` (79 lines)
- `addons/project_sale_expense/i18n/da.po` (79 lines)
- `addons/project_sale_expense/i18n/de.po` (87 lines)
- `addons/project_sale_expense/i18n/el.po` (78 lines)
- `addons/project_sale_expense/i18n/es.po` (82 lines)
- `addons/project_sale_expense/i18n/es_419.po` (86 lines)
- `addons/project_sale_expense/i18n/et.po` (78 lines)
- `addons/project_sale_expense/i18n/fa.po` (77 lines)
- `addons/project_sale_expense/i18n/fi.po` (79 lines)
- `addons/project_sale_expense/i18n/fr.po` (85 lines)
- `addons/project_sale_expense/i18n/he.po` (78 lines)
- `addons/project_sale_expense/i18n/hi.po` (77 lines)
- `addons/project_sale_expense/i18n/hr.po` (78 lines)
- `addons/project_sale_expense/i18n/hu.po` (78 lines)
- `addons/project_sale_expense/i18n/id.po` (80 lines)
- `addons/project_sale_expense/i18n/it.po` (85 lines)
- `addons/project_sale_expense/i18n/ja.po` (85 lines)
- `addons/project_sale_expense/i18n/kab.po` (78 lines)
- `addons/project_sale_expense/i18n/ko.po` (79 lines)
- `addons/project_sale_expense/i18n/ku.po` (77 lines)
- `addons/project_sale_expense/i18n/lo.po` (77 lines)
- `addons/project_sale_expense/i18n/lt.po` (79 lines)
- `addons/project_sale_expense/i18n/lv.po` (78 lines)
- `addons/project_sale_expense/i18n/mn.po` (77 lines)
- `addons/project_sale_expense/i18n/my.po` (77 lines)
- `addons/project_sale_expense/i18n/nb.po` (78 lines)
- `addons/project_sale_expense/i18n/nl.po` (85 lines)
- `addons/project_sale_expense/i18n/pl.po` (80 lines)
- `addons/project_sale_expense/i18n/project_sale_expense.pot` (74 lines)
- `addons/project_sale_expense/i18n/pt.po` (78 lines)
- `addons/project_sale_expense/i18n/pt_BR.po` (89 lines)
- `addons/project_sale_expense/i18n/ro.po` (79 lines)
- `addons/project_sale_expense/i18n/ru.po` (82 lines)
- `addons/project_sale_expense/i18n/sk.po` (77 lines)
- `addons/project_sale_expense/i18n/sl.po` (79 lines)
- `addons/project_sale_expense/i18n/sr@latin.po` (78 lines)
- `addons/project_sale_expense/i18n/sv.po` (79 lines)
- `addons/project_sale_expense/i18n/th.po` (82 lines)
- `addons/project_sale_expense/i18n/tr.po` (80 lines)
- `addons/project_sale_expense/i18n/uk.po` (78 lines)
- `addons/project_sale_expense/i18n/uz.po` (89 lines)
- `addons/project_sale_expense/i18n/vi.po` (79 lines)
- `addons/project_sale_expense/i18n/zh_CN.po` (86 lines)
- `addons/project_sale_expense/i18n/zh_TW.po` (82 lines)
- `addons/project_sale_expense/models/__init__.py` (5 lines)
- `addons/project_sale_expense/models/account_analytic_line.py` (35 lines)
- `addons/project_sale_expense/models/account_move_line.py` (23 lines)
- `addons/project_sale_expense/models/hr_expense.py` (50 lines)
- `addons/project_sale_expense/tests/__init__.py` (5 lines)
- `addons/project_sale_expense/tests/test_expense_analytics.py` (53 lines)
- `addons/project_sale_expense/tests/test_project_sale_expense.py` (254 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
