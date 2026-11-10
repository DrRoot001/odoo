# Module: l10n_in_hr_holidays

- **Module ID:** MOD-233
- **Path:** `addons/l10n_in_hr_holidays`
- **Manifest:** `addons/l10n_in_hr_holidays/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['hr_holidays']`
- **License:** `LGPL-3`

## Purpose and dependencies

Leave Management of Indian Localization

The Indian Time Off module provides additional features to the application. With it, you'll be able to define Sandwich Leaves on your time type, including weekends or holidays in the duration of the employee leave's request.

Declared dependencies: `hr_holidays`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "hr_holidays"
  ],
  "data": [
    "views/hr_leave_views.xml",
    "views/hr_work_entry_type_views.xml",
    "views/l10n_in_hr_leave_optional_holiday_views.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "l10n_in_hr_holidays/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_in_hr_holidays/__init__.py` (3 lines)
- `addons/l10n_in_hr_holidays/__manifest__.py` (24 lines)
- `addons/l10n_in_hr_holidays/i18n/hi.po` (220 lines)
- `addons/l10n_in_hr_holidays/i18n/l10n_in_hr_holidays.pot` (209 lines)
- `addons/l10n_in_hr_holidays/models/__init__.py` (6 lines)
- `addons/l10n_in_hr_holidays/models/hr_employee.py` (28 lines)
- `addons/l10n_in_hr_holidays/models/hr_leave.py` (352 lines)
- `addons/l10n_in_hr_holidays/models/hr_work_entry_type.py` (29 lines)
- `addons/l10n_in_hr_holidays/models/l10n_in_hr_leave_optional_holiday.py` (43 lines)
- `addons/l10n_in_hr_holidays/security/ir.access.csv` (4 lines)
- `addons/l10n_in_hr_holidays/static/src/views/calendar/side_panel/calendar_side_panel.js` (14 lines)
- `addons/l10n_in_hr_holidays/static/src/views/calendar/side_panel/calendar_side_panel.xml` (18 lines)
- `addons/l10n_in_hr_holidays/tests/__init__.py` (4 lines)
- `addons/l10n_in_hr_holidays/tests/test_optional_holiday.py` (44 lines)
- `addons/l10n_in_hr_holidays/tests/test_sandwich_leave.py` (800 lines)
- `addons/l10n_in_hr_holidays/views/hr_leave_views.xml` (17 lines)
- `addons/l10n_in_hr_holidays/views/hr_work_entry_type_views.xml` (18 lines)
- `addons/l10n_in_hr_holidays/views/l10n_in_hr_leave_optional_holiday_views.xml` (45 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
