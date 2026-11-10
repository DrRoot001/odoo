# Module: cloud_storage_google

- **Module ID:** MOD-051
- **Path:** `addons/cloud_storage_google`
- **Manifest:** `addons/cloud_storage_google/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Store chatter attachments in the Google cloud

No manifest description declared.

Declared dependencies: `cloud_storage`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "cloud_storage"
  ],
  "data": [
    "views/settings.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "cloud_storage_google/static/src/**/*"
    ]
  },
  "external_dependencies": {
    "python": [
      "google-auth"
    ],
    "apt": {
      "google-auth": "python3-google-auth"
    }
  }
}
```

### Representative source files

- `addons/cloud_storage_google/__init__.py` (14 lines)
- `addons/cloud_storage_google/__manifest__.py` (25 lines)
- `addons/cloud_storage_google/data/neutralize.sql` (4 lines)
- `addons/cloud_storage_google/i18n/ar.po` (125 lines)
- `addons/cloud_storage_google/i18n/az.po` (115 lines)
- `addons/cloud_storage_google/i18n/bg.po` (115 lines)
- `addons/cloud_storage_google/i18n/bs.po` (117 lines)
- `addons/cloud_storage_google/i18n/ca.po` (118 lines)
- `addons/cloud_storage_google/i18n/cloud_storage_google.pot` (111 lines)
- `addons/cloud_storage_google/i18n/cs.po` (116 lines)
- `addons/cloud_storage_google/i18n/da.po` (125 lines)
- `addons/cloud_storage_google/i18n/de.po` (127 lines)
- `addons/cloud_storage_google/i18n/el.po` (116 lines)
- `addons/cloud_storage_google/i18n/es.po` (127 lines)
- `addons/cloud_storage_google/i18n/es_419.po` (126 lines)
- `addons/cloud_storage_google/i18n/et.po` (123 lines)
- `addons/cloud_storage_google/i18n/fa.po` (115 lines)
- `addons/cloud_storage_google/i18n/fi.po` (125 lines)
- `addons/cloud_storage_google/i18n/fr.po` (125 lines)
- `addons/cloud_storage_google/i18n/he.po` (116 lines)
- `addons/cloud_storage_google/i18n/hi.po` (115 lines)
- `addons/cloud_storage_google/i18n/hr.po` (116 lines)
- `addons/cloud_storage_google/i18n/hu.po` (116 lines)
- `addons/cloud_storage_google/i18n/id.po` (124 lines)
- `addons/cloud_storage_google/i18n/it.po` (124 lines)
- `addons/cloud_storage_google/i18n/ja.po` (125 lines)
- `addons/cloud_storage_google/i18n/kab.po` (116 lines)
- `addons/cloud_storage_google/i18n/ko.po` (124 lines)
- `addons/cloud_storage_google/i18n/ku.po` (115 lines)
- `addons/cloud_storage_google/i18n/lo.po` (114 lines)
- `addons/cloud_storage_google/i18n/lt.po` (117 lines)
- `addons/cloud_storage_google/i18n/lv.po` (117 lines)
- `addons/cloud_storage_google/i18n/mn.po` (115 lines)
- `addons/cloud_storage_google/i18n/my.po` (115 lines)
- `addons/cloud_storage_google/i18n/nb.po` (116 lines)
- `addons/cloud_storage_google/i18n/nl.po` (124 lines)
- `addons/cloud_storage_google/i18n/pl.po` (127 lines)
- `addons/cloud_storage_google/i18n/pt.po` (125 lines)
- `addons/cloud_storage_google/i18n/pt_BR.po` (124 lines)
- `addons/cloud_storage_google/i18n/ro.po` (125 lines)
- `addons/cloud_storage_google/i18n/ru.po` (126 lines)
- `addons/cloud_storage_google/i18n/sk.po` (116 lines)
- `addons/cloud_storage_google/i18n/sl.po` (125 lines)
- `addons/cloud_storage_google/i18n/sr@latin.po` (116 lines)
- `addons/cloud_storage_google/i18n/sv.po` (127 lines)
- `addons/cloud_storage_google/i18n/th.po` (123 lines)
- `addons/cloud_storage_google/i18n/tr.po` (126 lines)
- `addons/cloud_storage_google/i18n/uk.po` (116 lines)
- `addons/cloud_storage_google/i18n/uz.po` (143 lines)
- `addons/cloud_storage_google/i18n/vi.po` (125 lines)
- `addons/cloud_storage_google/i18n/zh_CN.po` (123 lines)
- `addons/cloud_storage_google/i18n/zh_TW.po` (125 lines)
- `addons/cloud_storage_google/models/__init__.py` (4 lines)
- `addons/cloud_storage_google/models/ir_attachment.py` (88 lines)
- `addons/cloud_storage_google/models/res_config_settings.py` (122 lines)
- `addons/cloud_storage_google/static/src/scss/cloud_storage_google.scss` (5 lines)
- `addons/cloud_storage_google/tests/__init__.py` (5 lines)
- `addons/cloud_storage_google/tests/test_cloud_storage_google.py` (68 lines)
- `addons/cloud_storage_google/tests/test_cloud_storage_google_attachment_controller.py` (87 lines)
- `addons/cloud_storage_google/tests/test_res_config_settings.py` (31 lines)
- `addons/cloud_storage_google/utils/__init__.py` (3 lines)
- `addons/cloud_storage_google/utils/cleanup_cloud_storage_google.py` (131 lines)
- `addons/cloud_storage_google/utils/cloud_storage_google_utils.py` (290 lines)
- `addons/cloud_storage_google/views/settings.xml` (26 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
