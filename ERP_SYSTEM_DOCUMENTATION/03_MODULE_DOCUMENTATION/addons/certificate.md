# Module: certificate

- **Module ID:** MOD-048
- **Path:** `addons/certificate`
- **Manifest:** `addons/certificate/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Manage certificate

No manifest description declared.

Declared dependencies: `base_setup`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
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
    "base_setup"
  ],
  "data": [
    "views/certificate_views.xml",
    "views/key_views.xml",
    "views/action_menus.xml",
    "views/res_config_settings_view.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/certificate/__init__.py` (1 lines)
- `addons/certificate/__manifest__.py` (16 lines)
- `addons/certificate/data/neutralize.sql` (5 lines)
- `addons/certificate/i18n/ar.po` (551 lines)
- `addons/certificate/i18n/az.po` (536 lines)
- `addons/certificate/i18n/bg.po` (538 lines)
- `addons/certificate/i18n/bs.po` (536 lines)
- `addons/certificate/i18n/ca.po` (547 lines)
- `addons/certificate/i18n/certificate.pot` (528 lines)
- `addons/certificate/i18n/cs.po` (536 lines)
- `addons/certificate/i18n/da.po` (560 lines)
- `addons/certificate/i18n/de.po` (567 lines)
- `addons/certificate/i18n/el.po` (534 lines)
- `addons/certificate/i18n/es.po` (564 lines)
- `addons/certificate/i18n/es_419.po` (562 lines)
- `addons/certificate/i18n/et.po` (536 lines)
- `addons/certificate/i18n/fa.po` (536 lines)
- `addons/certificate/i18n/fi.po` (560 lines)
- `addons/certificate/i18n/fr.po` (564 lines)
- `addons/certificate/i18n/he.po` (537 lines)
- `addons/certificate/i18n/hi.po` (547 lines)
- `addons/certificate/i18n/hr.po` (537 lines)
- `addons/certificate/i18n/hu.po` (536 lines)
- `addons/certificate/i18n/id.po` (556 lines)
- `addons/certificate/i18n/it.po` (561 lines)
- `addons/certificate/i18n/ja.po` (557 lines)
- `addons/certificate/i18n/kab.po` (535 lines)
- `addons/certificate/i18n/ko.po` (549 lines)
- `addons/certificate/i18n/ku.po` (534 lines)
- `addons/certificate/i18n/lo.po` (543 lines)
- `addons/certificate/i18n/lt.po` (538 lines)
- `addons/certificate/i18n/lv.po` (538 lines)
- `addons/certificate/i18n/mn.po` (536 lines)
- `addons/certificate/i18n/my.po` (535 lines)
- `addons/certificate/i18n/nb.po` (536 lines)
- `addons/certificate/i18n/nl.po` (559 lines)
- `addons/certificate/i18n/pl.po` (560 lines)
- `addons/certificate/i18n/pt.po` (554 lines)
- `addons/certificate/i18n/pt_BR.po` (559 lines)
- `addons/certificate/i18n/ro.po` (555 lines)
- `addons/certificate/i18n/ru.po` (558 lines)
- `addons/certificate/i18n/sk.po` (537 lines)
- `addons/certificate/i18n/sl.po` (551 lines)
- `addons/certificate/i18n/sr@latin.po` (537 lines)
- `addons/certificate/i18n/sv.po` (558 lines)
- `addons/certificate/i18n/th.po` (542 lines)
- `addons/certificate/i18n/tr.po` (555 lines)
- `addons/certificate/i18n/uk.po` (553 lines)
- `addons/certificate/i18n/uz.po` (642 lines)
- `addons/certificate/i18n/vi.po` (550 lines)
- `addons/certificate/i18n/zh_CN.po` (541 lines)
- `addons/certificate/i18n/zh_TW.po` (544 lines)
- `addons/certificate/models/__init__.py` (2 lines)
- `addons/certificate/models/certificate.py` (647 lines)
- `addons/certificate/models/key.py` (485 lines)
- `addons/certificate/security/ir.access.csv` (5 lines)
- `addons/certificate/tests/__init__.py` (1 lines)
- `addons/certificate/tests/data/cert.pfx` (51 lines)
- `addons/certificate/tests/data/encrypted_private.key` (30 lines)
- `addons/certificate/tests/test_keys_certificates.py` (417 lines)
- `addons/certificate/tools/__init__.py` (1 lines)
- `addons/certificate/tools/certificate_adapter.py` (58 lines)
- `addons/certificate/views/action_menus.xml` (21 lines)
- `addons/certificate/views/certificate_views.xml` (66 lines)
- `addons/certificate/views/key_views.xml` (46 lines)
- `addons/certificate/views/res_config_settings_view.xml` (34 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
