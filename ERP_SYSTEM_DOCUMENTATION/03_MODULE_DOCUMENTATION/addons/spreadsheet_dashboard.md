# Module: spreadsheet_dashboard

- **Module ID:** MOD-546
- **Path:** `addons/spreadsheet_dashboard`
- **Manifest:** `addons/spreadsheet_dashboard/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Spreadsheet

Spreadsheet

Declared dependencies: `spreadsheet`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 18 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 15 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 37 | Client behavior/assets. |
| Tests | 8 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 4 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "spreadsheet"
  ],
  "data": [
    "security/security.xml",
    "views/spreadsheet_dashboard_views.xml",
    "views/menu_views.xml",
    "data/dashboard.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "spreadsheet.o_spreadsheet": [
      "spreadsheet_dashboard/static/src/bundle/**/*.js",
      "spreadsheet_dashboard/static/src/bundle/**/*.xml"
    ],
    "spreadsheet.public_spreadsheet": [
      "spreadsheet_dashboard/static/src/public/**/*.js",
      "spreadsheet_dashboard/static/src/public/**/*.xml",
      "spreadsheet_dashboard/static/src/public/**/*.scss"
    ],
    "web.assets_backend": [
      "spreadsheet_dashboard/static/src/assets/**/*.js",
      "spreadsheet_dashboard/static/src/**/*.scss"
    ],
    "web.assets_unit_tests": [
      "spreadsheet_dashboard/static/src/public/**/*.js",
      "spreadsheet_dashboard/static/src/public/**/*.xml",
      "spreadsheet_dashboard/static/tests/**/*"
    ],
    "web.assets_tests": [
      "spreadsheet_dashboard/static/tests/tours/*"
    ]
  }
}
```

### Representative source files

- `addons/spreadsheet_dashboard/__init__.py` (4 lines)
- `addons/spreadsheet_dashboard/__manifest__.py` (40 lines)
- `addons/spreadsheet_dashboard/controllers/__init__.py` (2 lines)
- `addons/spreadsheet_dashboard/controllers/dashboards_controllers.py` (29 lines)
- `addons/spreadsheet_dashboard/controllers/share.py` (59 lines)
- `addons/spreadsheet_dashboard/data/dashboard.xml` (39 lines)
- `addons/spreadsheet_dashboard/i18n/ar.po` (652 lines)
- `addons/spreadsheet_dashboard/i18n/az.po` (647 lines)
- `addons/spreadsheet_dashboard/i18n/bg.po` (647 lines)
- `addons/spreadsheet_dashboard/i18n/bs.po` (647 lines)
- `addons/spreadsheet_dashboard/i18n/ca.po` (648 lines)
- `addons/spreadsheet_dashboard/i18n/cs.po` (648 lines)
- `addons/spreadsheet_dashboard/i18n/da.po` (648 lines)
- `addons/spreadsheet_dashboard/i18n/de.po` (653 lines)
- `addons/spreadsheet_dashboard/i18n/el.po` (648 lines)
- `addons/spreadsheet_dashboard/i18n/es.po` (655 lines)
- `addons/spreadsheet_dashboard/i18n/es_419.po` (654 lines)
- `addons/spreadsheet_dashboard/i18n/et.po` (647 lines)
- `addons/spreadsheet_dashboard/i18n/fa.po` (647 lines)
- `addons/spreadsheet_dashboard/i18n/fi.po` (652 lines)
- `addons/spreadsheet_dashboard/i18n/fr.po` (658 lines)
- `addons/spreadsheet_dashboard/i18n/he.po` (648 lines)
- `addons/spreadsheet_dashboard/i18n/hi.po` (647 lines)
- `addons/spreadsheet_dashboard/i18n/hr.po` (648 lines)
- `addons/spreadsheet_dashboard/i18n/hu.po` (648 lines)
- `addons/spreadsheet_dashboard/i18n/id.po` (649 lines)
- `addons/spreadsheet_dashboard/i18n/it.po` (653 lines)
- `addons/spreadsheet_dashboard/i18n/ja.po` (651 lines)
- `addons/spreadsheet_dashboard/i18n/kab.po` (646 lines)
- `addons/spreadsheet_dashboard/i18n/ko.po` (648 lines)
- `addons/spreadsheet_dashboard/i18n/ku.po` (647 lines)
- `addons/spreadsheet_dashboard/i18n/lo.po` (648 lines)
- `addons/spreadsheet_dashboard/i18n/lt.po` (649 lines)
- `addons/spreadsheet_dashboard/i18n/lv.po` (646 lines)
- `addons/spreadsheet_dashboard/i18n/mn.po` (648 lines)
- `addons/spreadsheet_dashboard/i18n/my.po` (648 lines)
- `addons/spreadsheet_dashboard/i18n/nb.po` (648 lines)
- `addons/spreadsheet_dashboard/i18n/nl.po` (658 lines)
- `addons/spreadsheet_dashboard/i18n/pl.po` (650 lines)
- `addons/spreadsheet_dashboard/i18n/pt.po` (649 lines)
- `addons/spreadsheet_dashboard/i18n/pt_BR.po` (656 lines)
- `addons/spreadsheet_dashboard/i18n/ro.po` (649 lines)
- `addons/spreadsheet_dashboard/i18n/ru.po` (653 lines)
- `addons/spreadsheet_dashboard/i18n/sk.po` (645 lines)
- `addons/spreadsheet_dashboard/i18n/sl.po` (649 lines)
- `addons/spreadsheet_dashboard/i18n/spreadsheet_dashboard.pot` (642 lines)
- `addons/spreadsheet_dashboard/i18n/sr@latin.po` (649 lines)
- `addons/spreadsheet_dashboard/i18n/sv.po` (648 lines)
- `addons/spreadsheet_dashboard/i18n/th.po` (649 lines)
- `addons/spreadsheet_dashboard/i18n/tr.po` (651 lines)
- `addons/spreadsheet_dashboard/i18n/uk.po` (648 lines)
- `addons/spreadsheet_dashboard/i18n/uz.po` (711 lines)
- `addons/spreadsheet_dashboard/i18n/vi.po` (650 lines)
- `addons/spreadsheet_dashboard/i18n/zh_CN.po` (649 lines)
- `addons/spreadsheet_dashboard/i18n/zh_TW.po` (652 lines)
- `addons/spreadsheet_dashboard/models/__init__.py` (6 lines)
- `addons/spreadsheet_dashboard/models/spreadsheet_dashboard.py` (92 lines)
- `addons/spreadsheet_dashboard/models/spreadsheet_dashboard_favorite_filters.py` (25 lines)
- `addons/spreadsheet_dashboard/models/spreadsheet_dashboard_group.py` (21 lines)
- `addons/spreadsheet_dashboard/models/spreadsheet_dashboard_share.py` (54 lines)
- `addons/spreadsheet_dashboard/security/ir.access.csv` (11 lines)
- `addons/spreadsheet_dashboard/security/security.xml` (16 lines)
- `addons/spreadsheet_dashboard/static/description/icon.png` (8 lines)
- `addons/spreadsheet_dashboard/static/description/icon.svg` (1 lines)
- `addons/spreadsheet_dashboard/static/description/icon_hi.png` (52 lines)
- `addons/spreadsheet_dashboard/static/src/assets/dashboard_action_loader.js` (4 lines)
- `addons/spreadsheet_dashboard/static/src/assets/global_filter_widget_loader.js` (37 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/chart/chart_js_component_dashboard.js` (24 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/chart/chart_menu.js` (17 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/chart/chart_menu.scss` (58 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/chart/chart_menu.xml` (20 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/dashboard_action/dashboard_action.js` (180 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/dashboard_action/dashboard_action.scss` (123 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/dashboard_action/dashboard_action.xml` (106 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/dashboard_action/dashboard_date_filter/dashboard_date_filter.js` (50 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/dashboard_action/dashboard_date_filter/dashboard_date_filter.scss` (4 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/dashboard_action/dashboard_date_filter/dashboard_date_filter.xml` (24 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/dashboard_action/dashboard_facet/dashboard_facet.js` (12 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/dashboard_action/dashboard_facet/dashboard_facet.xml` (25 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/dashboard_action/dashboard_filter_list/dashboard_filter_list.js` (72 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/dashboard_action/dashboard_filter_list/dashboard_filter_list.scss` (21 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/dashboard_action/dashboard_filter_list/dashboard_filter_list.xml` (37 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/dashboard_action/dashboard_loader_service.js` (321 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/dashboard_action/dashboard_menu_translate_service.js` (31 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/dashboard_action/dashboard_search_bar/dashboard_search_bar.js` (488 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/dashboard_action/dashboard_search_bar/dashboard_search_bar.scss` (19 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/dashboard_action/dashboard_search_bar/dashboard_search_bar.xml` (76 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/dashboard_action/dashboard_search_bar_menu/dashboard_custom_favorite_item.js` (66 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/dashboard_action/dashboard_search_bar_menu/dashboard_search_bar_menu.js` (154 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/dashboard_action/dashboard_search_bar_menu/dashboard_search_bar_menu.scss` (22 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/dashboard_action/dashboard_search_bar_menu/dashboard_search_bar_menu.xml` (47 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/dashboard_action/dashboard_search_model.js` (277 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/dashboard_action/mobile_figure_container/mobile_figure_container.js` (147 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/dashboard_action/mobile_figure_container/mobile_figure_container.scss` (21 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/dashboard_action/mobile_figure_container/mobile_figure_container.xml` (29 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/dashboard_action/mobile_search_panel/mobile_search_panel.js` (38 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/dashboard_action/mobile_search_panel/mobile_search_panel.xml` (42 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/global_filter_widget/global_filter_widget.js` (104 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/global_filter_widget/global_filter_widget.xml` (22 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/list/clickable_cell.js` (58 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/list/sort_icon.js` (25 lines)
- `addons/spreadsheet_dashboard/static/src/bundle/pivot/clickable_cell.js` (25 lines)
- `addons/spreadsheet_dashboard/static/src/public/public_dashboard.js` (70 lines)
- `addons/spreadsheet_dashboard/static/src/public/public_dashboard.scss` (22 lines)
- `addons/spreadsheet_dashboard/static/src/public/public_dashboard.xml` (27 lines)
- `addons/spreadsheet_dashboard/static/tests/chart/chart_dashboard_menu.test.js` (47 lines)
- `addons/spreadsheet_dashboard/static/tests/chart/dashboard_chart_animations.test.js` (77 lines)
- `addons/spreadsheet_dashboard/static/tests/chart/dashboard_chart_menu.test.js` (265 lines)
- `addons/spreadsheet_dashboard/static/tests/clickable_cells/clickable_cells.test.js` (232 lines)
- `addons/spreadsheet_dashboard/static/tests/dashboard/dashboard_action.test.js` (1,121 lines)
- `addons/spreadsheet_dashboard/static/tests/dashboard/dashboard_action_mobile.test.js` (41 lines)
- `addons/spreadsheet_dashboard/static/tests/dashboard/dashboard_date_filter.test.js` (50 lines)
- `addons/spreadsheet_dashboard/static/tests/dashboard/dashboard_filter_list.test.js` (185 lines)
- `addons/spreadsheet_dashboard/static/tests/dashboard/dashboard_loader.test.js` (266 lines)
- `addons/spreadsheet_dashboard/static/tests/dashboard/dashboard_search_model.test.js` (427 lines)
- `addons/spreadsheet_dashboard/static/tests/global_filter_widget/global_filter_widget.test.js` (149 lines)
- `addons/spreadsheet_dashboard/static/tests/helpers/dashboard_action.js` (86 lines)
- `addons/spreadsheet_dashboard/static/tests/helpers/data.js` (139 lines)
- `addons/spreadsheet_dashboard/static/tests/mobile/mobile_dashboard_action.test.js` (297 lines)
- `addons/spreadsheet_dashboard/static/tests/public/public_dashboard.test.js` (82 lines)
- `addons/spreadsheet_dashboard/static/tests/tours/share_dashboard_public_tour.js` (10 lines)
- `addons/spreadsheet_dashboard/tests/__init__.py` (6 lines)
- `addons/spreadsheet_dashboard/tests/common.py` (39 lines)
- `addons/spreadsheet_dashboard/tests/data/sample_dashboard.json` (3 lines)
- `addons/spreadsheet_dashboard/tests/test_dashboard_controllers.py` (77 lines)
- `addons/spreadsheet_dashboard/tests/test_dashboard_favorite_filters.py` (67 lines)
- `addons/spreadsheet_dashboard/tests/test_dashboard_share.py` (59 lines)
- `addons/spreadsheet_dashboard/tests/test_share_controllers.py` (127 lines)
- `addons/spreadsheet_dashboard/tests/test_share_dashboard_tour.py` (18 lines)
- `addons/spreadsheet_dashboard/tests/test_spreadsheet_dashboard.py` (121 lines)
- `addons/spreadsheet_dashboard/views/menu_views.xml` (88 lines)
- `addons/spreadsheet_dashboard/views/spreadsheet_dashboard_views.xml` (182 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
