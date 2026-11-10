# Module: project_sms

- **Module ID:** MOD-487
- **Path:** `addons/project_sms`
- **Manifest:** `addons/project_sms/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Send text messages when project/task stage move

Send text messages when project/task stage move

Declared dependencies: `project`, `sms`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "project",
    "sms"
  ],
  "data": [
    "views/project_stage_views.xml",
    "views/project_task_type_views.xml",
    "views/project_project_views.xml",
    "views/project_task_views.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/project_sms/__init__.py` (4 lines)
- `addons/project_sms/__manifest__.py` (20 lines)
- `addons/project_sms/i18n/ar.po` (138 lines)
- `addons/project_sms/i18n/az.po` (119 lines)
- `addons/project_sms/i18n/bg.po` (119 lines)
- `addons/project_sms/i18n/bs.po` (121 lines)
- `addons/project_sms/i18n/ca.po` (124 lines)
- `addons/project_sms/i18n/cs.po` (121 lines)
- `addons/project_sms/i18n/da.po` (121 lines)
- `addons/project_sms/i18n/de.po` (138 lines)
- `addons/project_sms/i18n/el.po` (120 lines)
- `addons/project_sms/i18n/es.po` (137 lines)
- `addons/project_sms/i18n/es_419.po` (137 lines)
- `addons/project_sms/i18n/et.po` (135 lines)
- `addons/project_sms/i18n/fa.po` (119 lines)
- `addons/project_sms/i18n/fi.po` (136 lines)
- `addons/project_sms/i18n/fr.po` (136 lines)
- `addons/project_sms/i18n/he.po` (120 lines)
- `addons/project_sms/i18n/hi.po` (119 lines)
- `addons/project_sms/i18n/hr.po` (120 lines)
- `addons/project_sms/i18n/hu.po` (120 lines)
- `addons/project_sms/i18n/id.po` (137 lines)
- `addons/project_sms/i18n/it.po` (136 lines)
- `addons/project_sms/i18n/ja.po` (136 lines)
- `addons/project_sms/i18n/kab.po` (120 lines)
- `addons/project_sms/i18n/ko.po` (135 lines)
- `addons/project_sms/i18n/ku.po` (119 lines)
- `addons/project_sms/i18n/lo.po` (119 lines)
- `addons/project_sms/i18n/lt.po` (121 lines)
- `addons/project_sms/i18n/lv.po` (120 lines)
- `addons/project_sms/i18n/mn.po` (119 lines)
- `addons/project_sms/i18n/my.po` (120 lines)
- `addons/project_sms/i18n/nb.po` (120 lines)
- `addons/project_sms/i18n/nl.po` (136 lines)
- `addons/project_sms/i18n/pl.po` (138 lines)
- `addons/project_sms/i18n/project_sms.pot` (115 lines)
- `addons/project_sms/i18n/pt.po` (124 lines)
- `addons/project_sms/i18n/pt_BR.po` (138 lines)
- `addons/project_sms/i18n/ro.po` (136 lines)
- `addons/project_sms/i18n/ru.po` (139 lines)
- `addons/project_sms/i18n/sk.po` (119 lines)
- `addons/project_sms/i18n/sl.po` (121 lines)
- `addons/project_sms/i18n/sr@latin.po` (120 lines)
- `addons/project_sms/i18n/sv.po` (125 lines)
- `addons/project_sms/i18n/th.po` (132 lines)
- `addons/project_sms/i18n/tr.po` (138 lines)
- `addons/project_sms/i18n/uk.po` (120 lines)
- `addons/project_sms/i18n/uz.po` (149 lines)
- `addons/project_sms/i18n/vi.po` (136 lines)
- `addons/project_sms/i18n/zh_CN.po` (132 lines)
- `addons/project_sms/i18n/zh_TW.po` (134 lines)
- `addons/project_sms/models/__init__.py` (7 lines)
- `addons/project_sms/models/project_project.py` (28 lines)
- `addons/project_sms/models/project_stage.py` (12 lines)
- `addons/project_sms/models/project_task.py` (30 lines)
- `addons/project_sms/models/project_task_type.py` (12 lines)
- `addons/project_sms/security/ir.access.csv` (3 lines)
- `addons/project_sms/tests/__init__.py` (4 lines)
- `addons/project_sms/tests/test_project_sharing.py` (99 lines)
- `addons/project_sms/upgrades/1.1/pre-migrate.py` (13 lines)
- `addons/project_sms/views/project_project_views.xml` (17 lines)
- `addons/project_sms/views/project_stage_views.xml` (36 lines)
- `addons/project_sms/views/project_task_type_views.xml` (36 lines)
- `addons/project_sms/views/project_task_views.xml` (16 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
