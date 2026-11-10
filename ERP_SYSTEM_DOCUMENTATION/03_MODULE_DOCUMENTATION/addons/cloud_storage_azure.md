# Module: cloud_storage_azure

- **Module ID:** MOD-050
- **Path:** `addons/cloud_storage_azure`
- **Manifest:** `addons/cloud_storage_azure/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Store chatter attachments in the Azure cloud

No manifest description declared.

Declared dependencies: `cloud_storage`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 11 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
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
  ]
}
```

### Representative source files

- `addons/cloud_storage_azure/__init__.py` (17 lines)
- `addons/cloud_storage_azure/__manifest__.py` (14 lines)
- `addons/cloud_storage_azure/data/neutralize.sql` (7 lines)
- `addons/cloud_storage_azure/i18n/ar.po` (130 lines)
- `addons/cloud_storage_azure/i18n/az.po` (122 lines)
- `addons/cloud_storage_azure/i18n/bg.po` (122 lines)
- `addons/cloud_storage_azure/i18n/bs.po` (124 lines)
- `addons/cloud_storage_azure/i18n/ca.po` (123 lines)
- `addons/cloud_storage_azure/i18n/cloud_storage_azure.pot` (118 lines)
- `addons/cloud_storage_azure/i18n/cs.po` (123 lines)
- `addons/cloud_storage_azure/i18n/da.po` (132 lines)
- `addons/cloud_storage_azure/i18n/de.po` (133 lines)
- `addons/cloud_storage_azure/i18n/el.po` (123 lines)
- `addons/cloud_storage_azure/i18n/es.po` (131 lines)
- `addons/cloud_storage_azure/i18n/es_419.po` (131 lines)
- `addons/cloud_storage_azure/i18n/et.po` (128 lines)
- `addons/cloud_storage_azure/i18n/fa.po` (122 lines)
- `addons/cloud_storage_azure/i18n/fi.po` (130 lines)
- `addons/cloud_storage_azure/i18n/fr.po` (132 lines)
- `addons/cloud_storage_azure/i18n/he.po` (123 lines)
- `addons/cloud_storage_azure/i18n/hi.po` (124 lines)
- `addons/cloud_storage_azure/i18n/hr.po` (123 lines)
- `addons/cloud_storage_azure/i18n/hu.po` (123 lines)
- `addons/cloud_storage_azure/i18n/id.po` (129 lines)
- `addons/cloud_storage_azure/i18n/it.po` (129 lines)
- `addons/cloud_storage_azure/i18n/ja.po` (130 lines)
- `addons/cloud_storage_azure/i18n/kab.po` (123 lines)
- `addons/cloud_storage_azure/i18n/ko.po` (126 lines)
- `addons/cloud_storage_azure/i18n/ku.po` (122 lines)
- `addons/cloud_storage_azure/i18n/lo.po` (121 lines)
- `addons/cloud_storage_azure/i18n/lt.po` (124 lines)
- `addons/cloud_storage_azure/i18n/lv.po` (124 lines)
- `addons/cloud_storage_azure/i18n/mn.po` (122 lines)
- `addons/cloud_storage_azure/i18n/my.po` (122 lines)
- `addons/cloud_storage_azure/i18n/nb.po` (123 lines)
- `addons/cloud_storage_azure/i18n/nl.po` (129 lines)
- `addons/cloud_storage_azure/i18n/pl.po` (132 lines)
- `addons/cloud_storage_azure/i18n/pt.po` (130 lines)
- `addons/cloud_storage_azure/i18n/pt_BR.po` (129 lines)
- `addons/cloud_storage_azure/i18n/ro.po` (130 lines)
- `addons/cloud_storage_azure/i18n/ru.po` (132 lines)
- `addons/cloud_storage_azure/i18n/sk.po` (123 lines)
- `addons/cloud_storage_azure/i18n/sl.po` (130 lines)
- `addons/cloud_storage_azure/i18n/sr@latin.po` (123 lines)
- `addons/cloud_storage_azure/i18n/sv.po` (130 lines)
- `addons/cloud_storage_azure/i18n/th.po` (128 lines)
- `addons/cloud_storage_azure/i18n/tr.po` (131 lines)
- `addons/cloud_storage_azure/i18n/uk.po` (123 lines)
- `addons/cloud_storage_azure/i18n/uz.po` (148 lines)
- `addons/cloud_storage_azure/i18n/vi.po` (131 lines)
- `addons/cloud_storage_azure/i18n/zh_CN.po` (128 lines)
- `addons/cloud_storage_azure/i18n/zh_TW.po` (130 lines)
- `addons/cloud_storage_azure/models/__init__.py` (4 lines)
- `addons/cloud_storage_azure/models/ir_attachment.py` (128 lines)
- `addons/cloud_storage_azure/models/res_config_settings.py` (105 lines)
- `addons/cloud_storage_azure/tests/__init__.py` (4 lines)
- `addons/cloud_storage_azure/tests/test_cloud_storage_azure.py` (353 lines)
- `addons/cloud_storage_azure/tests/test_cloud_storage_azure_attachment_controller.py` (103 lines)
- `addons/cloud_storage_azure/utils/__init__.py` (3 lines)
- `addons/cloud_storage_azure/utils/cleanup_cloud_storage_azure.py` (140 lines)
- `addons/cloud_storage_azure/utils/cloud_storage_azure_utils.py` (393 lines)
- `addons/cloud_storage_azure/views/settings.xml` (32 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
