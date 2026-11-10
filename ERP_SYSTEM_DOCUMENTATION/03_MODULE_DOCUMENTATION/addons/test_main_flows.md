# Module: test_main_flows

- **Module ID:** MOD-662
- **Path:** `odoo/addons/test_main_flows`
- **Manifest:** `odoo/addons/test_main_flows/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This module will test the main workflow of Odoo.
It will install some main apps and will try to execute the most important actions.


Declared dependencies: `web_tour`, `crm`, `sale_timesheet`, `purchase_stock`, `mrp`, `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 5 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 1 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 3 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "web_tour",
    "crm",
    "sale_timesheet",
    "purchase_stock",
    "mrp",
    "account"
  ],
  "data": [
    "ir.access.csv"
  ],
  "assets": {
    "web.assets_tests": [
      "test_main_flows/static/tests/tours/*.js"
    ]
  }
}
```

### Representative source files

- `odoo/addons/test_main_flows/__init__.py` (15 lines)
- `odoo/addons/test_main_flows/__manifest__.py` (20 lines)
- `odoo/addons/test_main_flows/ir.access.csv` (2 lines)
- `odoo/addons/test_main_flows/models/model_multicompany.py` (9 lines)
- `odoo/addons/test_main_flows/static/tests/tours/main_flow.js` (1,230 lines)
- `odoo/addons/test_main_flows/static/tests/tours/switch_company_access_error_tour.js` (51 lines)
- `odoo/addons/test_main_flows/static/tests/tours/test_company_access_error_redirect_tour.js` (38 lines)
- `odoo/addons/test_main_flows/tests/__init__.py` (3 lines)
- `odoo/addons/test_main_flows/tests/test_flow.py` (213 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
