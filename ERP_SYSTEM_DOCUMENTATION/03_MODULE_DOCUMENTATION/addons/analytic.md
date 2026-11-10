# Module: analytic

- **Module ID:** MOD-017
- **Path:** `addons/analytic`
- **Manifest:** `addons/analytic/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Module for defining analytic accounting object.
===============================================

In Odoo, analytic accounts are linked to general accounts but are treated
totally independently. So, you can enter various different analytic operations
that have no counterpart in the general financial accounts.
    

Declared dependencies: `base`, `mail`, `uom`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 18 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 9 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 8 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 18 | Client behavior/assets. |
| Tests | 6 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base",
    "mail",
    "uom"
  ],
  "data": [
    "security/analytic_security.xml",
    "views/analytic_line_views.xml",
    "views/analytic_account_views.xml",
    "views/analytic_plan_views.xml",
    "views/analytic_distribution_model_views.xml",
    "data/analytic_data.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/analytic_account_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "analytic/static/src/components/**/*",
      "analytic/static/src/services/**/*",
      "analytic/static/src/views/**/*",
      [
        "remove",
        "analytic/static/src/views/graph/**"
      ],
      [
        "remove",
        "analytic/static/src/views/pivot/**"
      ]
    ],
    "web.assets_backend_lazy": [
      "analytic/static/src/views/graph/**",
      "analytic/static/src/views/pivot/**"
    ],
    "web.assets_unit_tests": [
      "analytic/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/analytic/__init__.py` (4 lines)
- `addons/analytic/__manifest__.py` (46 lines)
- `addons/analytic/data/analytic_account_demo.xml` (144 lines)
- `addons/analytic/data/analytic_data.xml` (19 lines)
- `addons/analytic/i18n/af.po` (983 lines)
- `addons/analytic/i18n/am.po` (979 lines)
- `addons/analytic/i18n/analytic.pot` (988 lines)
- `addons/analytic/i18n/ar.po` (1,031 lines)
- `addons/analytic/i18n/az.po` (1,027 lines)
- `addons/analytic/i18n/bg.po` (1,020 lines)
- `addons/analytic/i18n/bs.po` (1,001 lines)
- `addons/analytic/i18n/ca.po` (1,037 lines)
- `addons/analytic/i18n/cs.po` (1,033 lines)
- `addons/analytic/i18n/da.po` (1,037 lines)
- `addons/analytic/i18n/de.po` (1,047 lines)
- `addons/analytic/i18n/el.po` (1,032 lines)
- `addons/analytic/i18n/es.po` (1,049 lines)
- `addons/analytic/i18n/es_419.po` (1,038 lines)
- `addons/analytic/i18n/es_CL.po` (134 lines)
- `addons/analytic/i18n/et.po` (1,039 lines)
- `addons/analytic/i18n/eu.po` (982 lines)
- `addons/analytic/i18n/fa.po` (1,032 lines)
- `addons/analytic/i18n/fi.po` (1,057 lines)
- `addons/analytic/i18n/fo.po` (982 lines)
- `addons/analytic/i18n/fr.po` (1,051 lines)
- `addons/analytic/i18n/fr_BE.po` (121 lines)
- `addons/analytic/i18n/fr_CA.po` (110 lines)
- `addons/analytic/i18n/gl.po` (982 lines)
- `addons/analytic/i18n/gu.po` (983 lines)
- `addons/analytic/i18n/he.po` (1,033 lines)
- `addons/analytic/i18n/hi.po` (1,020 lines)
- `addons/analytic/i18n/hr.po` (1,018 lines)
- `addons/analytic/i18n/hu.po` (1,021 lines)
- `addons/analytic/i18n/hy.po` (981 lines)
- `addons/analytic/i18n/id.po` (1,035 lines)
- `addons/analytic/i18n/is.po` (983 lines)
- `addons/analytic/i18n/it.po` (1,048 lines)
- `addons/analytic/i18n/ja.po` (1,038 lines)
- `addons/analytic/i18n/ka.po` (982 lines)
- `addons/analytic/i18n/kab.po` (998 lines)
- `addons/analytic/i18n/kk.po` (981 lines)
- `addons/analytic/i18n/km.po` (984 lines)
- `addons/analytic/i18n/ko.po` (1,025 lines)
- `addons/analytic/i18n/ku.po` (1,007 lines)
- `addons/analytic/i18n/lo.po` (1,026 lines)
- `addons/analytic/i18n/lt.po` (1,041 lines)
- `addons/analytic/i18n/lv.po` (1,005 lines)
- `addons/analytic/i18n/mk.po` (982 lines)
- `addons/analytic/i18n/mn.po` (1,046 lines)
- `addons/analytic/i18n/my.po` (997 lines)
- `addons/analytic/i18n/nb.po` (1,002 lines)
- `addons/analytic/i18n/nl.po` (1,045 lines)
- `addons/analytic/i18n/pl.po` (1,051 lines)
- `addons/analytic/i18n/pt.po` (1,042 lines)
- `addons/analytic/i18n/pt_BR.po` (1,047 lines)
- `addons/analytic/i18n/ro.po` (1,033 lines)
- `addons/analytic/i18n/ru.po` (1,037 lines)
- `addons/analytic/i18n/sk.po` (1,014 lines)
- `addons/analytic/i18n/sl.po` (1,032 lines)
- `addons/analytic/i18n/sq.po` (982 lines)
- `addons/analytic/i18n/sr@latin.po` (1,001 lines)
- `addons/analytic/i18n/sv.po` (1,038 lines)
- `addons/analytic/i18n/ta.po` (983 lines)
- `addons/analytic/i18n/te.po` (981 lines)
- `addons/analytic/i18n/th.po` (1,023 lines)
- `addons/analytic/i18n/tr.po` (1,056 lines)
- `addons/analytic/i18n/uk.po` (1,029 lines)
- `addons/analytic/i18n/uz.po` (1,188 lines)
- `addons/analytic/i18n/vi.po` (1,035 lines)
- `addons/analytic/i18n/zh_CN.po` (1,027 lines)
- `addons/analytic/i18n/zh_TW.po` (1,016 lines)
- `addons/analytic/migrations/1.2/pre-migrate.py` (31 lines)
- `addons/analytic/models/__init__.py` (12 lines)
- `addons/analytic/models/analytic_account.py` (235 lines)
- `addons/analytic/models/analytic_distribution_model.py` (99 lines)
- `addons/analytic/models/analytic_line.py` (288 lines)
- `addons/analytic/models/analytic_mixin.py` (323 lines)
- `addons/analytic/models/analytic_plan.py` (495 lines)
- `addons/analytic/models/ir_config_parameter.py` (29 lines)
- `addons/analytic/models/res_config_settings.py` (10 lines)
- `addons/analytic/models/res_groups.py` (13 lines)
- `addons/analytic/security/analytic_security.xml` (8 lines)
- `addons/analytic/security/ir.access.csv` (10 lines)
- `addons/analytic/static/src/components/analytic_distribution/analytic_distribution.js` (781 lines)
- `addons/analytic/static/src/components/analytic_distribution/analytic_distribution.scss` (84 lines)
- `addons/analytic/static/src/components/analytic_distribution/analytic_distribution.xml` (88 lines)
- `addons/analytic/static/src/services/batched_orm_service.js` (87 lines)
- `addons/analytic/static/src/services/reload_analytic_plan_service.js` (21 lines)
- `addons/analytic/static/src/views/analytic_search_model.js` (30 lines)
- `addons/analytic/static/src/views/graph/graph_view.js` (10 lines)
- `addons/analytic/static/src/views/kanban/kanban_view.js` (10 lines)
- `addons/analytic/static/src/views/list/list_view.js` (10 lines)
- `addons/analytic/static/src/views/pivot/pivot_renderer.js` (26 lines)
- `addons/analytic/static/src/views/pivot/pivot_view.js` (12 lines)
- `addons/analytic/static/tests/analytic_distribution.test.js` (417 lines)
- `addons/analytic/static/tests/analytic_test_helpers.js` (17 lines)
- `addons/analytic/static/tests/analytic_views.test.js` (121 lines)
- `addons/analytic/static/tests/analytic_widget.test.js` (253 lines)
- `addons/analytic/static/tests/batched_orm_service.test.js` (67 lines)
- `addons/analytic/static/tests/mock_server/mock_models/account_analytic_account.js` (8 lines)
- `addons/analytic/static/tests/mock_server/mock_models/account_analytic_distribution_model.js` (7 lines)
- `addons/analytic/static/tests/mock_server/mock_models/account_analytic_line.js` (13 lines)
- `addons/analytic/static/tests/mock_server/mock_models/account_analytic_plan.js` (21 lines)
- `addons/analytic/tests/__init__.py` (6 lines)
- `addons/analytic/tests/common.py` (65 lines)
- `addons/analytic/tests/test_analytic_account.py` (368 lines)
- `addons/analytic/tests/test_analytic_dynamic_update.py` (242 lines)
- `addons/analytic/tests/test_analytic_mixin.py` (84 lines)
- `addons/analytic/tests/test_plan_operations.py` (148 lines)
- `addons/analytic/views/analytic_account_views.xml` (145 lines)
- `addons/analytic/views/analytic_distribution_model_views.xml` (53 lines)
- `addons/analytic/views/analytic_line_views.xml` (170 lines)
- `addons/analytic/views/analytic_plan_views.xml` (81 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
