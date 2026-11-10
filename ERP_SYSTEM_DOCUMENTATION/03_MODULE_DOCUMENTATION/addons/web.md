# Module: web

- **Module ID:** MOD-592
- **Path:** `addons/web`
- **Manifest:** `addons/web/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Odoo Web core module.
========================

This module provides the core of the Odoo Web Client.


Declared dependencies: `base`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 70 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 15 | Files under `models/` or `models.py`. |
| Controller-path Python files | 20 | Files under `controllers/` or `controllers.py`. |
| XML files | 287 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1083 | Client behavior/assets. |
| Tests | 31 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 73 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base"
  ],
  "data": [
    "views/webclient_templates.xml",
    "views/report_templates.xml",
    "views/base_document_layout_views.xml",
    "views/partner_view.xml",
    "views/speedscope_template.xml",
    "views/memory_template.xml",
    "views/speedscope_config_wizard.xml",
    "views/neutralize_views.xml",
    "views/ir_ui_view_views.xml",
    "data/ir_attachment.xml",
    "data/report_layout.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_emoji": [
      "web/static/src/core/emoji_picker/emoji_data.js"
    ],
    "web.assets_backend": [
      [
        "include",
        "web._assets_helpers"
      ],
      [
        "include",
        "web._assets_backend_helpers"
      ],
      "web/static/src/scss/pre_variables.scss",
      "web/static/lib/bootstrap/scss/_variables.scss",
      "web/static/lib/bootstrap/scss/_variables-dark.scss",
      "web/static/lib/bootstrap/scss/_maps.scss",
      [
        "include",
        "web._assets_bootstrap_backend"
      ],
      [
        "include",
        "web._assets_core"
      ],
      [
        "include",
        "web.icons_fonts"
      ],
      "web/static/src/webclient/navbar/navbar.scss",
      "web/static/src/scss/animation.scss",
      "web/static/src/scss/mimetypes.scss",
      "web/static/src/scss/ui.scss",
      "web/static/src/polyfills/clipboard.js",
      "web/static/lib/popper/popper.js",
      "web/static/lib/bootstrap/js/dist/util/index.js",
      "web/static/lib/bootstrap/js/dist/dom/data.js",
      "web/static/lib/bootstrap/js/dist/dom/event-handler.js",
      "web/static/lib/bootstrap/js/dist/dom/manipulator.js",
      "web/static/lib/bootstrap/js/dist/dom/selector-engine.js",
      "web/static/lib/bootstrap/js/dist/util/config.js",
      "web/static/lib/bootstrap/js/dist/util/component-functions.js",
      "web/static/lib/bootstrap/js/dist/util/backdrop.js",
      "web/static/lib/bootstrap/js/dist/util/focustrap.js",
      "web/static/lib/bootstrap/js/dist/util/sanitizer.js",
      "web/static/lib/bootstrap/js/dist/util/scrollbar.js",
      "web/static/lib/bootstrap/js/dist/util/swipe.js",
      "web/static/lib/bootstrap/js/dist/util/template-factory.js",
      "web/static/lib/bootstrap/js/dist/base-component.js",
      "web/static/lib/bootstrap/js/dist/alert.js",
      "web/static/lib/bootstrap/js/dist/button.js",
      "web/static/lib/bootstrap/js/dist/carousel.js",
      "web/static/lib/bootstrap/js/dist/collapse.js",
      "web/static/lib/bootstrap/js/dist/dropdown.js",
      "web/static/lib/bootstrap/js/dist/modal.js",
      "web/static/lib/bootstrap/js/dist/offcanvas.js",
      "web/static/lib/bootstrap/js/dist/tooltip.js",
      "web/static/lib/bootstrap/js/dist/popover.js",
      "web/static/lib/bootstrap/js/dist/scrollspy.js",
      "web/static/lib/bootstrap/js/dist/tab.js",
      "web/static/lib/bootstrap/js/dist/toast.js",
      "web/static/src/libs/bootstrap.js",
      "web/static/lib/dompurify/DOMpurify.js",
      "base/static/src/css/modules.css",
      "web/static/src/core/utils/transitions.scss",
      "web/static/src/model/**/*",
      "web/static/src/search/**/*",
      "web/static/src/webclient/icons.scss",
      "web/static/src/views/**/*",
      [
        "remove",
        "web/static/src/views/graph/**"
      ],
      [
        "remove",
        "web/static/src/views/pivot/**"
      ],
      "web/static/src/webclient/**/*",
      [
        "remove",
        "web/static/src/webclient/clickbot/clickbot.js"
      ],
      [
        "remove",
        "web/static/src/views/form/button_box/*.scss"
      ],
      [
        "remove",
        "web/static/src/webclient/actions/reports/**/*"
      ],
      "web/static/src/webclient/actions/reports/*.js",
      "web/static/src/webclient/actions/reports/*.xml",
      "web/static/src/scss/ace.scss",
      "web/static/src/scss/base_document_layout.scss",
      "base/static/src/scss/res_partner.scss",
      "base/static/src/scss/res_users.scss",
      "web/static/src/views/form/button_box/*.scss",
      [
        "remove",
        "web/static/src/**/*.dark.scss"
      ]
    ],
    "web.assets_backend_lazy": [
      [
        "include",
        "web._assets_helpers"
      ],
      [
        "include",
        "web._assets_backend_helpers"
      ],
      "web/static/src/scss/pre_variables.scss",
      "web/static/lib/bootstrap/scss/_variables.scss",
      "web/static/lib/bootstrap/scss/_variables-dark.scss",
      "web/static/lib/bootstrap/scss/_maps.scss",
      "web/static/src/views/graph/**",
      "web/static/src/views/pivot/**"
    ],
    "web.assets_backend_lazy_dark": [
      [
        "include",
        "web.assets_backend_lazy"
      ]
    ],
    "web.assets_web": [
      [
        "include",
        "web.assets_backend"
      ],
      "web/static/src/main.js",
      "web/static/src/start.js"
    ],
    "web.assets_frontend_minimal": [
      "web/static/src/polyfills/object.js",
      "web/static/src/polyfills/array.js",
      "web/static/src/polyfills/promise.js",
      "web/static/src/module_loader.js",
      "web/static/src/polyfills/set.js",
      "web/static/src/polyfills/map.js",
      "web/static/src/session.js",
      "web/static/src/core/browser/cookie.js",
      "web/static/src/core/utils/ui.js",
      "web/static/src/public/utils.js",
      "web/static/src/public/lazyloader.js"
    ],
    "web.assets_frontend": [
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
      "web/static/lib/luxon/luxon.js",
      "web/static/src/libs/luxon.js",
      [
        "include",
        "web._assets_bootstrap_frontend"
      ],
      [
        "include",
        "web.icons_fonts"
      ],
      "web/static/src/webclient/navbar/navbar.scss",
      "web/static/src/scss/animation.scss",
      "web/static/src/scss/base_frontend.scss",
      "web/static/src/scss/mimetypes.scss",
      "web/static/src/scss/ui.scss",
      "web/static/src/views/fields/signature/signature_field.scss",
      [
        "include",
        "web.assets_frontend_minimal"
      ],
      "web/static/lib/owl/owl.js",
      "web/static/src/owl2/owl3_compatibility_layer.js",
      "web/static/src/owl2/utils.js",
      "web/static/lib/owl/odoo_module.js",
      "web/static/lib/popper/popper.js",
      "web/static/lib/bootstrap/js/dist/util/index.js",
      "web/static/lib/bootstrap/js/dist/dom/data.js",
      "web/static/lib/bootstrap/js/dist/dom/event-handler.js",
      "web/static/lib/bootstrap/js/dist/dom/manipulator.js",
      "web/static/lib/bootstrap/js/dist/dom/selector-engine.js",
      "web/static/lib/bootstrap/js/dist/util/config.js",
      "web/static/lib/bootstrap/js/dist/util/component-functions.js",
      "web/static/lib/bootstrap/js/dist/util/backdrop.js",
      "web/static/lib/bootstrap/js/dist/util/focustrap.js",
      "web/static/lib/bootstrap/js/dist/util/sanitizer.js",
      "web/static/lib/bootstrap/js/dist/util/scrollbar.js",
      "web/static/lib/bootstrap/js/dist/util/swipe.js",
      "web/static/lib/bootstrap/js/dist/util/template-factory.js",
      "web/static/lib/bootstrap/js/dist/base-component.js",
      "web/static/lib/bootstrap/js/dist/alert.js",
      "web/static/lib/bootstrap/js/dist/button.js",
      "web/static/lib/bootstrap/js/dist/carousel.js",
      "web/static/lib/bootstrap/js/dist/collapse.js",
      "web/static/lib/bootstrap/js/dist/dropdown.js",
      "web/static/lib/bootstrap/js/dist/modal.js",
      "web/static/lib/bootstrap/js/dist/offcanvas.js",
      "web/static/lib/bootstrap/js/dist/tooltip.js",
      "web/static/lib/bootstrap/js/dist/popover.js",
      "web/static/lib/bootstrap/js/dist/scrollspy.js",
      "web/static/lib/bootstrap/js/dist/tab.js",
      "web/static/lib/bootstrap/js/dist/toast.js",
      "web/static/src/libs/bootstrap.js",
      "web/static/src/env.js",
      "web/static/src/core/utils/transitions.scss",
      "web/static/src/core/**/*",
      [
        "remove",
        "web/static/src/core/commands/**/*"
      ],
      [
        "remove",
        "web/static/src/core/debug/debug_menu.js"
      ],
      [
        "remove",
        "web/static/src/core/file_viewer/file_viewer.dark.scss"
      ],
      [
        "remove",
        "web/static/src/core/emoji_picker/emoji_data.js"
      ],
      "web/static/src/core/commands/default_providers.js",
      "web/static/src/core/commands/command_palette.js",
      "web/static/src/public/**/*.js",
      "web/static/src/public/**/*.xml",
      [
        "remove",
        "web/static/src/public/database_manager.js"
      ]
    ],
    "web.assets_frontend_lazy": [
      [
        "include",
        "web.assets_frontend"
      ],
      [
        "remove",
        "web/static/src/module_loader.js"
      ],
      [
        "remove",
        "web/static/src/session.js"
      ],
      [
        "remove",
        "web/static/src/core/browser/cookie.js"
      ],
      [
        "remove",
        "web/static/src/core/utils/ui.js"
      ],
      [
        "remove",
        "web/static/src/public/utils.js"
      ],
      [
        "remove",
        "web/static/src/public/lazyloader.js"
      ]
    ],
    "web.report_assets_common": [
      "web/static/src/scss/functions.scss",
      "web/static/src/scss/utils.scss",
      [
        "include",
        "web._assets_primary_variables"
      ],
      [
        "include",
        "web._assets_secondary_variables"
      ],
      "web/static/src/webclient/actions/reports/bootstrap_overridden_report.scss",
      [
        "include",
        "web._assets_helpers"
      ],
      [
        "include",
        "web._assets_backend_helpers"
      ],
      "web/static/src/scss/pre_variables.scss",
      "web/static/lib/bootstrap/scss/_variables.scss",
      "web/static/lib/bootstrap/scss/_variables-dark.scss",
      "web/static/lib/bootstrap/scss/_maps.scss",
      [
        "include",
        "web._assets_bootstrap_backend"
      ],
      [
        "remove",
        "web/static/src/scss/utilities_custom_backend.scss"
      ],
      [
        "remove",
        "web/static/src/scss/bootstrap_review_backend.scss"
      ],
      [
        "after",
        "web/static/src/scss/utilities_custom.scss",
        "web/static/src/webclient/actions/reports/utilities_custom_report.scss"
      ],
      "web/static/lib/popper/popper.js",
      "web/static/lib/bootstrap/js/dist/util/index.js",
      "web/static/lib/bootstrap/js/dist/dom/data.js",
      "web/static/lib/bootstrap/js/dist/dom/event-handler.js",
      "web/static/lib/bootstrap/js/dist/dom/manipulator.js",
      "web/static/lib/bootstrap/js/dist/dom/selector-engine.js",
      "web/static/lib/bootstrap/js/dist/util/config.js",
      "web/static/lib/bootstrap/js/dist/util/component-functions.js",
      "web/static/lib/bootstrap/js/dist/util/backdrop.js",
      "web/static/lib/bootstrap/js/dist/util/focustrap.js",
      "web/static/lib/bootstrap/js/dist/util/sanitizer.js",
      "web/static/lib/bootstrap/js/dist/util/scrollbar.js",
      "web/static/lib/bootstrap/js/dist/util/swipe.js",
      "web/static/lib/bootstrap/js/dist/util/template-factory.js",
      "web/static/lib/bootstrap/js/dist/base-component.js",
      "web/static/lib/bootstrap/js/dist/alert.js",
      "web/static/lib/bootstrap/js/dist/button.js",
      "web/static/lib/bootstrap/js/dist/carousel.js",
      "web/static/lib/bootstrap/js/dist/collapse.js",
      "web/static/lib/bootstrap/js/dist/dropdown.js",
      "web/static/lib/bootstrap/js/dist/modal.js",
      "web/static/lib/bootstrap/js/dist/offcanvas.js",
      "web/static/lib/bootstrap/js/dist/tooltip.js",
      "web/static/lib/bootstrap/js/dist/popover.js",
      "web/static/lib/bootstrap/js/dist/scrollspy.js",
      "web/static/lib/bootstrap/js/di
```

### Representative source files

- `addons/web/__init__.py` (5 lines)
- `addons/web/__manifest__.py` (560 lines)
- `addons/web/controllers/__init__.py` (33 lines)
- `addons/web/controllers/action.py` (113 lines)
- `addons/web/controllers/binary.py` (321 lines)
- `addons/web/controllers/database.py` (308 lines)
- `addons/web/controllers/dataset.py` (41 lines)
- `addons/web/controllers/domain.py` (24 lines)
- `addons/web/controllers/export.py` (617 lines)
- `addons/web/controllers/home.py` (231 lines)
- `addons/web/controllers/json.py` (354 lines)
- `addons/web/controllers/main.py` (8 lines)
- `addons/web/controllers/model.py` (14 lines)
- `addons/web/controllers/pivot.py` (98 lines)
- `addons/web/controllers/profiling.py` (86 lines)
- `addons/web/controllers/report.py` (166 lines)
- `addons/web/controllers/session.py` (110 lines)
- `addons/web/controllers/utils.py` (281 lines)
- `addons/web/controllers/vcard.py` (47 lines)
- `addons/web/controllers/view.py` (27 lines)
- `addons/web/controllers/webclient.py` (215 lines)
- `addons/web/controllers/webmanifest.py` (204 lines)
- `addons/web/data/ir_attachment.xml` (10 lines)
- `addons/web/data/neutralize.sql` (4 lines)
- `addons/web/data/report_layout.xml` (63 lines)
- `addons/web/i18n/af.po` (27,557 lines)
- `addons/web/i18n/ar.po` (33,809 lines)
- `addons/web/i18n/az.po` (33,777 lines)
- `addons/web/i18n/bg.po` (33,716 lines)
- `addons/web/i18n/bn.po` (27,559 lines)
- `addons/web/i18n/bs.po` (33,674 lines)
- `addons/web/i18n/ca.po` (33,748 lines)
- `addons/web/i18n/cs.po` (33,763 lines)
- `addons/web/i18n/da.po` (33,809 lines)
- `addons/web/i18n/de.po` (34,064 lines)
- `addons/web/i18n/el.po` (33,694 lines)
- `addons/web/i18n/es.po` (33,883 lines)
- `addons/web/i18n/es_419.po` (33,943 lines)
- `addons/web/i18n/es_CL.po` (340 lines)
- `addons/web/i18n/et.po` (33,757 lines)
- `addons/web/i18n/eu.po` (27,559 lines)
- `addons/web/i18n/fa.po` (33,839 lines)
- `addons/web/i18n/fi.po` (33,875 lines)
- `addons/web/i18n/fr.po` (33,977 lines)
- `addons/web/i18n/gl.po` (27,559 lines)
- `addons/web/i18n/gu.po` (27,566 lines)
- `addons/web/i18n/he.po` (33,713 lines)
- `addons/web/i18n/hi.po` (33,674 lines)
- `addons/web/i18n/hr.po` (33,746 lines)
- `addons/web/i18n/hu.po` (33,707 lines)
- `addons/web/i18n/id.po` (33,923 lines)
- `addons/web/i18n/is.po` (27,558 lines)
- `addons/web/i18n/it.po` (33,957 lines)
- `addons/web/i18n/ja.po` (33,908 lines)
- `addons/web/i18n/ka.po` (27,559 lines)
- `addons/web/i18n/kab.po` (33,660 lines)
- `addons/web/i18n/km.po` (27,559 lines)
- `addons/web/i18n/ko.po` (33,783 lines)
- `addons/web/i18n/ku.po` (33,667 lines)
- `addons/web/i18n/lo.po` (35,548 lines)
- `addons/web/i18n/lt.po` (33,709 lines)
- `addons/web/i18n/lv.po` (33,675 lines)
- `addons/web/i18n/mk.po` (27,564 lines)
- `addons/web/i18n/mn.po` (33,899 lines)
- `addons/web/i18n/my.po` (33,661 lines)
- `addons/web/i18n/nb.po` (33,697 lines)
- `addons/web/i18n/nl.po` (34,025 lines)
- `addons/web/i18n/pl.po` (33,985 lines)
- `addons/web/i18n/pt.po` (33,823 lines)
- `addons/web/i18n/pt_BR.po` (36,923 lines)
- `addons/web/i18n/ro.po` (33,846 lines)
- `addons/web/i18n/ru.po` (33,814 lines)
- `addons/web/i18n/sk.po` (33,713 lines)
- `addons/web/i18n/sl.po` (33,699 lines)
- `addons/web/i18n/sr@latin.po` (33,683 lines)
- `addons/web/i18n/sv.po` (33,804 lines)
- `addons/web/i18n/th.po` (33,736 lines)
- `addons/web/i18n/tr.po` (33,859 lines)
- `addons/web/i18n/uk.po` (33,763 lines)
- `addons/web/i18n/uz.po` (38,070 lines)
- `addons/web/i18n/vi.po` (33,810 lines)
- `addons/web/i18n/web.pot` (33,323 lines)
- `addons/web/i18n/zh_CN.po` (33,937 lines)
- `addons/web/i18n/zh_TW.po` (33,726 lines)
- `addons/web/icons.py` (701 lines)
- `addons/web/models/__init__.py` (17 lines)
- `addons/web/models/base_document_layout.py` (266 lines)
- `addons/web/models/ir_attachment.py` (34 lines)
- `addons/web/models/ir_http.py` (221 lines)
- `addons/web/models/ir_model.py` (98 lines)
- `addons/web/models/ir_qweb_fields.py` (166 lines)
- `addons/web/models/ir_ui_menu.py` (87 lines)
- `addons/web/models/ir_ui_view.py` (31 lines)
- `addons/web/models/models.py` (2,571 lines)
- `addons/web/models/properties_base_definition.py` (21 lines)
- `addons/web/models/res_config_settings.py` (10 lines)
- `addons/web/models/res_partner.py` (95 lines)
- `addons/web/models/res_users.py` (36 lines)
- `addons/web/models/res_users_settings.py` (39 lines)
- `addons/web/models/res_users_settings_embedded_action.py` (66 lines)
- `addons/web/security/ir.access.csv` (4 lines)
- `addons/web/static/fonts/fonts.scss` (122 lines)
- `addons/web/static/fonts/google/Fira_Mono/Fira_Mono-Bold.ttf` (1,629 lines)
- `addons/web/static/fonts/google/Fira_Mono/Fira_Mono-Medium.ttf` (1,391 lines)
- `addons/web/static/fonts/google/Fira_Mono/Fira_Mono-Regular.ttf` (1,461 lines)
- `addons/web/static/fonts/google/Fira_Mono/OFL.txt` (93 lines)
- `addons/web/static/fonts/google/Montserrat/Montserrat-Black.ttf` (2,519 lines)
- `addons/web/static/fonts/google/Montserrat/Montserrat-BlackItalic.ttf` (2,540 lines)
- `addons/web/static/fonts/google/Montserrat/Montserrat-Bold.ttf` (2,018 lines)
- `addons/web/static/fonts/google/Montserrat/Montserrat-BoldItalic.ttf` (2,035 lines)
- `addons/web/static/fonts/google/Montserrat/Montserrat-ExtraBold.ttf` (1,881 lines)
- `addons/web/static/fonts/google/Montserrat/Montserrat-ExtraBoldItalic.ttf` (2,053 lines)
- `addons/web/static/fonts/google/Montserrat/Montserrat-ExtraLight.ttf` (1,916 lines)
- `addons/web/static/fonts/google/Montserrat/Montserrat-ExtraLightItalic.ttf` (2,027 lines)
- `addons/web/static/fonts/google/Montserrat/Montserrat-Italic.ttf` (2,086 lines)
- `addons/web/static/fonts/google/Montserrat/Montserrat-Light.ttf` (2,036 lines)
- `addons/web/static/fonts/google/Montserrat/Montserrat-LightItalic.ttf` (2,223 lines)
- `addons/web/static/fonts/google/Montserrat/Montserrat-Medium.ttf` (1,903 lines)
- `addons/web/static/fonts/google/Montserrat/Montserrat-MediumItalic.ttf` (2,035 lines)
- `addons/web/static/fonts/google/Montserrat/Montserrat-Regular.ttf` (1,812 lines)
- `addons/web/static/fonts/google/Montserrat/Montserrat-SemiBold.ttf` (1,961 lines)
- `addons/web/static/fonts/google/Montserrat/Montserrat-SemiBoldItalic.ttf` (2,063 lines)
- `addons/web/static/fonts/google/Montserrat/Montserrat-Thin.ttf` (2,168 lines)
- `addons/web/static/fonts/google/Montserrat/Montserrat-ThinItalic.ttf` (2,239 lines)
- `addons/web/static/fonts/google/Montserrat/OFL.txt` (93 lines)
- `addons/web/static/fonts/google/Noto_Sans_Mono/Noto_Sans_Mono-Bold.woff` (152 lines)
- `addons/web/static/fonts/google/Noto_Sans_Mono/Noto_Sans_Mono-Medium.woff` (171 lines)
- `addons/web/static/fonts/google/Noto_Sans_Mono/Noto_Sans_Mono-Regular.woff` (167 lines)
- `addons/web/static/fonts/google/Noto_Sans_Mono/OFL.txt` (93 lines)
- `addons/web/static/fonts/google/Open_Sans/LICENSE.txt` (202 lines)
- `addons/web/static/fonts/google/Open_Sans/Open_Sans-Bold.ttf` (1,296 lines)
- `addons/web/static/fonts/google/Open_Sans/Open_Sans-BoldItalic.ttf` (771 lines)
- `addons/web/static/fonts/google/Open_Sans/Open_Sans-ExtraBold.ttf` (1,139 lines)
- `addons/web/static/fonts/google/Open_Sans/Open_Sans-ExtraBoldItalic.ttf` (840 lines)
- `addons/web/static/fonts/google/Open_Sans/Open_Sans-Italic.ttf` (853 lines)
- `addons/web/static/fonts/google/Open_Sans/Open_Sans-Light.ttf` (1,183 lines)
- `addons/web/static/fonts/google/Open_Sans/Open_Sans-LightItalic.ttf` (728 lines)
- `addons/web/static/fonts/google/Open_Sans/Open_Sans-Regular.ttf` (1,056 lines)
- `addons/web/static/fonts/google/Open_Sans/Open_Sans-SemiBold.ttf` (1,174 lines)
- `addons/web/static/fonts/google/Open_Sans/Open_Sans-SemiBoldItalic.ttf` (904 lines)
- `addons/web/static/fonts/google/Oswald/OFL.txt` (93 lines)
- `addons/web/static/fonts/google/Oswald/Oswald-Bold.ttf` (799 lines)
- `addons/web/static/fonts/google/Oswald/Oswald-ExtraLight.ttf` (705 lines)
- `addons/web/static/fonts/google/Oswald/Oswald-Light.ttf` (857 lines)
- `addons/web/static/fonts/google/Oswald/Oswald-Medium.ttf` (792 lines)
- `addons/web/static/fonts/google/Oswald/Oswald-Regular.ttf` (799 lines)
- `addons/web/static/fonts/google/Oswald/Oswald-SemiBold.ttf` (792 lines)
- `addons/web/static/fonts/google/Playball/OFL.txt` (93 lines)
- `addons/web/static/fonts/google/Playball/Playball-Regular.ttf` (3,820 lines)
- `addons/web/static/fonts/google/Raleway/OFL.txt` (95 lines)
- `addons/web/static/fonts/google/Raleway/Raleway-Black.ttf` (1,398 lines)
- `addons/web/static/fonts/google/Raleway/Raleway-BlackItalic.ttf` (1,564 lines)
- `addons/web/static/fonts/google/Raleway/Raleway-Bold.ttf` (1,312 lines)
- `addons/web/static/fonts/google/Raleway/Raleway-BoldItalic.ttf` (1,528 lines)
- `addons/web/static/fonts/google/Raleway/Raleway-ExtraBold.ttf` (1,465 lines)
- `addons/web/static/fonts/google/Raleway/Raleway-ExtraBoldItalic.ttf` (1,476 lines)
- `addons/web/static/fonts/google/Raleway/Raleway-ExtraLight.ttf` (1,475 lines)
- `addons/web/static/fonts/google/Raleway/Raleway-ExtraLightItalic.ttf` (1,328 lines)
- `addons/web/static/fonts/google/Raleway/Raleway-Italic.ttf` (1,496 lines)
- `addons/web/static/fonts/google/Raleway/Raleway-Light.ttf` (1,447 lines)

Additional files not expanded here: 2270. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
