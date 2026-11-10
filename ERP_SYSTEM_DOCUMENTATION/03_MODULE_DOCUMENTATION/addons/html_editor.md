# Module: html_editor

- **Module ID:** MOD-106
- **Path:** `addons/html_editor`
- **Manifest:** `addons/html_editor/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

A Html Editor component and plugin system.


Html Editor
==========================
This addon provides an extensible, maintainable editor.
    

Declared dependencies: `base`, `bus`, `web`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 26 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 10 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 75 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 395 | Client behavior/assets. |
| Tests | 11 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 17 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base",
    "bus",
    "web"
  ],
  "data": [
    "security/ir.access.csv"
  ],
  "assets": {
    "web._assets_primary_variables": [
      [
        "after",
        "web/static/src/scss/primary_variables.scss",
        "html_editor/static/src/scss/html_editor.variables.scss"
      ]
    ],
    "web.assets_frontend_minimal": [
      "html_editor/static/src/main/media/video/abstract_third_party_video.js",
      "html_editor/static/src/main/media/video/providers/**/*",
      "html_editor/static/src/main/media/video/utils.js"
    ],
    "web.assets_frontend": [
      [
        "include",
        "html_editor.assets_media_dialog"
      ],
      [
        "include",
        "html_editor.assets_readonly"
      ],
      "html_editor/static/src/public/**/*",
      "html_editor/static/src/scss/html_editor.common.scss",
      "html_editor/static/src/scss/html_editor.frontend.scss",
      "html_editor/static/src/scss/base_style.scss",
      "html_editor/static/src/main/selection_placeholder_plugin.scss"
    ],
    "web.assets_backend": [
      [
        "include",
        "html_editor.assets_editor"
      ],
      "html_editor/static/src/backend/**/*",
      "html_editor/static/src/fields/**/*",
      "html_editor/static/lib/vkbeautify/**/*",
      "html_editor/static/src/scss/base_style.scss",
      "html_editor/static/src/scss/html_editor.common.scss",
      "html_editor/static/src/scss/html_editor.backend.scss"
    ],
    "html_editor.assets_editor": [
      "web/static/lib/dompurify/DOMpurify.js",
      [
        "include",
        "html_editor.assets_media_dialog"
      ],
      [
        "include",
        "html_editor.assets_readonly"
      ],
      "html_editor/static/src/*",
      "html_editor/static/src/components/color_picker/**/*",
      "html_editor/static/src/components/history_dialog/**/*",
      "html_editor/static/src/components/iframe_input/**/*",
      "html_editor/static/src/components/suggestion/**/*",
      "html_editor/static/src/core/**/*",
      "html_editor/static/src/main/**/*",
      "html_editor/static/src/others/collaboration/**/*",
      "html_editor/static/src/others/embedded_components/**/*",
      "html_editor/static/src/others/embedded_component*",
      "html_editor/static/src/others/qweb_picker*",
      "html_editor/static/src/others/qweb_plugin*",
      "html_editor/static/src/others/autofocus_plugin*",
      "html_editor/static/src/services/**/*",
      [
        "remove",
        "html_editor/static/src/**/*.dark.scss"
      ]
    ],
    "html_editor.assets_history_diff": [
      "html_editor/static/lib/diff2html/diff2html.min.css",
      "html_editor/static/lib/diff2html/diff2html.min.js"
    ],
    "html_editor.assets_media_dialog": [
      "html_editor/static/src/components/switch/**/*",
      "html_editor/static/src/main/media/media_dialog/**/*"
    ],
    "html_editor.assets_readonly": [
      "html_editor/static/src/components/html_viewer/**/*",
      "html_editor/static/src/local_overlay_container.*",
      "html_editor/static/src/main/local_overlay.scss",
      "html_editor/static/src/position_hook.*",
      "html_editor/static/src/html_migrations/**/*",
      "html_editor/static/src/main/list/list.scss",
      "html_editor/static/src/main/media/file.scss",
      "html_editor/static/src/others/embedded_component_utils.js",
      "html_editor/static/src/others/embedded_components/core/**/*",
      "html_editor/static/src/utils/**/*",
      "html_editor/static/src/others/qweb_plugin.scss"
    ],
    "web.assets_web_dark": [
      "html_editor/static/src/**/*.dark.scss"
    ],
    "web.assets_tests": [
      "html_editor/static/tests/tours/**/*"
    ],
    "web.assets_unit_tests": [
      "html_editor/static/tests/**/*"
    ],
    "web.assets_unit_tests_setup": [
      "html_editor/static/src/public/**/*"
    ],
    "html_editor.assets_image_cropper": [
      "html_editor/static/lib/cropperjs/cropper.css",
      "html_editor/static/lib/cropperjs/cropper.js",
      "html_editor/static/lib/webgl-image-filter/webgl-image-filter.js"
    ],
    "web.report_assets_common": [
      "html_editor/static/src/scss/base_style.scss",
      "html_editor/static/src/scss/bootstrap_overridden.scss",
      "html_editor/static/src/scss/html_editor.common.scss"
    ],
    "web._assets_secondary_variables": [
      "html_editor/static/src/scss/secondary_variables.scss"
    ],
    "web._assets_backend_helpers": [
      "html_editor/static/src/scss/bootstrap_overridden_backend.scss",
      "html_editor/static/src/scss/bootstrap_overridden.scss"
    ],
    "web._assets_frontend_helpers": [
      [
        "prepend",
        "html_editor/static/src/scss/bootstrap_overridden.scss"
      ]
    ],
    "html_editor.assets_prism": [
      "web/static/lib/prismjs/prism.js",
      "web/static/lib/prismjs/themes/default.css"
    ],
    "html_editor.assets_prism_dark": [
      "web/static/lib/prismjs/prism.js",
      "web/static/lib/prismjs/themes/okaida.css"
    ]
  }
}
```

### Representative source files

- `addons/html_editor/__init__.py` (2 lines)
- `addons/html_editor/__manifest__.py` (128 lines)
- `addons/html_editor/controllers/__init__.py` (3 lines)
- `addons/html_editor/controllers/main.py` (834 lines)
- `addons/html_editor/controllers/svg_utils.py` (100 lines)
- `addons/html_editor/i18n/ar.po` (3,050 lines)
- `addons/html_editor/i18n/az.po` (3,015 lines)
- `addons/html_editor/i18n/bg.po` (2,989 lines)
- `addons/html_editor/i18n/bs.po` (2,968 lines)
- `addons/html_editor/i18n/ca.po` (3,022 lines)
- `addons/html_editor/i18n/cs.po` (3,016 lines)
- `addons/html_editor/i18n/da.po` (3,020 lines)
- `addons/html_editor/i18n/de.po` (3,097 lines)
- `addons/html_editor/i18n/el.po` (2,978 lines)
- `addons/html_editor/i18n/es.po` (3,068 lines)
- `addons/html_editor/i18n/es_419.po` (3,080 lines)
- `addons/html_editor/i18n/et.po` (3,005 lines)
- `addons/html_editor/i18n/fa.po` (3,020 lines)
- `addons/html_editor/i18n/fi.po` (3,057 lines)
- `addons/html_editor/i18n/fr.po` (3,083 lines)
- `addons/html_editor/i18n/he.po` (2,992 lines)
- `addons/html_editor/i18n/hi.po` (2,980 lines)
- `addons/html_editor/i18n/hr.po` (2,979 lines)
- `addons/html_editor/i18n/html_editor.pot` (2,964 lines)
- `addons/html_editor/i18n/hu.po` (3,004 lines)
- `addons/html_editor/i18n/id.po` (3,063 lines)
- `addons/html_editor/i18n/it.po` (3,076 lines)
- `addons/html_editor/i18n/ja.po` (3,061 lines)
- `addons/html_editor/i18n/kab.po` (2,967 lines)
- `addons/html_editor/i18n/ko.po` (3,052 lines)
- `addons/html_editor/i18n/ku.po` (2,970 lines)
- `addons/html_editor/i18n/lo.po` (2,984 lines)
- `addons/html_editor/i18n/lt.po` (2,992 lines)
- `addons/html_editor/i18n/lv.po` (2,967 lines)
- `addons/html_editor/i18n/mn.po` (2,976 lines)
- `addons/html_editor/i18n/my.po` (2,970 lines)
- `addons/html_editor/i18n/nb.po` (2,988 lines)
- `addons/html_editor/i18n/nl.po` (3,077 lines)
- `addons/html_editor/i18n/pl.po` (3,081 lines)
- `addons/html_editor/i18n/pt.po` (3,058 lines)
- `addons/html_editor/i18n/pt_BR.po` (3,082 lines)
- `addons/html_editor/i18n/ro.po` (3,067 lines)
- `addons/html_editor/i18n/ru.po` (3,050 lines)
- `addons/html_editor/i18n/sk.po` (2,966 lines)
- `addons/html_editor/i18n/sl.po` (3,030 lines)
- `addons/html_editor/i18n/sr@latin.po` (2,974 lines)
- `addons/html_editor/i18n/sv.po` (3,024 lines)
- `addons/html_editor/i18n/th.po` (3,019 lines)
- `addons/html_editor/i18n/tr.po` (3,055 lines)
- `addons/html_editor/i18n/uk.po` (3,028 lines)
- `addons/html_editor/i18n/uz.po` (3,391 lines)
- `addons/html_editor/i18n/vi.po` (3,041 lines)
- `addons/html_editor/i18n/zh_CN.po` (3,050 lines)
- `addons/html_editor/i18n/zh_TW.po` (3,043 lines)
- `addons/html_editor/models/__init__.py` (10 lines)
- `addons/html_editor/models/diff_utils.py` (349 lines)
- `addons/html_editor/models/html_field_history_mixin.py` (167 lines)
- `addons/html_editor/models/ir_attachment.py` (108 lines)
- `addons/html_editor/models/ir_http.py` (23 lines)
- `addons/html_editor/models/ir_qweb_fields.py` (581 lines)
- `addons/html_editor/models/ir_ui_view.py` (94 lines)
- `addons/html_editor/models/ir_websocket.py` (45 lines)
- `addons/html_editor/models/models.py` (14 lines)
- `addons/html_editor/models/test_models.py` (36 lines)
- `addons/html_editor/security/ir.access.csv` (3 lines)
- `addons/html_editor/static/lib/cropperjs/LICENSE` (21 lines)
- `addons/html_editor/static/lib/cropperjs/cropper.css` (304 lines)
- `addons/html_editor/static/lib/cropperjs/cropper.js` (3,576 lines)
- `addons/html_editor/static/lib/diff2html/LICENSE` (14 lines)
- `addons/html_editor/static/lib/diff2html/diff2html.min.css` (1 lines)
- `addons/html_editor/static/lib/diff2html/diff2html.min.js` (1 lines)
- `addons/html_editor/static/lib/vkbeautify/vkbeautify.0.99.00.beta.js` (358 lines)
- `addons/html_editor/static/lib/webgl-image-filter/LICENSE` (21 lines)
- `addons/html_editor/static/lib/webgl-image-filter/webgl-image-filter.js` (650 lines)
- `addons/html_editor/static/src/@types/plugins.d.ts` (302 lines)
- `addons/html_editor/static/src/backend/dynamic_field/dynamic_field_plugin.js` (360 lines)
- `addons/html_editor/static/src/backend/dynamic_field/dynamic_field_plugin.scss` (6 lines)
- `addons/html_editor/static/src/backend/dynamic_field/field_selector_popover.js` (130 lines)
- `addons/html_editor/static/src/backend/dynamic_field/field_selector_popover.xml` (49 lines)
- `addons/html_editor/static/src/components/color_picker/color_picker.js` (407 lines)
- `addons/html_editor/static/src/components/color_picker/color_picker.scss` (103 lines)
- `addons/html_editor/static/src/components/color_picker/color_picker.xml` (72 lines)
- `addons/html_editor/static/src/components/color_picker/custom_color_picker/custom_color_picker.js` (692 lines)
- `addons/html_editor/static/src/components/color_picker/custom_color_picker/custom_color_picker.scss` (48 lines)
- `addons/html_editor/static/src/components/color_picker/custom_color_picker/custom_color_picker.xml` (44 lines)
- `addons/html_editor/static/src/components/color_picker/gradient_picker/gradient_picker.js` (319 lines)
- `addons/html_editor/static/src/components/color_picker/gradient_picker/gradient_picker.scss` (64 lines)
- `addons/html_editor/static/src/components/color_picker/gradient_picker/gradient_picker.xml` (165 lines)
- `addons/html_editor/static/src/components/color_picker/tabs/custom/color_picker_custom_tab.js` (48 lines)
- `addons/html_editor/static/src/components/color_picker/tabs/custom/color_picker_custom_tab.xml` (45 lines)
- `addons/html_editor/static/src/components/color_picker/tabs/gradient/color_picker_gradient_tab.js` (85 lines)
- `addons/html_editor/static/src/components/color_picker/tabs/gradient/color_picker_gradient_tab.scss` (101 lines)
- `addons/html_editor/static/src/components/color_picker/tabs/gradient/color_picker_gradient_tab.xml` (32 lines)
- `addons/html_editor/static/src/components/color_picker/tabs/solid/color_picker_solid_tab.js` (33 lines)
- `addons/html_editor/static/src/components/color_picker/tabs/solid/color_picker_solid_tab.xml` (26 lines)
- `addons/html_editor/static/src/components/history_dialog/history_dialog.dark.scss` (9 lines)
- `addons/html_editor/static/src/components/history_dialog/history_dialog.js` (356 lines)
- `addons/html_editor/static/src/components/history_dialog/history_dialog.scss` (226 lines)
- `addons/html_editor/static/src/components/history_dialog/history_dialog.xml` (163 lines)
- `addons/html_editor/static/src/components/html_viewer/html_viewer.js` (349 lines)
- `addons/html_editor/static/src/components/html_viewer/html_viewer.xml` (12 lines)
- `addons/html_editor/static/src/components/iframe_input/iframe_input.js` (133 lines)
- `addons/html_editor/static/src/components/iframe_input/iframe_input.xml` (6 lines)
- `addons/html_editor/static/src/components/suggestion/suggestion_list.js` (33 lines)
- `addons/html_editor/static/src/components/suggestion/suggestion_list.scss` (8 lines)
- `addons/html_editor/static/src/components/suggestion/suggestion_list.xml` (12 lines)
- `addons/html_editor/static/src/components/switch/switch.js` (45 lines)
- `addons/html_editor/static/src/components/switch/switch.scss` (67 lines)
- `addons/html_editor/static/src/core/base_container_plugin.js` (279 lines)
- `addons/html_editor/static/src/core/clipboard_plugin.js` (791 lines)
- `addons/html_editor/static/src/core/comment_plugin.js` (20 lines)
- `addons/html_editor/static/src/core/content_editable_plugin.js` (77 lines)
- `addons/html_editor/static/src/core/delete_plugin.js` (1,576 lines)
- `addons/html_editor/static/src/core/dialog_plugin.js` (35 lines)
- `addons/html_editor/static/src/core/dom_observer_plugin.js` (1,353 lines)
- `addons/html_editor/static/src/core/dom_plugin.js` (825 lines)
- `addons/html_editor/static/src/core/dom_reference_map_plugin.js` (266 lines)
- `addons/html_editor/static/src/core/editor_version_plugin.js` (33 lines)
- `addons/html_editor/static/src/core/format_plugin.js` (1,023 lines)
- `addons/html_editor/static/src/core/format_plugin.scss` (7 lines)
- `addons/html_editor/static/src/core/history_plugin.js` (841 lines)
- `addons/html_editor/static/src/core/input_plugin.js` (88 lines)
- `addons/html_editor/static/src/core/legacy_compatibility_plugin.js` (23 lines)
- `addons/html_editor/static/src/core/line_break_plugin.js` (156 lines)
- `addons/html_editor/static/src/core/no_inline_root_plugin.js` (143 lines)
- `addons/html_editor/static/src/core/overlay.js` (258 lines)
- `addons/html_editor/static/src/core/overlay_plugin.js` (129 lines)
- `addons/html_editor/static/src/core/protected_node_plugin.js` (206 lines)
- `addons/html_editor/static/src/core/sanitize_plugin.js` (98 lines)
- `addons/html_editor/static/src/core/selection_plugin.js` (1,515 lines)
- `addons/html_editor/static/src/core/shortcut_plugin.js` (206 lines)
- `addons/html_editor/static/src/core/split_plugin.js` (524 lines)
- `addons/html_editor/static/src/core/style_plugin.js` (22 lines)
- `addons/html_editor/static/src/core/user_command_plugin.js` (53 lines)
- `addons/html_editor/static/src/editor.js` (557 lines)
- `addons/html_editor/static/src/fields/html_field.js` (560 lines)
- `addons/html_editor/static/src/fields/html_field.scss` (17 lines)
- `addons/html_editor/static/src/fields/html_field.xml` (38 lines)
- `addons/html_editor/static/src/fields/image_field_with_media_dialog/image_field_with_media_dialog.js` (53 lines)
- `addons/html_editor/static/src/fields/image_field_with_media_dialog/image_field_with_media_dialog.xml` (26 lines)
- `addons/html_editor/static/src/fields/property_value.js` (99 lines)
- `addons/html_editor/static/src/fields/property_value.scss` (24 lines)
- `addons/html_editor/static/src/fields/property_value.xml` (19 lines)
- `addons/html_editor/static/src/fields/x2many_field/custom_media_dialog.js` (54 lines)
- `addons/html_editor/static/src/fields/x2many_field/x2many_image_field.js` (102 lines)
- `addons/html_editor/static/src/fields/x2many_field/x2many_image_field.xml` (26 lines)
- `addons/html_editor/static/src/fields/x2many_field/x2many_media_viewer.js` (111 lines)
- `addons/html_editor/static/src/fields/x2many_field/x2many_media_viewer.xml` (10 lines)
- `addons/html_editor/static/src/html_migrations/html_migrations_utils.js` (36 lines)
- `addons/html_editor/static/src/html_migrations/html_upgrade_manager.js` (99 lines)
- `addons/html_editor/static/src/html_migrations/manifest.js` (16 lines)
- `addons/html_editor/static/src/html_migrations/migration-1.1.js` (19 lines)
- `addons/html_editor/static/src/html_migrations/migration-1.2.js` (47 lines)
- `addons/html_editor/static/src/img/curved_arrow.svg` (14 lines)
- `addons/html_editor/static/src/img/gradient-closest-corner.svg` (12 lines)
- `addons/html_editor/static/src/img/gradient-closest-side.svg` (12 lines)
- `addons/html_editor/static/src/img/gradient-farthest-corner.svg` (12 lines)
- `addons/html_editor/static/src/img/gradient-farthest-side.svg` (12 lines)
- `addons/html_editor/static/src/img/placeholder_thumbnail.png` (23 lines)
- `addons/html_editor/static/src/img/signature-icon.svg` (1 lines)

Additional files not expanded here: 478. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
