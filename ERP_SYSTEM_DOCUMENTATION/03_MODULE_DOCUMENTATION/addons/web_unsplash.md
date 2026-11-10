# Module: web_unsplash

- **Module ID:** MOD-595
- **Path:** `addons/web_unsplash`
- **Manifest:** `addons/web_unsplash/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Find free high-resolution images from Unsplash

Explore the free high-resolution image library of Unsplash.com and find images to use in Odoo. An Unsplash search bar is added to the image library modal.

Declared dependencies: `base_setup`, `html_editor`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 7 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 4 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base_setup",
    "html_editor"
  ],
  "data": [
    "views/res_config_settings_view.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "web_unsplash/static/src/frontend/unsplash_beacon.js"
    ],
    "html_editor.assets_media_dialog": [
      "web_unsplash/static/src/media_dialog/**/*",
      "web_unsplash/static/src/unsplash_credentials/**/*",
      "web_unsplash/static/src/unsplash_error/**/*",
      "web_unsplash/static/src/unsplash_service.js"
    ],
    "web.assets_unit_tests": [
      "web_unsplash/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/web_unsplash/__init__.py` (5 lines)
- `addons/web_unsplash/__manifest__.py` (29 lines)
- `addons/web_unsplash/controllers/__init__.py` (3 lines)
- `addons/web_unsplash/controllers/main.py` (148 lines)
- `addons/web_unsplash/i18n/ar.po` (221 lines)
- `addons/web_unsplash/i18n/az.po` (220 lines)
- `addons/web_unsplash/i18n/bg.po` (213 lines)
- `addons/web_unsplash/i18n/bs.po` (216 lines)
- `addons/web_unsplash/i18n/ca.po` (225 lines)
- `addons/web_unsplash/i18n/cs.po` (221 lines)
- `addons/web_unsplash/i18n/da.po` (222 lines)
- `addons/web_unsplash/i18n/de.po` (226 lines)
- `addons/web_unsplash/i18n/el.po` (217 lines)
- `addons/web_unsplash/i18n/es.po` (227 lines)
- `addons/web_unsplash/i18n/es_419.po` (217 lines)
- `addons/web_unsplash/i18n/et.po` (219 lines)
- `addons/web_unsplash/i18n/fa.po` (219 lines)
- `addons/web_unsplash/i18n/fi.po` (222 lines)
- `addons/web_unsplash/i18n/fr.po` (222 lines)
- `addons/web_unsplash/i18n/gu.po` (213 lines)
- `addons/web_unsplash/i18n/he.po` (218 lines)
- `addons/web_unsplash/i18n/hi.po` (213 lines)
- `addons/web_unsplash/i18n/hr.po` (221 lines)
- `addons/web_unsplash/i18n/hu.po` (220 lines)
- `addons/web_unsplash/i18n/id.po` (216 lines)
- `addons/web_unsplash/i18n/is.po` (209 lines)
- `addons/web_unsplash/i18n/it.po` (223 lines)
- `addons/web_unsplash/i18n/ja.po` (219 lines)
- `addons/web_unsplash/i18n/kab.po` (213 lines)
- `addons/web_unsplash/i18n/km.po` (212 lines)
- `addons/web_unsplash/i18n/ko.po` (221 lines)
- `addons/web_unsplash/i18n/ku.po` (213 lines)
- `addons/web_unsplash/i18n/lo.po` (216 lines)
- `addons/web_unsplash/i18n/lt.po` (219 lines)
- `addons/web_unsplash/i18n/lv.po` (213 lines)
- `addons/web_unsplash/i18n/mn.po` (216 lines)
- `addons/web_unsplash/i18n/my.po` (213 lines)
- `addons/web_unsplash/i18n/nb.po` (216 lines)
- `addons/web_unsplash/i18n/nl.po` (222 lines)
- `addons/web_unsplash/i18n/pl.po` (225 lines)
- `addons/web_unsplash/i18n/pt.po` (224 lines)
- `addons/web_unsplash/i18n/pt_BR.po` (226 lines)
- `addons/web_unsplash/i18n/ro.po` (225 lines)
- `addons/web_unsplash/i18n/ru.po` (222 lines)
- `addons/web_unsplash/i18n/sk.po` (217 lines)
- `addons/web_unsplash/i18n/sl.po` (216 lines)
- `addons/web_unsplash/i18n/sr@latin.po` (218 lines)
- `addons/web_unsplash/i18n/sv.po` (216 lines)
- `addons/web_unsplash/i18n/th.po` (216 lines)
- `addons/web_unsplash/i18n/tr.po` (226 lines)
- `addons/web_unsplash/i18n/uk.po` (222 lines)
- `addons/web_unsplash/i18n/uz.po` (248 lines)
- `addons/web_unsplash/i18n/vi.po` (221 lines)
- `addons/web_unsplash/i18n/web_unsplash.pot` (209 lines)
- `addons/web_unsplash/i18n/zh_CN.po` (220 lines)
- `addons/web_unsplash/i18n/zh_TW.po` (216 lines)
- `addons/web_unsplash/models/__init__.py` (7 lines)
- `addons/web_unsplash/models/ir_attachment.py` (46 lines)
- `addons/web_unsplash/models/ir_qweb_fields.py` (30 lines)
- `addons/web_unsplash/models/res_config_settings.py` (10 lines)
- `addons/web_unsplash/models/res_users.py` (16 lines)
- `addons/web_unsplash/static/description/icon.png` (5 lines)
- `addons/web_unsplash/static/description/icon.svg` (1 lines)
- `addons/web_unsplash/static/description/icon2.png` (53 lines)
- `addons/web_unsplash/static/description/icon_hi.png` (12 lines)
- `addons/web_unsplash/static/description/index.html` (22 lines)
- `addons/web_unsplash/static/description/unsplash_interface.png` (2,621 lines)
- `addons/web_unsplash/static/description/unsplash_interface_bar.png` (66 lines)
- `addons/web_unsplash/static/src/frontend/unsplash_beacon.js` (35 lines)
- `addons/web_unsplash/static/src/media_dialog/image_selector_patch.js` (212 lines)
- `addons/web_unsplash/static/src/media_dialog/media_dialog.xml` (54 lines)
- `addons/web_unsplash/static/src/media_dialog/media_dialog_patch.js` (40 lines)
- `addons/web_unsplash/static/src/unsplash_credentials/unsplash_credentials.js` (27 lines)
- `addons/web_unsplash/static/src/unsplash_credentials/unsplash_credentials.xml` (27 lines)
- `addons/web_unsplash/static/src/unsplash_error/unsplash_error.js` (16 lines)
- `addons/web_unsplash/static/src/unsplash_error/unsplash_error.xml` (9 lines)
- `addons/web_unsplash/static/src/unsplash_service.js` (130 lines)
- `addons/web_unsplash/static/tests/unsplash.test.js` (169 lines)
- `addons/web_unsplash/tests/__init__.py` (3 lines)
- `addons/web_unsplash/tests/test_unsplash.py` (107 lines)
- `addons/web_unsplash/utils.py` (18 lines)
- `addons/web_unsplash/views/res_config_settings_view.xml` (25 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
