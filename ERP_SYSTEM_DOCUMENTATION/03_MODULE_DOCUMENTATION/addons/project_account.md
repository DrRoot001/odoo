# Module: project_account

- **Module ID:** MOD-476
- **Path:** `addons/project_account`
- **Manifest:** `addons/project_account/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

project profitability items computation


Allows the computation of some section for the project profitability
==================================================================================================
This module allows the computation of the 'Vendor Bills', 'Other Costs' and 'Other Revenue' section for the project profitability, in the project update view.


Declared dependencies: `account`, `project`.

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
    "account",
    "project"
  ],
  "data": [
    "views/project_project_views.xml",
    "views/project_task_views.xml",
    "views/project_sharing_project_task_views.xml"
  ]
}
```

### Representative source files

- `addons/project_account/__init__.py` (4 lines)
- `addons/project_account/__manifest__.py` (20 lines)
- `addons/project_account/i18n/ar.po` (70 lines)
- `addons/project_account/i18n/az.po` (61 lines)
- `addons/project_account/i18n/bg.po` (61 lines)
- `addons/project_account/i18n/bs.po` (63 lines)
- `addons/project_account/i18n/ca.po` (62 lines)
- `addons/project_account/i18n/cs.po` (63 lines)
- `addons/project_account/i18n/da.po` (62 lines)
- `addons/project_account/i18n/de.po` (69 lines)
- `addons/project_account/i18n/el.po` (62 lines)
- `addons/project_account/i18n/es.po` (64 lines)
- `addons/project_account/i18n/es_419.po` (64 lines)
- `addons/project_account/i18n/et.po` (62 lines)
- `addons/project_account/i18n/fa.po` (61 lines)
- `addons/project_account/i18n/fi.po` (63 lines)
- `addons/project_account/i18n/fr.po` (63 lines)
- `addons/project_account/i18n/he.po` (62 lines)
- `addons/project_account/i18n/hi.po` (61 lines)
- `addons/project_account/i18n/hr.po` (62 lines)
- `addons/project_account/i18n/hu.po` (62 lines)
- `addons/project_account/i18n/id.po` (63 lines)
- `addons/project_account/i18n/it.po` (70 lines)
- `addons/project_account/i18n/ja.po` (63 lines)
- `addons/project_account/i18n/kab.po` (62 lines)
- `addons/project_account/i18n/ko.po` (63 lines)
- `addons/project_account/i18n/ku.po` (61 lines)
- `addons/project_account/i18n/lo.po` (61 lines)
- `addons/project_account/i18n/lt.po` (63 lines)
- `addons/project_account/i18n/lv.po` (62 lines)
- `addons/project_account/i18n/mn.po` (61 lines)
- `addons/project_account/i18n/my.po` (62 lines)
- `addons/project_account/i18n/nb.po` (62 lines)
- `addons/project_account/i18n/nl.po` (63 lines)
- `addons/project_account/i18n/pl.po` (64 lines)
- `addons/project_account/i18n/project_account.pot` (56 lines)
- `addons/project_account/i18n/pt.po` (62 lines)
- `addons/project_account/i18n/pt_BR.po` (71 lines)
- `addons/project_account/i18n/ro.po` (63 lines)
- `addons/project_account/i18n/ru.po` (66 lines)
- `addons/project_account/i18n/sk.po` (61 lines)
- `addons/project_account/i18n/sl.po` (63 lines)
- `addons/project_account/i18n/sr@latin.po` (62 lines)
- `addons/project_account/i18n/sv.po` (63 lines)
- `addons/project_account/i18n/th.po` (63 lines)
- `addons/project_account/i18n/tr.po` (71 lines)
- `addons/project_account/i18n/uk.po` (62 lines)
- `addons/project_account/i18n/uz.po` (73 lines)
- `addons/project_account/i18n/vi.po` (63 lines)
- `addons/project_account/i18n/zh_CN.po` (68 lines)
- `addons/project_account/i18n/zh_TW.po` (65 lines)
- `addons/project_account/models/__init__.py` (3 lines)
- `addons/project_account/models/project_project.py` (18 lines)
- `addons/project_account/views/project_project_views.xml` (47 lines)
- `addons/project_account/views/project_sharing_project_task_views.xml` (21 lines)
- `addons/project_account/views/project_task_views.xml` (32 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
