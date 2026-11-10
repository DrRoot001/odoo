# Module: project_mrp_sale

- **Module ID:** MOD-482
- **Path:** `addons/project_mrp_sale`
- **Manifest:** `addons/project_mrp_sale/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Technical Bridge

No manifest description declared.

Declared dependencies: `project_mrp`, `sale_mrp`, `sale_project`.

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
{
  "depends": [
    "project_mrp",
    "sale_mrp",
    "sale_project"
  ]
}
```

### Representative source files

- `addons/project_mrp_sale/__init__.py` (3 lines)
- `addons/project_mrp_sale/__manifest__.py` (11 lines)
- `addons/project_mrp_sale/i18n/ar.po` (52 lines)
- `addons/project_mrp_sale/i18n/az.po` (50 lines)
- `addons/project_mrp_sale/i18n/bg.po` (50 lines)
- `addons/project_mrp_sale/i18n/bs.po` (51 lines)
- `addons/project_mrp_sale/i18n/ca.po` (50 lines)
- `addons/project_mrp_sale/i18n/cs.po` (50 lines)
- `addons/project_mrp_sale/i18n/da.po` (50 lines)
- `addons/project_mrp_sale/i18n/de.po` (54 lines)
- `addons/project_mrp_sale/i18n/el.po` (50 lines)
- `addons/project_mrp_sale/i18n/es.po` (54 lines)
- `addons/project_mrp_sale/i18n/es_419.po` (54 lines)
- `addons/project_mrp_sale/i18n/et.po` (50 lines)
- `addons/project_mrp_sale/i18n/fa.po` (50 lines)
- `addons/project_mrp_sale/i18n/fi.po` (51 lines)
- `addons/project_mrp_sale/i18n/fr.po` (55 lines)
- `addons/project_mrp_sale/i18n/he.po` (51 lines)
- `addons/project_mrp_sale/i18n/hi.po` (50 lines)
- `addons/project_mrp_sale/i18n/hr.po` (51 lines)
- `addons/project_mrp_sale/i18n/hu.po` (50 lines)
- `addons/project_mrp_sale/i18n/id.po` (50 lines)
- `addons/project_mrp_sale/i18n/it.po` (54 lines)
- `addons/project_mrp_sale/i18n/ja.po` (54 lines)
- `addons/project_mrp_sale/i18n/kab.po` (50 lines)
- `addons/project_mrp_sale/i18n/ko.po` (50 lines)
- `addons/project_mrp_sale/i18n/ku.po` (50 lines)
- `addons/project_mrp_sale/i18n/lo.po` (50 lines)
- `addons/project_mrp_sale/i18n/lt.po` (52 lines)
- `addons/project_mrp_sale/i18n/lv.po` (51 lines)
- `addons/project_mrp_sale/i18n/mn.po` (50 lines)
- `addons/project_mrp_sale/i18n/my.po` (50 lines)
- `addons/project_mrp_sale/i18n/nb.po` (50 lines)
- `addons/project_mrp_sale/i18n/nl.po` (54 lines)
- `addons/project_mrp_sale/i18n/pl.po` (51 lines)
- `addons/project_mrp_sale/i18n/project_mrp_sale.pot` (47 lines)
- `addons/project_mrp_sale/i18n/pt.po` (50 lines)
- `addons/project_mrp_sale/i18n/pt_BR.po` (56 lines)
- `addons/project_mrp_sale/i18n/ro.po` (51 lines)
- `addons/project_mrp_sale/i18n/ru.po` (51 lines)
- `addons/project_mrp_sale/i18n/sk.po` (50 lines)
- `addons/project_mrp_sale/i18n/sl.po` (51 lines)
- `addons/project_mrp_sale/i18n/sr@latin.po` (51 lines)
- `addons/project_mrp_sale/i18n/sv.po` (51 lines)
- `addons/project_mrp_sale/i18n/th.po` (54 lines)
- `addons/project_mrp_sale/i18n/tr.po` (51 lines)
- `addons/project_mrp_sale/i18n/uk.po` (51 lines)
- `addons/project_mrp_sale/i18n/uz.po` (50 lines)
- `addons/project_mrp_sale/i18n/vi.po` (50 lines)
- `addons/project_mrp_sale/i18n/zh_CN.po` (54 lines)
- `addons/project_mrp_sale/i18n/zh_TW.po` (50 lines)
- `addons/project_mrp_sale/models/__init__.py` (3 lines)
- `addons/project_mrp_sale/models/account_analytic_line.py` (15 lines)
- `addons/project_mrp_sale/tests/__init__.py` (3 lines)
- `addons/project_mrp_sale/tests/test_sale_mrp_account.py` (72 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
