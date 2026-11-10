# Module: web_hierarchy

- **Module ID:** MOD-593
- **Path:** `addons/web_hierarchy`
- **Manifest:** `addons/web_hierarchy/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Odoo Web Hierarchy view
=======================

This module adds a new view called to be able to define a view to display
an organization such as an Organization Chart for employees for instance.
        

Declared dependencies: `web`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 10 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "web"
  ],
  "assets": {
    "web.assets_backend_lazy": [
      "web_hierarchy/static/src/**/*",
      [
        "remove",
        "web_hierarchy/static/src/hierarchy.variables.dark.scss"
      ]
    ],
    "web.assets_backend_lazy_dark": [
      [
        "before",
        "web_hierarchy/static/src/hierarchy.variables.scss",
        "web_hierarchy/static/src/hierarchy.variables.dark.scss"
      ]
    ],
    "web.assets_unit_tests": [
      "web_hierarchy/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/web_hierarchy/__init__.py` (3 lines)
- `addons/web_hierarchy/__manifest__.py` (29 lines)
- `addons/web_hierarchy/i18n/ar.po` (138 lines)
- `addons/web_hierarchy/i18n/az.po` (131 lines)
- `addons/web_hierarchy/i18n/bg.po` (131 lines)
- `addons/web_hierarchy/i18n/bs.po` (137 lines)
- `addons/web_hierarchy/i18n/ca.po` (136 lines)
- `addons/web_hierarchy/i18n/cs.po` (131 lines)
- `addons/web_hierarchy/i18n/da.po` (139 lines)
- `addons/web_hierarchy/i18n/de.po` (147 lines)
- `addons/web_hierarchy/i18n/el.po` (132 lines)
- `addons/web_hierarchy/i18n/es.po` (143 lines)
- `addons/web_hierarchy/i18n/es_419.po` (137 lines)
- `addons/web_hierarchy/i18n/et.po` (131 lines)
- `addons/web_hierarchy/i18n/fa.po` (135 lines)
- `addons/web_hierarchy/i18n/fi.po` (136 lines)
- `addons/web_hierarchy/i18n/fr.po` (140 lines)
- `addons/web_hierarchy/i18n/he.po` (132 lines)
- `addons/web_hierarchy/i18n/hi.po` (133 lines)
- `addons/web_hierarchy/i18n/hr.po` (132 lines)
- `addons/web_hierarchy/i18n/hu.po` (132 lines)
- `addons/web_hierarchy/i18n/id.po` (137 lines)
- `addons/web_hierarchy/i18n/it.po` (145 lines)
- `addons/web_hierarchy/i18n/ja.po` (135 lines)
- `addons/web_hierarchy/i18n/kab.po` (134 lines)
- `addons/web_hierarchy/i18n/ko.po` (137 lines)
- `addons/web_hierarchy/i18n/ku.po` (131 lines)
- `addons/web_hierarchy/i18n/lo.po` (149 lines)
- `addons/web_hierarchy/i18n/lt.po` (133 lines)
- `addons/web_hierarchy/i18n/lv.po` (137 lines)
- `addons/web_hierarchy/i18n/mn.po` (131 lines)
- `addons/web_hierarchy/i18n/my.po` (132 lines)
- `addons/web_hierarchy/i18n/nb.po` (131 lines)
- `addons/web_hierarchy/i18n/nl.po` (138 lines)
- `addons/web_hierarchy/i18n/pl.po` (141 lines)
- `addons/web_hierarchy/i18n/pt.po` (139 lines)
- `addons/web_hierarchy/i18n/pt_BR.po` (145 lines)
- `addons/web_hierarchy/i18n/ro.po` (138 lines)
- `addons/web_hierarchy/i18n/ru.po` (142 lines)
- `addons/web_hierarchy/i18n/sk.po` (137 lines)
- `addons/web_hierarchy/i18n/sl.po` (133 lines)
- `addons/web_hierarchy/i18n/sr@latin.po` (132 lines)
- `addons/web_hierarchy/i18n/sv.po` (138 lines)
- `addons/web_hierarchy/i18n/th.po` (133 lines)
- `addons/web_hierarchy/i18n/tr.po` (141 lines)
- `addons/web_hierarchy/i18n/uk.po` (137 lines)
- `addons/web_hierarchy/i18n/uz.po` (158 lines)
- `addons/web_hierarchy/i18n/vi.po` (137 lines)
- `addons/web_hierarchy/i18n/web_hierarchy.pot` (125 lines)
- `addons/web_hierarchy/i18n/zh_CN.po` (133 lines)
- `addons/web_hierarchy/i18n/zh_TW.po` (136 lines)
- `addons/web_hierarchy/models/__init__.py` (5 lines)
- `addons/web_hierarchy/models/ir_actions.py` (9 lines)
- `addons/web_hierarchy/models/ir_ui_view.py` (58 lines)
- `addons/web_hierarchy/models/models.py` (41 lines)
- `addons/web_hierarchy/static/src/hierarchy.variables.dark.scss` (3 lines)
- `addons/web_hierarchy/static/src/hierarchy.variables.scss` (3 lines)
- `addons/web_hierarchy/static/src/hierarchy_arch_parser.js` (83 lines)
- `addons/web_hierarchy/static/src/hierarchy_card.js` (71 lines)
- `addons/web_hierarchy/static/src/hierarchy_card.scss` (77 lines)
- `addons/web_hierarchy/static/src/hierarchy_card.xml` (53 lines)
- `addons/web_hierarchy/static/src/hierarchy_compiler.js` (43 lines)
- `addons/web_hierarchy/static/src/hierarchy_controller.js` (79 lines)
- `addons/web_hierarchy/static/src/hierarchy_controller.xml` (42 lines)
- `addons/web_hierarchy/static/src/hierarchy_model.js` (1,208 lines)
- `addons/web_hierarchy/static/src/hierarchy_node_draggable.js` (92 lines)
- `addons/web_hierarchy/static/src/hierarchy_renderer.js` (156 lines)
- `addons/web_hierarchy/static/src/hierarchy_renderer.scss` (74 lines)
- `addons/web_hierarchy/static/src/hierarchy_renderer.xml` (40 lines)
- `addons/web_hierarchy/static/src/hierarchy_view.js` (29 lines)
- `addons/web_hierarchy/static/tests/hierarchy_mock_server.js` (76 lines)
- `addons/web_hierarchy/static/tests/hierarchy_view.test.js` (1,561 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
