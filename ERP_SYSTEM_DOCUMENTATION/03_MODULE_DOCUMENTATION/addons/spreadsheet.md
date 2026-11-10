# Module: spreadsheet

- **Module ID:** MOD-544
- **Path:** `addons/spreadsheet`
- **Manifest:** `addons/spreadsheet/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Spreadsheet

Spreadsheet

Declared dependencies: `bus`, `web`, `portal`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 24 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 7 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 13 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 152 | Client behavior/assets. |
| Tests | 8 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "bus",
    "web",
    "portal"
  ],
  "data": [
    "views/public_readonly_spreadsheet_templates.xml"
  ],
  "assets": {
    "web.chartjs_lib": [
      "spreadsheet/static/lib/chartjs-chart-geo/chartjs-chart-geo.js",
      "spreadsheet/static/lib/chart_js_treemap.js"
    ],
    "spreadsheet.o_spreadsheet_core": [
      "web/static/src/views/graph/graph_model.js",
      "web/static/src/views/pivot/pivot_model.js",
      "web/static/src/polyfills/clipboard.js",
      [
        "include",
        "web.chartjs_lib"
      ],
      "spreadsheet/static/src/o_spreadsheet/o_spreadsheet.js",
      "spreadsheet/static/src/**/*.js",
      "spreadsheet/static/src/o_spreadsheet/o_spreadsheet.xml",
      "spreadsheet/static/src/**/*.xml",
      [
        "remove",
        "spreadsheet/static/src/assets_backend/**/*"
      ],
      [
        "remove",
        "spreadsheet/static/src/public_spreadsheet/**/*"
      ]
    ],
    "spreadsheet.o_spreadsheet": [
      [
        "include",
        "spreadsheet.o_spreadsheet_core"
      ]
    ],
    "spreadsheet.public_spreadsheet": [
      [
        "include",
        "web.assets_frontend"
      ],
      [
        "include",
        "spreadsheet.o_spreadsheet_core"
      ],
      "web/static/src/model/**/*.js",
      "web/static/src/views/**/*.js",
      "web/static/src/search/**/*.js",
      "web/static/src/core/commands/command_hook.js",
      "web/static/src/webclient/menus/menu_helpers.js",
      [
        "remove",
        "spreadsheet/static/src/ir_ui_menu/spreadsheet_link_service.js"
      ],
      [
        "remove",
        "spreadsheet/static/src/chart/odoo_link/components/*"
      ],
      "spreadsheet/static/src/o_spreadsheet/o_spreadsheet.css",
      "spreadsheet/static/src/**/*.scss",
      "spreadsheet/static/src/public_spreadsheet/**/*"
    ],
    "web.assets_backend": [
      "spreadsheet/static/src/o_spreadsheet/o_spreadsheet.css",
      "spreadsheet/static/src/**/*.scss",
      "spreadsheet/static/src/assets_backend/**/*"
    ],
    "web.assets_unit_tests": [
      "spreadsheet/static/tests/**/*",
      [
        "include",
        "spreadsheet.o_spreadsheet"
      ]
    ]
  }
}
```

### Representative source files

- `addons/spreadsheet/__init__.py` (4 lines)
- `addons/spreadsheet/__manifest__.py` (58 lines)
- `addons/spreadsheet/controllers/__init__.py` (3 lines)
- `addons/spreadsheet/controllers/main.py` (45 lines)
- `addons/spreadsheet/i18n/ar.po` (15,784 lines)
- `addons/spreadsheet/i18n/az.po` (15,416 lines)
- `addons/spreadsheet/i18n/bg.po` (15,417 lines)
- `addons/spreadsheet/i18n/bs.po` (15,413 lines)
- `addons/spreadsheet/i18n/ca.po` (15,453 lines)
- `addons/spreadsheet/i18n/cs.po` (15,443 lines)
- `addons/spreadsheet/i18n/da.po` (15,443 lines)
- `addons/spreadsheet/i18n/de.po` (16,273 lines)
- `addons/spreadsheet/i18n/el.po` (15,417 lines)
- `addons/spreadsheet/i18n/es.po` (16,039 lines)
- `addons/spreadsheet/i18n/es_419.po` (16,111 lines)
- `addons/spreadsheet/i18n/et.po` (15,422 lines)
- `addons/spreadsheet/i18n/fa.po` (15,443 lines)
- `addons/spreadsheet/i18n/fi.po` (15,934 lines)
- `addons/spreadsheet/i18n/fr.po` (16,179 lines)
- `addons/spreadsheet/i18n/he.po` (15,421 lines)
- `addons/spreadsheet/i18n/hi.po` (15,416 lines)
- `addons/spreadsheet/i18n/hr.po` (15,441 lines)
- `addons/spreadsheet/i18n/hu.po` (15,417 lines)
- `addons/spreadsheet/i18n/id.po` (15,935 lines)
- `addons/spreadsheet/i18n/it.po` (16,132 lines)
- `addons/spreadsheet/i18n/ja.po` (15,597 lines)
- `addons/spreadsheet/i18n/kab.po` (15,412 lines)
- `addons/spreadsheet/i18n/ko.po` (15,500 lines)
- `addons/spreadsheet/i18n/ku.po` (15,413 lines)
- `addons/spreadsheet/i18n/lo.po` (15,601 lines)
- `addons/spreadsheet/i18n/lt.po` (15,418 lines)
- `addons/spreadsheet/i18n/lv.po` (15,412 lines)
- `addons/spreadsheet/i18n/mn.po` (15,417 lines)
- `addons/spreadsheet/i18n/my.po` (15,418 lines)
- `addons/spreadsheet/i18n/nb.po` (15,420 lines)
- `addons/spreadsheet/i18n/nl.po` (16,210 lines)
- `addons/spreadsheet/i18n/pl.po` (15,506 lines)
- `addons/spreadsheet/i18n/pt.po` (15,507 lines)
- `addons/spreadsheet/i18n/pt_BR.po` (16,114 lines)
- `addons/spreadsheet/i18n/ro.po` (15,509 lines)
- `addons/spreadsheet/i18n/ru.po` (15,718 lines)
- `addons/spreadsheet/i18n/sk.po` (15,415 lines)
- `addons/spreadsheet/i18n/sl.po` (15,422 lines)
- `addons/spreadsheet/i18n/spreadsheet.pot` (15,426 lines)
- `addons/spreadsheet/i18n/sr@latin.po` (15,418 lines)
- `addons/spreadsheet/i18n/sv.po` (15,493 lines)
- `addons/spreadsheet/i18n/th.po` (15,469 lines)
- `addons/spreadsheet/i18n/tr.po` (15,894 lines)
- `addons/spreadsheet/i18n/uk.po` (15,444 lines)
- `addons/spreadsheet/i18n/uz.po` (17,981 lines)
- `addons/spreadsheet/i18n/vi.po` (15,852 lines)
- `addons/spreadsheet/i18n/zh_CN.po` (15,627 lines)
- `addons/spreadsheet/i18n/zh_TW.po` (16,844 lines)
- `addons/spreadsheet/models/__init__.py` (8 lines)
- `addons/spreadsheet/models/ir_http.py` (16 lines)
- `addons/spreadsheet/models/ir_model.py` (21 lines)
- `addons/spreadsheet/models/res_currency.py` (27 lines)
- `addons/spreadsheet/models/res_currency_rate.py` (39 lines)
- `addons/spreadsheet/models/res_lang.py` (41 lines)
- `addons/spreadsheet/models/spreadsheet_mixin.py` (171 lines)
- `addons/spreadsheet/static/description/icon.png` (6 lines)
- `addons/spreadsheet/static/description/icon.svg` (1 lines)
- `addons/spreadsheet/static/description/icon_hi.png` (19 lines)
- `addons/spreadsheet/static/img/spreadsheet.svg` (1 lines)
- `addons/spreadsheet/static/lib/chart_js_treemap.js` (1,298 lines)
- `addons/spreadsheet/static/lib/chartjs-chart-geo/chartjs-chart-geo.js` (5,322 lines)
- `addons/spreadsheet/static/src/@types/commands.d.ts` (203 lines)
- `addons/spreadsheet/static/src/@types/env.d.ts` (11 lines)
- `addons/spreadsheet/static/src/@types/functions.d.ts` (11 lines)
- `addons/spreadsheet/static/src/@types/getters.d.ts` (74 lines)
- `addons/spreadsheet/static/src/@types/global_filter.d.ts` (175 lines)
- `addons/spreadsheet/static/src/@types/misc.d.ts` (10 lines)
- `addons/spreadsheet/static/src/@types/models.d.ts` (16 lines)
- `addons/spreadsheet/static/src/@types/pivot.d.ts` (75 lines)
- `addons/spreadsheet/static/src/@types/plugins.d.ts` (29 lines)
- `addons/spreadsheet/static/src/actions/helpers.js` (58 lines)
- `addons/spreadsheet/static/src/actions/spreadsheet_component.js` (33 lines)
- `addons/spreadsheet/static/src/actions/spreadsheet_component.scss` (5 lines)
- `addons/spreadsheet/static/src/actions/spreadsheet_component.xml` (6 lines)
- `addons/spreadsheet/static/src/actions/spreadsheet_download_action.js` (48 lines)
- `addons/spreadsheet/static/src/assets_backend/spreadsheet_action_loader.js` (51 lines)
- `addons/spreadsheet/static/src/assets_backend/spreadsheet_binary_field/spreadsheet_binary_field.js` (19 lines)
- `addons/spreadsheet/static/src/assets_backend/spreadsheet_binary_field/spreadsheet_binary_field.xml` (9 lines)
- `addons/spreadsheet/static/src/chart/data_source/chart_data_source.js` (176 lines)
- `addons/spreadsheet/static/src/chart/index.js` (14 lines)
- `addons/spreadsheet/static/src/chart/odoo_chart/odoo_chart_datasource.js` (119 lines)
- `addons/spreadsheet/static/src/chart/odoo_chart/odoo_chart_helpers.js` (245 lines)
- `addons/spreadsheet/static/src/chart/odoo_chart/odoo_chart_zoomable_component.js` (14 lines)
- `addons/spreadsheet/static/src/chart/odoo_chart/odoo_dataset_styles.js` (54 lines)
- `addons/spreadsheet/static/src/chart/odoo_link/chartjs/odoo_link_chartjs_plugin.js` (22 lines)
- `addons/spreadsheet/static/src/chart/odoo_link/components/chart_menu.js` (25 lines)
- `addons/spreadsheet/static/src/chart/odoo_link/components/figure_component.js` (156 lines)
- `addons/spreadsheet/static/src/chart/odoo_link/components/figure_component.xml` (16 lines)
- `addons/spreadsheet/static/src/chart/plugins/chart_odoo_link_plugin.js` (175 lines)
- `addons/spreadsheet/static/src/chart/plugins/odoo_chart_core_plugin.js` (239 lines)
- `addons/spreadsheet/static/src/chart/plugins/odoo_chart_core_view_plugin.js` (219 lines)
- `addons/spreadsheet/static/src/chart/plugins/odoo_chart_feature_plugin.js` (126 lines)
- `addons/spreadsheet/static/src/chart/plugins/operational_transform.js` (47 lines)
- `addons/spreadsheet/static/src/command_palette.js` (13 lines)
- `addons/spreadsheet/static/src/command_provider.js` (88 lines)
- `addons/spreadsheet/static/src/components/share_button/share_button.js` (78 lines)
- `addons/spreadsheet/static/src/components/share_button/share_button.scss` (18 lines)
- `addons/spreadsheet/static/src/components/share_button/share_button.xml` (39 lines)
- `addons/spreadsheet/static/src/currency/formulas.js` (30 lines)
- `addons/spreadsheet/static/src/currency/helpers.js` (40 lines)
- `addons/spreadsheet/static/src/currency/plugins/currency.js` (72 lines)
- `addons/spreadsheet/static/src/data_sources/data_source.js` (186 lines)
- `addons/spreadsheet/static/src/data_sources/data_source_link.js` (74 lines)
- `addons/spreadsheet/static/src/data_sources/odoo_data_provider.js` (55 lines)
- `addons/spreadsheet/static/src/data_sources/odoo_views_data_source.js` (167 lines)
- `addons/spreadsheet/static/src/data_sources/server_data.js` (318 lines)
- `addons/spreadsheet/static/src/global_filters/components/date_filter_dropdown/date_filter_dropdown.js` (174 lines)
- `addons/spreadsheet/static/src/global_filters/components/date_filter_dropdown/date_filter_dropdown.xml` (30 lines)
- `addons/spreadsheet/static/src/global_filters/components/date_filter_value/date_filter_value.js` (32 lines)
- `addons/spreadsheet/static/src/global_filters/components/date_filter_value/date_filter_value.scss` (52 lines)
- `addons/spreadsheet/static/src/global_filters/components/date_filter_value/date_filter_value.xml` (20 lines)
- `addons/spreadsheet/static/src/global_filters/components/default_date_value/default_date_value.js` (47 lines)
- `addons/spreadsheet/static/src/global_filters/components/default_date_value/default_date_value.xml` (18 lines)
- `addons/spreadsheet/static/src/global_filters/components/filter_text_value/filter_text_value.js` (77 lines)
- `addons/spreadsheet/static/src/global_filters/components/filter_text_value/filter_text_value.xml` (17 lines)
- `addons/spreadsheet/static/src/global_filters/components/filter_value/filter_value.js` (201 lines)
- `addons/spreadsheet/static/src/global_filters/components/filter_value/filter_value.scss` (27 lines)
- `addons/spreadsheet/static/src/global_filters/components/filter_value/filter_value.xml` (72 lines)
- `addons/spreadsheet/static/src/global_filters/components/selection_filter_value/selection_filter_value.js` (75 lines)
- `addons/spreadsheet/static/src/global_filters/components/selection_filter_value/selection_filter_value.xml` (11 lines)
- `addons/spreadsheet/static/src/global_filters/helpers.js` (1,127 lines)
- `addons/spreadsheet/static/src/global_filters/index.js` (73 lines)
- `addons/spreadsheet/static/src/global_filters/plugins/global_filters_core_plugin.js` (349 lines)
- `addons/spreadsheet/static/src/global_filters/plugins/global_filters_core_view_plugin.js` (339 lines)
- `addons/spreadsheet/static/src/global_filters/plugins/global_filters_ui_plugin.js` (142 lines)
- `addons/spreadsheet/static/src/helpers/constants.js` (7 lines)
- `addons/spreadsheet/static/src/helpers/geo_json_service.js` (168 lines)
- `addons/spreadsheet/static/src/helpers/helpers.js` (85 lines)
- `addons/spreadsheet/static/src/helpers/model.js` (356 lines)
- `addons/spreadsheet/static/src/helpers/neutralized_link.js` (33 lines)
- `addons/spreadsheet/static/src/helpers/odoo_functions_helpers.js` (23 lines)
- `addons/spreadsheet/static/src/hooks.js` (69 lines)
- `addons/spreadsheet/static/src/index.js` (141 lines)
- `addons/spreadsheet/static/src/ir_ui_menu/index.js` (7 lines)
- `addons/spreadsheet/static/src/ir_ui_menu/ir_ui_menu_plugin.js` (26 lines)
- `addons/spreadsheet/static/src/ir_ui_menu/odoo_menu_link_cell.js` (103 lines)
- `addons/spreadsheet/static/src/ir_ui_menu/spreadsheet_link_service.js` (131 lines)
- `addons/spreadsheet/static/src/list/index.js` (75 lines)
- `addons/spreadsheet/static/src/list/list_actions.js` (91 lines)
- `addons/spreadsheet/static/src/list/list_data_source.js` (525 lines)
- `addons/spreadsheet/static/src/list/list_functions.js` (102 lines)
- `addons/spreadsheet/static/src/list/list_helpers.js` (55 lines)
- `addons/spreadsheet/static/src/list/plugins/list_core_global_filter_plugin.js` (149 lines)
- `addons/spreadsheet/static/src/list/plugins/list_core_plugin.js` (487 lines)
- `addons/spreadsheet/static/src/list/plugins/list_core_view_plugin.js` (596 lines)
- `addons/spreadsheet/static/src/list/plugins/list_ui_plugin.js` (157 lines)
- `addons/spreadsheet/static/src/logging/logging_ui_plugin.js` (93 lines)
- `addons/spreadsheet/static/src/model.js` (7 lines)
- `addons/spreadsheet/static/src/o_spreadsheet/cancelled_reason.js` (22 lines)
- `addons/spreadsheet/static/src/o_spreadsheet/errors.js` (19 lines)
- `addons/spreadsheet/static/src/o_spreadsheet/icons.xml` (17 lines)
- `addons/spreadsheet/static/src/o_spreadsheet/init_callbacks.js` (3 lines)
- `addons/spreadsheet/static/src/o_spreadsheet/migration.js` (643 lines)
- `addons/spreadsheet/static/src/o_spreadsheet/o_spreadsheet.css` (3,802 lines)
- `addons/spreadsheet/static/src/o_spreadsheet/o_spreadsheet.js` (91,107 lines)

Additional files not expanded here: 97. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
