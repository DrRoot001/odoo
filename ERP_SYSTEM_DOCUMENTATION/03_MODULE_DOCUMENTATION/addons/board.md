# Module: board

- **Module ID:** MOD-044
- **Path:** `addons/board`
- **Manifest:** `addons/board/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Build your own dashboards


Lets the user create a custom dashboard.
========================================

Allows users to create custom dashboard.
    

Declared dependencies: `spreadsheet_dashboard`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 6 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "spreadsheet_dashboard"
  ],
  "data": [
    "views/board_views.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "board/static/src/**/*.scss",
      "board/static/src/**/*.js",
      "board/static/src/**/*.xml"
    ],
    "web.assets_unit_tests": [
      "board/static/tests/**/*.test.js"
    ]
  }
}
```

### Representative source files

- `addons/board/__init__.py` (5 lines)
- `addons/board/__manifest__.py` (31 lines)
- `addons/board/controllers/__init__.py` (4 lines)
- `addons/board/controllers/main.py` (44 lines)
- `addons/board/i18n/af.po` (158 lines)
- `addons/board/i18n/ar.po` (166 lines)
- `addons/board/i18n/az.po` (156 lines)
- `addons/board/i18n/bg.po` (159 lines)
- `addons/board/i18n/bn.po` (156 lines)
- `addons/board/i18n/board.pot` (148 lines)
- `addons/board/i18n/bs.po` (157 lines)
- `addons/board/i18n/ca.po` (166 lines)
- `addons/board/i18n/cs.po` (166 lines)
- `addons/board/i18n/da.po` (166 lines)
- `addons/board/i18n/de.po` (175 lines)
- `addons/board/i18n/el.po` (160 lines)
- `addons/board/i18n/es.po` (171 lines)
- `addons/board/i18n/es_419.po` (168 lines)
- `addons/board/i18n/es_CL.po` (25 lines)
- `addons/board/i18n/et.po` (163 lines)
- `addons/board/i18n/eu.po` (157 lines)
- `addons/board/i18n/fa.po` (163 lines)
- `addons/board/i18n/fi.po` (175 lines)
- `addons/board/i18n/fo.po` (157 lines)
- `addons/board/i18n/fr.po` (177 lines)
- `addons/board/i18n/fr_BE.po` (24 lines)
- `addons/board/i18n/fr_CA.po` (25 lines)
- `addons/board/i18n/gl.po` (157 lines)
- `addons/board/i18n/gu.po` (158 lines)
- `addons/board/i18n/he.po` (166 lines)
- `addons/board/i18n/hi.po` (155 lines)
- `addons/board/i18n/hr.po` (163 lines)
- `addons/board/i18n/hu.po` (163 lines)
- `addons/board/i18n/id.po` (161 lines)
- `addons/board/i18n/is.po` (154 lines)
- `addons/board/i18n/it.po` (171 lines)
- `addons/board/i18n/ja.po` (170 lines)
- `addons/board/i18n/ka.po` (157 lines)
- `addons/board/i18n/kab.po` (154 lines)
- `addons/board/i18n/km.po` (157 lines)
- `addons/board/i18n/ko.po` (160 lines)
- `addons/board/i18n/ku.po` (152 lines)
- `addons/board/i18n/lo.po` (162 lines)
- `addons/board/i18n/lt.po` (161 lines)
- `addons/board/i18n/lv.po` (155 lines)
- `addons/board/i18n/mk.po` (157 lines)
- `addons/board/i18n/ml_IN.po` (157 lines)
- `addons/board/i18n/mn.po` (160 lines)
- `addons/board/i18n/my.po` (152 lines)
- `addons/board/i18n/nb.po` (155 lines)
- `addons/board/i18n/nl.po` (171 lines)
- `addons/board/i18n/pl.po` (169 lines)
- `addons/board/i18n/pt.po` (165 lines)
- `addons/board/i18n/pt_BR.po` (172 lines)
- `addons/board/i18n/ro.po` (163 lines)
- `addons/board/i18n/ru.po` (160 lines)
- `addons/board/i18n/sk.po` (159 lines)
- `addons/board/i18n/sl.po` (163 lines)
- `addons/board/i18n/sq.po` (157 lines)
- `addons/board/i18n/sr@latin.po` (156 lines)
- `addons/board/i18n/sv.po` (174 lines)
- `addons/board/i18n/ta.po` (157 lines)
- `addons/board/i18n/th.po` (166 lines)
- `addons/board/i18n/tr.po` (173 lines)
- `addons/board/i18n/uk.po` (163 lines)
- `addons/board/i18n/uz.po` (175 lines)
- `addons/board/i18n/vi.po` (162 lines)
- `addons/board/i18n/zh_CN.po` (166 lines)
- `addons/board/i18n/zh_TW.po` (161 lines)
- `addons/board/models/__init__.py` (4 lines)
- `addons/board/models/board.py` (54 lines)
- `addons/board/security/ir.access.csv` (2 lines)
- `addons/board/static/description/icon.png` (8 lines)
- `addons/board/static/description/icon.svg` (1 lines)
- `addons/board/static/description/icon_hi.png` (52 lines)
- `addons/board/static/img/layout_1-1-1.png` (7 lines)
- `addons/board/static/img/layout_1-1.png` (5 lines)
- `addons/board/static/img/layout_1-2.png` (7 lines)
- `addons/board/static/img/layout_1.png` (6 lines)
- `addons/board/static/img/layout_2-1.png` (5 lines)
- `addons/board/static/img/view_todo_arrow.png` (34 lines)
- `addons/board/static/src/add_to_board/add_to_board.js` (100 lines)
- `addons/board/static/src/add_to_board/add_to_board.xml` (32 lines)
- `addons/board/static/src/board_action.js` (82 lines)
- `addons/board/static/src/board_action.xml` (12 lines)
- `addons/board/static/src/board_controller.js` (136 lines)
- `addons/board/static/src/board_controller.scss` (58 lines)
- `addons/board/static/src/board_controller.xml` (89 lines)
- `addons/board/static/src/board_view.js` (73 lines)
- `addons/board/static/tests/add_to_dashboard.test.js` (438 lines)
- `addons/board/static/tests/board.test.js` (803 lines)
- `addons/board/views/board_views.xml` (38 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
