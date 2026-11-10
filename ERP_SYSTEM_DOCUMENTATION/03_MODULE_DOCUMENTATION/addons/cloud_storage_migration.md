# Module: cloud_storage_migration

- **Module ID:** MOD-052
- **Path:** `addons/cloud_storage_migration`
- **Manifest:** `addons/cloud_storage_migration/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Migrate local attachments to cloud storage

No manifest description declared.

Declared dependencies: `cloud_storage`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "cloud_storage"
  ],
  "data": [
    "data/data.xml",
    "data/ir_cron.xml",
    "views/cloud_storage_migration_report_views.xml",
    "views/res_config_settings.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/cloud_storage_migration/__init__.py` (3 lines)
- `addons/cloud_storage_migration/__manifest__.py` (17 lines)
- `addons/cloud_storage_migration/data/data.xml` (33 lines)
- `addons/cloud_storage_migration/data/ir_cron.xml` (16 lines)
- `addons/cloud_storage_migration/i18n/ar.po` (303 lines)
- `addons/cloud_storage_migration/i18n/az.po` (287 lines)
- `addons/cloud_storage_migration/i18n/bg.po` (287 lines)
- `addons/cloud_storage_migration/i18n/bs.po` (288 lines)
- `addons/cloud_storage_migration/i18n/ca.po` (287 lines)
- `addons/cloud_storage_migration/i18n/cloud_storage_migration.pot` (284 lines)
- `addons/cloud_storage_migration/i18n/cs.po` (288 lines)
- `addons/cloud_storage_migration/i18n/da.po` (311 lines)
- `addons/cloud_storage_migration/i18n/de.po` (313 lines)
- `addons/cloud_storage_migration/i18n/el.po` (287 lines)
- `addons/cloud_storage_migration/i18n/es.po` (316 lines)
- `addons/cloud_storage_migration/i18n/es_419.po` (317 lines)
- `addons/cloud_storage_migration/i18n/et.po` (287 lines)
- `addons/cloud_storage_migration/i18n/fa.po` (287 lines)
- `addons/cloud_storage_migration/i18n/fi.po` (302 lines)
- `addons/cloud_storage_migration/i18n/fr.po` (314 lines)
- `addons/cloud_storage_migration/i18n/he.po` (288 lines)
- `addons/cloud_storage_migration/i18n/hi.po` (287 lines)
- `addons/cloud_storage_migration/i18n/hr.po` (288 lines)
- `addons/cloud_storage_migration/i18n/hu.po` (287 lines)
- `addons/cloud_storage_migration/i18n/id.po` (306 lines)
- `addons/cloud_storage_migration/i18n/it.po` (312 lines)
- `addons/cloud_storage_migration/i18n/ja.po` (310 lines)
- `addons/cloud_storage_migration/i18n/kab.po` (287 lines)
- `addons/cloud_storage_migration/i18n/ko.po` (288 lines)
- `addons/cloud_storage_migration/i18n/ku.po` (287 lines)
- `addons/cloud_storage_migration/i18n/lo.po` (297 lines)
- `addons/cloud_storage_migration/i18n/lt.po` (289 lines)
- `addons/cloud_storage_migration/i18n/lv.po` (288 lines)
- `addons/cloud_storage_migration/i18n/mn.po` (287 lines)
- `addons/cloud_storage_migration/i18n/my.po` (287 lines)
- `addons/cloud_storage_migration/i18n/nb.po` (287 lines)
- `addons/cloud_storage_migration/i18n/nl.po` (308 lines)
- `addons/cloud_storage_migration/i18n/pl.po` (312 lines)
- `addons/cloud_storage_migration/i18n/pt.po` (287 lines)
- `addons/cloud_storage_migration/i18n/pt_BR.po` (309 lines)
- `addons/cloud_storage_migration/i18n/ro.po` (288 lines)
- `addons/cloud_storage_migration/i18n/ru.po` (308 lines)
- `addons/cloud_storage_migration/i18n/sk.po` (287 lines)
- `addons/cloud_storage_migration/i18n/sl.po` (288 lines)
- `addons/cloud_storage_migration/i18n/sr@latin.po` (288 lines)
- `addons/cloud_storage_migration/i18n/sv.po` (288 lines)
- `addons/cloud_storage_migration/i18n/th.po` (288 lines)
- `addons/cloud_storage_migration/i18n/tr.po` (306 lines)
- `addons/cloud_storage_migration/i18n/uk.po` (288 lines)
- `addons/cloud_storage_migration/i18n/uz.po` (287 lines)
- `addons/cloud_storage_migration/i18n/vi.po` (287 lines)
- `addons/cloud_storage_migration/i18n/zh_CN.po` (288 lines)
- `addons/cloud_storage_migration/i18n/zh_TW.po` (288 lines)
- `addons/cloud_storage_migration/models/__init__.py` (4 lines)
- `addons/cloud_storage_migration/models/cloud_storage_migration_report.py` (98 lines)
- `addons/cloud_storage_migration/models/ir_attachment.py` (186 lines)
- `addons/cloud_storage_migration/models/res_config_settings.py` (79 lines)
- `addons/cloud_storage_migration/security/ir.access.csv` (2 lines)
- `addons/cloud_storage_migration/tests/__init__.py` (3 lines)
- `addons/cloud_storage_migration/tests/test_res_config_settings.py` (60 lines)
- `addons/cloud_storage_migration/views/cloud_storage_migration_report_views.xml` (37 lines)
- `addons/cloud_storage_migration/views/res_config_settings.xml` (52 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
