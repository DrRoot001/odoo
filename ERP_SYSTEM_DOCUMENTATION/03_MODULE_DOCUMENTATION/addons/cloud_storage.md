# Module: cloud_storage

- **Module ID:** MOD-049
- **Path:** `addons/cloud_storage`
- **Manifest:** `addons/cloud_storage/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Store chatter attachments in the cloud

No manifest description declared.

Declared dependencies: `base_setup`, `mail`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 14 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 7 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base_setup",
    "mail"
  ],
  "data": [
    "views/settings.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "cloud_storage/static/src/core/common/**/*",
      "cloud_storage/static/src/core/public_web/**/*",
      "cloud_storage/static/src/**/web/**/*"
    ],
    "mail.assets_public": [
      "cloud_storage/static/src/core/common/**/*",
      "cloud_storage/static/src/core/public_web/**/*"
    ],
    "portal.assets_chatter_helpers": [
      "cloud_storage/static/src/core/common/**/*"
    ],
    "web.assets_unit_tests": [
      "cloud_storage/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/cloud_storage/__init__.py` (4 lines)
- `addons/cloud_storage/__manifest__.py` (30 lines)
- `addons/cloud_storage/controllers/__init__.py` (4 lines)
- `addons/cloud_storage/controllers/attachment.py` (35 lines)
- `addons/cloud_storage/controllers/rtc.py` (92 lines)
- `addons/cloud_storage/data/neutralize.sql` (1 lines)
- `addons/cloud_storage/i18n/ar.po` (171 lines)
- `addons/cloud_storage/i18n/az.po` (166 lines)
- `addons/cloud_storage/i18n/bg.po` (166 lines)
- `addons/cloud_storage/i18n/bs.po` (166 lines)
- `addons/cloud_storage/i18n/ca.po` (169 lines)
- `addons/cloud_storage/i18n/cloud_storage.pot` (159 lines)
- `addons/cloud_storage/i18n/cs.po` (167 lines)
- `addons/cloud_storage/i18n/da.po` (172 lines)
- `addons/cloud_storage/i18n/de.po` (177 lines)
- `addons/cloud_storage/i18n/el.po` (165 lines)
- `addons/cloud_storage/i18n/es.po` (181 lines)
- `addons/cloud_storage/i18n/es_419.po` (178 lines)
- `addons/cloud_storage/i18n/et.po` (171 lines)
- `addons/cloud_storage/i18n/fa.po` (166 lines)
- `addons/cloud_storage/i18n/fi.po` (176 lines)
- `addons/cloud_storage/i18n/fr.po` (178 lines)
- `addons/cloud_storage/i18n/he.po` (165 lines)
- `addons/cloud_storage/i18n/hi.po` (166 lines)
- `addons/cloud_storage/i18n/hr.po` (167 lines)
- `addons/cloud_storage/i18n/hu.po` (167 lines)
- `addons/cloud_storage/i18n/id.po` (173 lines)
- `addons/cloud_storage/i18n/it.po` (176 lines)
- `addons/cloud_storage/i18n/ja.po` (174 lines)
- `addons/cloud_storage/i18n/kab.po` (165 lines)
- `addons/cloud_storage/i18n/ko.po` (170 lines)
- `addons/cloud_storage/i18n/ku.po` (164 lines)
- `addons/cloud_storage/i18n/lo.po` (168 lines)
- `addons/cloud_storage/i18n/lt.po` (168 lines)
- `addons/cloud_storage/i18n/lv.po` (168 lines)
- `addons/cloud_storage/i18n/mn.po` (166 lines)
- `addons/cloud_storage/i18n/my.po` (164 lines)
- `addons/cloud_storage/i18n/nb.po` (167 lines)
- `addons/cloud_storage/i18n/nl.po` (172 lines)
- `addons/cloud_storage/i18n/pl.po` (175 lines)
- `addons/cloud_storage/i18n/pt.po` (176 lines)
- `addons/cloud_storage/i18n/pt_BR.po` (176 lines)
- `addons/cloud_storage/i18n/ro.po` (177 lines)
- `addons/cloud_storage/i18n/ru.po` (174 lines)
- `addons/cloud_storage/i18n/sk.po` (167 lines)
- `addons/cloud_storage/i18n/sl.po` (173 lines)
- `addons/cloud_storage/i18n/sr@latin.po` (167 lines)
- `addons/cloud_storage/i18n/sv.po` (174 lines)
- `addons/cloud_storage/i18n/th.po` (170 lines)
- `addons/cloud_storage/i18n/tr.po` (173 lines)
- `addons/cloud_storage/i18n/uk.po` (167 lines)
- `addons/cloud_storage/i18n/uz.po` (197 lines)
- `addons/cloud_storage/i18n/vi.po` (172 lines)
- `addons/cloud_storage/i18n/zh_CN.po` (170 lines)
- `addons/cloud_storage/i18n/zh_TW.po` (172 lines)
- `addons/cloud_storage/models/__init__.py` (5 lines)
- `addons/cloud_storage/models/ir_attachment.py` (148 lines)
- `addons/cloud_storage/models/ir_http.py` (16 lines)
- `addons/cloud_storage/models/res_config_settings.py` (85 lines)
- `addons/cloud_storage/static/src/chatter/web/chatter_patch.js` (11 lines)
- `addons/cloud_storage/static/src/chatter/web/chatter_patch.xml` (12 lines)
- `addons/cloud_storage/static/src/core/common/attachment_list_patch.js` (20 lines)
- `addons/cloud_storage/static/src/core/common/attachment_model_patch.js` (99 lines)
- `addons/cloud_storage/static/src/core/common/file_viewer_patch.js` (33 lines)
- `addons/cloud_storage/static/src/core/public_web/attachment_upload_service_patch.js` (110 lines)
- `addons/cloud_storage/static/src/core/public_web/composer_patch.js` (13 lines)
- `addons/cloud_storage/static/src/core/public_web/composer_patch.xml` (8 lines)
- `addons/cloud_storage/static/tests/attachment_list.test.js` (54 lines)
- `addons/cloud_storage/tests/__init__.py` (5 lines)
- `addons/cloud_storage/tests/test_attachment_controller.py` (57 lines)
- `addons/cloud_storage/tests/test_ir_attachment.py` (27 lines)
- `addons/cloud_storage/tests/test_rtc.py` (183 lines)
- `addons/cloud_storage/tests/tools.py` (9 lines)
- `addons/cloud_storage/views/settings.xml` (26 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
