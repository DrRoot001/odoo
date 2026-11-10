# Module: html_builder

- **Module ID:** MOD-105
- **Path:** `addons/html_builder`
- **Manifest:** `addons/html_builder/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Generic html builder


    This addon contains a generic html builder application. It is designed to be
    used by the website builder and mass mailing editor.
    

Declared dependencies: `html_editor`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 81 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 214 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "html_editor"
  ],
  "assets": {
    "web._assets_primary_variables": [
      "html_builder/static/src/**/*.variables.scss"
    ],
    "web.assets_backend": [
      "html_builder/static/src/utils/keyboard_navigation.js"
    ],
    "html_builder.assets": [
      [
        "include",
        "web._assets_helpers"
      ],
      "html_editor/static/src/scss/bootstrap_overridden.scss",
      "web/static/src/scss/pre_variables.scss",
      "web/static/lib/bootstrap/scss/_variables.scss",
      "web/static/lib/bootstrap/scss/_variables-dark.scss",
      "web/static/lib/bootstrap/scss/_maps.scss",
      "web/static/fonts/fonts.scss",
      "html_builder/static/src/**/*",
      [
        "remove",
        "html_builder/static/src/**/*.edit.*"
      ],
      [
        "remove",
        "html_builder/static/src/**/*.dark.scss"
      ]
    ],
    "web.assets_frontend": [
      "html_builder/static/src/scss/background.scss"
    ],
    "web.assets_web_dark": [
      "html_builder/static/src/**/*.dark.scss"
    ],
    "html_builder.assets_inside_builder_iframe": [
      [
        "include",
        "web._assets_helpers"
      ],
      "web/static/src/scss/bootstrap_overridden.scss",
      "html_builder/static/src/**/*.edit.*",
      "html_editor/static/src/main/translate/translate_plugin.scss",
      "html_editor/static/src/main/link/link.scss"
    ],
    "html_builder.iframe_add_dialog": [
      [
        "include",
        "web._assets_helpers"
      ],
      [
        "include",
        "web._assets_frontend_helpers"
      ],
      "web/static/src/scss/pre_variables.scss",
      "web/static/lib/bootstrap/scss/_variables.scss",
      "web/static/lib/bootstrap/scss/_variables-dark.scss",
      "web/static/lib/bootstrap/scss/_maps.scss",
      "html_builder/static/src/snippets/snippet_viewer.scss"
    ],
    "web.assets_unit_tests": [
      "html_builder/static/tests/**/*",
      [
        "include",
        "html_builder.assets"
      ]
    ]
  }
}
```

### Representative source files

- `addons/html_builder/__init__.py` (1 lines)
- `addons/html_builder/__manifest__.py` (63 lines)
- `addons/html_builder/i18n/af.po` (3,743 lines)
- `addons/html_builder/i18n/ar.po` (3,909 lines)
- `addons/html_builder/i18n/az.po` (3,902 lines)
- `addons/html_builder/i18n/bg.po` (3,899 lines)
- `addons/html_builder/i18n/bs.po` (3,894 lines)
- `addons/html_builder/i18n/ca.po` (3,906 lines)
- `addons/html_builder/i18n/cs.po` (3,902 lines)
- `addons/html_builder/i18n/da.po` (3,904 lines)
- `addons/html_builder/i18n/de.po` (3,934 lines)
- `addons/html_builder/i18n/el.po` (3,895 lines)
- `addons/html_builder/i18n/es.po` (3,922 lines)
- `addons/html_builder/i18n/es_419.po` (3,928 lines)
- `addons/html_builder/i18n/es_CL.po` (52 lines)
- `addons/html_builder/i18n/et.po` (3,898 lines)
- `addons/html_builder/i18n/fa.po` (3,904 lines)
- `addons/html_builder/i18n/fi.po` (3,916 lines)
- `addons/html_builder/i18n/fr.po` (3,928 lines)
- `addons/html_builder/i18n/fr_CA.po` (25 lines)
- `addons/html_builder/i18n/gl.po` (3,743 lines)
- `addons/html_builder/i18n/gu.po` (3,743 lines)
- `addons/html_builder/i18n/he.po` (3,900 lines)
- `addons/html_builder/i18n/hi.po` (3,897 lines)
- `addons/html_builder/i18n/hr.po` (3,896 lines)
- `addons/html_builder/i18n/html_builder.pot` (3,889 lines)
- `addons/html_builder/i18n/hu.po` (3,901 lines)
- `addons/html_builder/i18n/id.po` (3,917 lines)
- `addons/html_builder/i18n/is.po` (3,743 lines)
- `addons/html_builder/i18n/it.po` (3,929 lines)
- `addons/html_builder/i18n/ja.po` (3,916 lines)
- `addons/html_builder/i18n/ka.po` (3,743 lines)
- `addons/html_builder/i18n/kab.po` (3,893 lines)
- `addons/html_builder/i18n/km.po` (3,743 lines)
- `addons/html_builder/i18n/ko.po` (3,901 lines)
- `addons/html_builder/i18n/ku.po` (3,895 lines)
- `addons/html_builder/i18n/lo.po` (3,908 lines)
- `addons/html_builder/i18n/lt.po` (3,901 lines)
- `addons/html_builder/i18n/lv.po` (3,893 lines)
- `addons/html_builder/i18n/mk.po` (3,747 lines)
- `addons/html_builder/i18n/mn.po` (3,895 lines)
- `addons/html_builder/i18n/my.po` (3,894 lines)
- `addons/html_builder/i18n/nb.po` (3,898 lines)
- `addons/html_builder/i18n/nl.po` (3,926 lines)
- `addons/html_builder/i18n/pl.po` (3,922 lines)
- `addons/html_builder/i18n/pt.po` (3,909 lines)
- `addons/html_builder/i18n/pt_BR.po` (3,929 lines)
- `addons/html_builder/i18n/ro.po` (3,917 lines)
- `addons/html_builder/i18n/ru.po` (3,916 lines)
- `addons/html_builder/i18n/sk.po` (3,894 lines)
- `addons/html_builder/i18n/sl.po` (3,901 lines)
- `addons/html_builder/i18n/sr@latin.po` (3,896 lines)
- `addons/html_builder/i18n/sv.po` (3,903 lines)
- `addons/html_builder/i18n/th.po` (3,904 lines)
- `addons/html_builder/i18n/tr.po` (3,913 lines)
- `addons/html_builder/i18n/uk.po` (3,905 lines)
- `addons/html_builder/i18n/uz.po` (4,395 lines)
- `addons/html_builder/i18n/vi.po` (3,906 lines)
- `addons/html_builder/i18n/zh_CN.po` (3,912 lines)
- `addons/html_builder/i18n/zh_TW.po` (3,909 lines)
- `addons/html_builder/models/__init__.py` (2 lines)
- `addons/html_builder/models/ir_qweb.py` (151 lines)
- `addons/html_builder/models/ir_ui_view.py` (199 lines)
- `addons/html_builder/static/image_shapes/brushed/brush_1.svg` (15 lines)
- `addons/html_builder/static/image_shapes/brushed/brush_2.svg` (15 lines)
- `addons/html_builder/static/image_shapes/brushed/brush_3.svg` (15 lines)
- `addons/html_builder/static/image_shapes/brushed/brush_4.svg` (15 lines)
- `addons/html_builder/static/image_shapes/composite/composite_cut_circle.svg` (15 lines)
- `addons/html_builder/static/image_shapes/composite/composite_double_pill.svg` (15 lines)
- `addons/html_builder/static/image_shapes/composite/composite_half_circle.svg` (15 lines)
- `addons/html_builder/static/image_shapes/composite/composite_sonar.svg` (15 lines)
- `addons/html_builder/static/image_shapes/composite/composite_triple_pill.svg` (15 lines)
- `addons/html_builder/static/image_shapes/composition/composition_line_1.svg` (33 lines)
- `addons/html_builder/static/image_shapes/composition/composition_line_2.svg` (42 lines)
- `addons/html_builder/static/image_shapes/composition/composition_line_3.svg` (40 lines)
- `addons/html_builder/static/image_shapes/composition/composition_mixed_1.svg` (51 lines)
- `addons/html_builder/static/image_shapes/composition/composition_mixed_2.svg` (65 lines)
- `addons/html_builder/static/image_shapes/composition/composition_organic_line.svg` (19 lines)
- `addons/html_builder/static/image_shapes/composition/composition_oval_line.svg` (20 lines)
- `addons/html_builder/static/image_shapes/composition/composition_planet_1.svg` (108 lines)
- `addons/html_builder/static/image_shapes/composition/composition_planet_2.svg` (108 lines)
- `addons/html_builder/static/image_shapes/composition/composition_square_1.svg` (63 lines)
- `addons/html_builder/static/image_shapes/composition/composition_square_2.svg` (52 lines)
- `addons/html_builder/static/image_shapes/composition/composition_square_3.svg` (59 lines)
- `addons/html_builder/static/image_shapes/composition/composition_square_4.svg` (71 lines)
- `addons/html_builder/static/image_shapes/composition/composition_square_line.svg` (34 lines)
- `addons/html_builder/static/image_shapes/composition/composition_triangle_line.svg` (60 lines)
- `addons/html_builder/static/image_shapes/convert-to-percentages.html` (17 lines)
- `addons/html_builder/static/image_shapes/convert-to-percentages.js` (175 lines)
- `addons/html_builder/static/image_shapes/devices/browser_01.svg` (22 lines)
- `addons/html_builder/static/image_shapes/devices/browser_02.svg` (59 lines)
- `addons/html_builder/static/image_shapes/devices/browser_03.svg` (52 lines)
- `addons/html_builder/static/image_shapes/devices/galaxy_3d_landscape_01.svg` (76 lines)
- `addons/html_builder/static/image_shapes/devices/galaxy_3d_landscape_02.svg` (86 lines)
- `addons/html_builder/static/image_shapes/devices/galaxy_3d_portrait_01.svg` (73 lines)
- `addons/html_builder/static/image_shapes/devices/galaxy_3d_portrait_02.svg` (96 lines)
- `addons/html_builder/static/image_shapes/devices/galaxy_front_landscape.svg` (55 lines)
- `addons/html_builder/static/image_shapes/devices/galaxy_front_portrait.svg` (55 lines)
- `addons/html_builder/static/image_shapes/devices/galaxy_front_portrait_half.svg` (54 lines)
- `addons/html_builder/static/image_shapes/devices/imac_3d_01.svg` (78 lines)
- `addons/html_builder/static/image_shapes/devices/imac_3d_02.svg` (78 lines)
- `addons/html_builder/static/image_shapes/devices/imac_front.svg` (87 lines)
- `addons/html_builder/static/image_shapes/devices/ipad_3d_landscape_01.svg` (294 lines)
- `addons/html_builder/static/image_shapes/devices/ipad_3d_landscape_02.svg` (278 lines)
- `addons/html_builder/static/image_shapes/devices/ipad_3d_portrait_01.svg` (281 lines)
- `addons/html_builder/static/image_shapes/devices/ipad_3d_portrait_02.svg` (289 lines)
- `addons/html_builder/static/image_shapes/devices/ipad_front_landscape.svg` (58 lines)
- `addons/html_builder/static/image_shapes/devices/ipad_front_portrait.svg` (58 lines)
- `addons/html_builder/static/image_shapes/devices/iphone_3d_landscape_01.svg` (157 lines)
- `addons/html_builder/static/image_shapes/devices/iphone_3d_landscape_02.svg` (150 lines)
- `addons/html_builder/static/image_shapes/devices/iphone_3d_portrait_01.svg` (132 lines)
- `addons/html_builder/static/image_shapes/devices/iphone_3d_portrait_02.svg` (129 lines)
- `addons/html_builder/static/image_shapes/devices/iphone_front_landscape.svg` (71 lines)
- `addons/html_builder/static/image_shapes/devices/iphone_front_portrait.svg` (71 lines)
- `addons/html_builder/static/image_shapes/devices/iphone_front_portrait_half.svg` (68 lines)
- `addons/html_builder/static/image_shapes/devices/macbook_3d_01.svg` (178 lines)
- `addons/html_builder/static/image_shapes/devices/macbook_3d_02.svg` (160 lines)
- `addons/html_builder/static/image_shapes/devices/macbook_front.svg` (100 lines)
- `addons/html_builder/static/image_shapes/devices/macbook_front_half.svg` (34 lines)
- `addons/html_builder/static/image_shapes/geometric/geo_cornered_triangle.svg` (14 lines)
- `addons/html_builder/static/image_shapes/geometric/geo_diamond.svg` (15 lines)
- `addons/html_builder/static/image_shapes/geometric/geo_door.svg` (15 lines)
- `addons/html_builder/static/image_shapes/geometric/geo_emerald.svg` (15 lines)
- `addons/html_builder/static/image_shapes/geometric/geo_gem.svg` (15 lines)
- `addons/html_builder/static/image_shapes/geometric/geo_heptagon.svg` (15 lines)
- `addons/html_builder/static/image_shapes/geometric/geo_hexagon.svg` (15 lines)
- `addons/html_builder/static/image_shapes/geometric/geo_kayak.svg` (15 lines)
- `addons/html_builder/static/image_shapes/geometric/geo_pentagon.svg` (15 lines)
- `addons/html_builder/static/image_shapes/geometric/geo_shuriken.svg` (15 lines)
- `addons/html_builder/static/image_shapes/geometric/geo_slanted.svg` (12 lines)
- `addons/html_builder/static/image_shapes/geometric/geo_sonar.svg` (15 lines)
- `addons/html_builder/static/image_shapes/geometric/geo_square.svg` (15 lines)
- `addons/html_builder/static/image_shapes/geometric/geo_square_1.svg` (23 lines)
- `addons/html_builder/static/image_shapes/geometric/geo_square_2.svg` (23 lines)
- `addons/html_builder/static/image_shapes/geometric/geo_square_3.svg` (24 lines)
- `addons/html_builder/static/image_shapes/geometric/geo_square_4.svg` (23 lines)
- `addons/html_builder/static/image_shapes/geometric/geo_square_5.svg` (22 lines)
- `addons/html_builder/static/image_shapes/geometric/geo_square_6.svg` (22 lines)
- `addons/html_builder/static/image_shapes/geometric/geo_star.svg` (15 lines)
- `addons/html_builder/static/image_shapes/geometric/geo_star_16pin.svg` (15 lines)
- `addons/html_builder/static/image_shapes/geometric/geo_star_8pin.svg` (15 lines)
- `addons/html_builder/static/image_shapes/geometric/geo_tear.svg` (15 lines)
- `addons/html_builder/static/image_shapes/geometric/geo_tetris.svg` (15 lines)
- `addons/html_builder/static/image_shapes/geometric/geo_triangle.svg` (15 lines)
- `addons/html_builder/static/image_shapes/geometric/geo_triangle_corner.svg` (13 lines)
- `addons/html_builder/static/image_shapes/geometric_round/geo_round_blob_hard.svg` (25 lines)
- `addons/html_builder/static/image_shapes/geometric_round/geo_round_blob_medium.svg` (25 lines)
- `addons/html_builder/static/image_shapes/geometric_round/geo_round_blob_soft.svg` (23 lines)
- `addons/html_builder/static/image_shapes/geometric_round/geo_round_bread.svg` (15 lines)
- `addons/html_builder/static/image_shapes/geometric_round/geo_round_circle.svg` (14 lines)
- `addons/html_builder/static/image_shapes/geometric_round/geo_round_clover.svg` (15 lines)
- `addons/html_builder/static/image_shapes/geometric_round/geo_round_cornered.svg` (15 lines)
- `addons/html_builder/static/image_shapes/geometric_round/geo_round_diamond.svg` (15 lines)
- `addons/html_builder/static/image_shapes/geometric_round/geo_round_door.svg` (15 lines)
- `addons/html_builder/static/image_shapes/geometric_round/geo_round_emerald.svg` (15 lines)
- `addons/html_builder/static/image_shapes/geometric_round/geo_round_gem.svg` (15 lines)
- `addons/html_builder/static/image_shapes/geometric_round/geo_round_heptagon.svg` (15 lines)
- `addons/html_builder/static/image_shapes/geometric_round/geo_round_hexagon.svg` (15 lines)
- `addons/html_builder/static/image_shapes/geometric_round/geo_round_lemon.svg` (15 lines)
- `addons/html_builder/static/image_shapes/geometric_round/geo_round_pentagon.svg` (15 lines)

Additional files not expanded here: 708. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
