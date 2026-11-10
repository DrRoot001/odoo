# Module: crm_sale_project

- **Module ID:** MOD-059
- **Path:** `addons/crm_sale_project`
- **Manifest:** `addons/crm_sale_project/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Project Generation from Opportunities

No manifest description declared.

Declared dependencies: `sale_project`, `crm`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sale_project",
    "crm"
  ],
  "data": [
    "data/ir_actions_server_data.xml",
    "views/crm_lead_views.xml",
    "views/project_project_views.xml",
    "wizard/project_template_create_wizard.xml"
  ]
}
```

### Representative source files

- `addons/crm_sale_project/__init__.py` (2 lines)
- `addons/crm_sale_project/__manifest__.py` (18 lines)
- `addons/crm_sale_project/data/ir_actions_server_data.xml` (15 lines)
- `addons/crm_sale_project/i18n/ar.po` (122 lines)
- `addons/crm_sale_project/i18n/az.po` (121 lines)
- `addons/crm_sale_project/i18n/bg.po` (121 lines)
- `addons/crm_sale_project/i18n/bs.po` (122 lines)
- `addons/crm_sale_project/i18n/ca.po` (121 lines)
- `addons/crm_sale_project/i18n/crm_sale_project.pot` (118 lines)
- `addons/crm_sale_project/i18n/cs.po` (122 lines)
- `addons/crm_sale_project/i18n/da.po` (122 lines)
- `addons/crm_sale_project/i18n/de.po` (123 lines)
- `addons/crm_sale_project/i18n/el.po` (121 lines)
- `addons/crm_sale_project/i18n/es.po` (122 lines)
- `addons/crm_sale_project/i18n/es_419.po` (122 lines)
- `addons/crm_sale_project/i18n/et.po` (121 lines)
- `addons/crm_sale_project/i18n/fa.po` (121 lines)
- `addons/crm_sale_project/i18n/fi.po` (122 lines)
- `addons/crm_sale_project/i18n/fr.po` (123 lines)
- `addons/crm_sale_project/i18n/he.po` (122 lines)
- `addons/crm_sale_project/i18n/hi.po` (121 lines)
- `addons/crm_sale_project/i18n/hr.po` (122 lines)
- `addons/crm_sale_project/i18n/hu.po` (121 lines)
- `addons/crm_sale_project/i18n/id.po` (124 lines)
- `addons/crm_sale_project/i18n/it.po` (122 lines)
- `addons/crm_sale_project/i18n/ja.po` (122 lines)
- `addons/crm_sale_project/i18n/kab.po` (121 lines)
- `addons/crm_sale_project/i18n/ko.po` (122 lines)
- `addons/crm_sale_project/i18n/ku.po` (121 lines)
- `addons/crm_sale_project/i18n/lo.po` (121 lines)
- `addons/crm_sale_project/i18n/lt.po` (123 lines)
- `addons/crm_sale_project/i18n/lv.po` (122 lines)
- `addons/crm_sale_project/i18n/mn.po` (121 lines)
- `addons/crm_sale_project/i18n/my.po` (122 lines)
- `addons/crm_sale_project/i18n/nb.po` (121 lines)
- `addons/crm_sale_project/i18n/nl.po` (122 lines)
- `addons/crm_sale_project/i18n/pl.po` (122 lines)
- `addons/crm_sale_project/i18n/pt.po` (121 lines)
- `addons/crm_sale_project/i18n/pt_BR.po` (122 lines)
- `addons/crm_sale_project/i18n/ro.po` (122 lines)
- `addons/crm_sale_project/i18n/ru.po` (123 lines)
- `addons/crm_sale_project/i18n/sk.po` (121 lines)
- `addons/crm_sale_project/i18n/sl.po` (122 lines)
- `addons/crm_sale_project/i18n/sr@latin.po` (122 lines)
- `addons/crm_sale_project/i18n/sv.po` (122 lines)
- `addons/crm_sale_project/i18n/th.po` (122 lines)
- `addons/crm_sale_project/i18n/tr.po` (122 lines)
- `addons/crm_sale_project/i18n/uk.po` (122 lines)
- `addons/crm_sale_project/i18n/uz.po` (121 lines)
- `addons/crm_sale_project/i18n/vi.po` (121 lines)
- `addons/crm_sale_project/i18n/zh_CN.po` (123 lines)
- `addons/crm_sale_project/i18n/zh_TW.po` (121 lines)
- `addons/crm_sale_project/models/__init__.py` (3 lines)
- `addons/crm_sale_project/models/crm_lead.py` (109 lines)
- `addons/crm_sale_project/models/project_project.py` (31 lines)
- `addons/crm_sale_project/models/sale_order.py` (17 lines)
- `addons/crm_sale_project/tests/__init__.py` (1 lines)
- `addons/crm_sale_project/tests/test_crm_sale_project.py` (46 lines)
- `addons/crm_sale_project/views/crm_lead_views.xml` (38 lines)
- `addons/crm_sale_project/views/project_project_views.xml` (20 lines)
- `addons/crm_sale_project/wizard/__init__.py` (1 lines)
- `addons/crm_sale_project/wizard/project_template_create_wizard.py` (46 lines)
- `addons/crm_sale_project/wizard/project_template_create_wizard.xml` (36 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
