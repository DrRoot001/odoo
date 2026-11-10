# Module: project_mrp

- **Module ID:** MOD-480
- **Path:** `addons/project_mrp`
- **Manifest:** `addons/project_mrp/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Monitor MRP using project

No manifest description declared.

Declared dependencies: `mrp`, `project`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mrp",
    "project"
  ],
  "data": [
    "views/mrp_bom_views.xml",
    "views/mrp_production_views.xml",
    "views/project_project_views.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/project_mrp/__init__.py` (3 lines)
- `addons/project_mrp/__manifest__.py` (17 lines)
- `addons/project_mrp/i18n/ar.po` (97 lines)
- `addons/project_mrp/i18n/az.po` (93 lines)
- `addons/project_mrp/i18n/bg.po` (93 lines)
- `addons/project_mrp/i18n/bs.po` (95 lines)
- `addons/project_mrp/i18n/ca.po` (94 lines)
- `addons/project_mrp/i18n/cs.po` (95 lines)
- `addons/project_mrp/i18n/da.po` (94 lines)
- `addons/project_mrp/i18n/de.po` (95 lines)
- `addons/project_mrp/i18n/el.po` (94 lines)
- `addons/project_mrp/i18n/es.po` (96 lines)
- `addons/project_mrp/i18n/es_419.po` (96 lines)
- `addons/project_mrp/i18n/et.po` (94 lines)
- `addons/project_mrp/i18n/fa.po` (93 lines)
- `addons/project_mrp/i18n/fi.po` (95 lines)
- `addons/project_mrp/i18n/fr.po` (95 lines)
- `addons/project_mrp/i18n/he.po` (94 lines)
- `addons/project_mrp/i18n/hi.po` (93 lines)
- `addons/project_mrp/i18n/hr.po` (94 lines)
- `addons/project_mrp/i18n/hu.po` (94 lines)
- `addons/project_mrp/i18n/id.po` (96 lines)
- `addons/project_mrp/i18n/it.po` (95 lines)
- `addons/project_mrp/i18n/ja.po` (95 lines)
- `addons/project_mrp/i18n/kab.po` (94 lines)
- `addons/project_mrp/i18n/ko.po` (95 lines)
- `addons/project_mrp/i18n/ku.po` (93 lines)
- `addons/project_mrp/i18n/lo.po` (93 lines)
- `addons/project_mrp/i18n/lt.po` (95 lines)
- `addons/project_mrp/i18n/lv.po` (94 lines)
- `addons/project_mrp/i18n/mn.po` (93 lines)
- `addons/project_mrp/i18n/my.po` (94 lines)
- `addons/project_mrp/i18n/nb.po` (94 lines)
- `addons/project_mrp/i18n/nl.po` (95 lines)
- `addons/project_mrp/i18n/pl.po` (97 lines)
- `addons/project_mrp/i18n/project_mrp.pot` (90 lines)
- `addons/project_mrp/i18n/pt.po` (94 lines)
- `addons/project_mrp/i18n/pt_BR.po` (97 lines)
- `addons/project_mrp/i18n/ro.po` (95 lines)
- `addons/project_mrp/i18n/ru.po` (98 lines)
- `addons/project_mrp/i18n/sk.po` (93 lines)
- `addons/project_mrp/i18n/sl.po` (95 lines)
- `addons/project_mrp/i18n/sr@latin.po` (94 lines)
- `addons/project_mrp/i18n/sv.po` (95 lines)
- `addons/project_mrp/i18n/th.po` (95 lines)
- `addons/project_mrp/i18n/tr.po` (97 lines)
- `addons/project_mrp/i18n/uk.po` (94 lines)
- `addons/project_mrp/i18n/uz.po` (110 lines)
- `addons/project_mrp/i18n/vi.po` (95 lines)
- `addons/project_mrp/i18n/zh_CN.po` (95 lines)
- `addons/project_mrp/i18n/zh_TW.po` (97 lines)
- `addons/project_mrp/models/__init__.py` (6 lines)
- `addons/project_mrp/models/mrp_bom.py` (9 lines)
- `addons/project_mrp/models/mrp_production.py` (29 lines)
- `addons/project_mrp/models/project_project.py` (52 lines)
- `addons/project_mrp/models/stock.py` (24 lines)
- `addons/project_mrp/security/ir.access.csv` (3 lines)
- `addons/project_mrp/tests/__init__.py` (3 lines)
- `addons/project_mrp/tests/test_mto_replenishment.py` (45 lines)
- `addons/project_mrp/views/mrp_bom_views.xml` (13 lines)
- `addons/project_mrp/views/mrp_production_views.xml` (38 lines)
- `addons/project_mrp/views/project_project_views.xml` (60 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
