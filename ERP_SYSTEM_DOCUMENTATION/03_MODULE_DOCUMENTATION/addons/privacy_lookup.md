# Module: privacy_lookup

- **Module ID:** MOD-469
- **Path:** `addons/privacy_lookup`
- **Manifest:** `addons/privacy_lookup/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

No manifest description declared.

Declared dependencies: `mail`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mail"
  ],
  "data": [
    "wizard/privacy_lookup_wizard_views.xml",
    "views/privacy_log_views.xml",
    "data/ir_actions_server_data.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/privacy_lookup/__init__.py` (5 lines)
- `addons/privacy_lookup/__manifest__.py` (16 lines)
- `addons/privacy_lookup/data/ir_actions_server_data.xml` (24 lines)
- `addons/privacy_lookup/i18n/ar.po` (324 lines)
- `addons/privacy_lookup/i18n/az.po` (321 lines)
- `addons/privacy_lookup/i18n/bg.po` (322 lines)
- `addons/privacy_lookup/i18n/bs.po` (349 lines)
- `addons/privacy_lookup/i18n/ca.po` (322 lines)
- `addons/privacy_lookup/i18n/cs.po` (322 lines)
- `addons/privacy_lookup/i18n/da.po` (344 lines)
- `addons/privacy_lookup/i18n/de.po` (325 lines)
- `addons/privacy_lookup/i18n/el.po` (322 lines)
- `addons/privacy_lookup/i18n/es.po` (326 lines)
- `addons/privacy_lookup/i18n/es_419.po` (325 lines)
- `addons/privacy_lookup/i18n/et.po` (322 lines)
- `addons/privacy_lookup/i18n/fa.po` (321 lines)
- `addons/privacy_lookup/i18n/fi.po` (324 lines)
- `addons/privacy_lookup/i18n/fr.po` (325 lines)
- `addons/privacy_lookup/i18n/he.po` (323 lines)
- `addons/privacy_lookup/i18n/hi.po` (327 lines)
- `addons/privacy_lookup/i18n/hr.po` (348 lines)
- `addons/privacy_lookup/i18n/hu.po` (323 lines)
- `addons/privacy_lookup/i18n/id.po` (325 lines)
- `addons/privacy_lookup/i18n/it.po` (325 lines)
- `addons/privacy_lookup/i18n/ja.po` (323 lines)
- `addons/privacy_lookup/i18n/kab.po` (338 lines)
- `addons/privacy_lookup/i18n/ko.po` (322 lines)
- `addons/privacy_lookup/i18n/ku.po` (321 lines)
- `addons/privacy_lookup/i18n/lo.po` (322 lines)
- `addons/privacy_lookup/i18n/lt.po` (323 lines)
- `addons/privacy_lookup/i18n/lv.po` (349 lines)
- `addons/privacy_lookup/i18n/mn.po` (321 lines)
- `addons/privacy_lookup/i18n/my.po` (323 lines)
- `addons/privacy_lookup/i18n/nb.po` (323 lines)
- `addons/privacy_lookup/i18n/nl.po` (324 lines)
- `addons/privacy_lookup/i18n/pl.po` (325 lines)
- `addons/privacy_lookup/i18n/privacy_lookup.pot` (317 lines)
- `addons/privacy_lookup/i18n/pt.po` (324 lines)
- `addons/privacy_lookup/i18n/pt_BR.po` (323 lines)
- `addons/privacy_lookup/i18n/ro.po` (325 lines)
- `addons/privacy_lookup/i18n/ru.po` (325 lines)
- `addons/privacy_lookup/i18n/sk.po` (349 lines)
- `addons/privacy_lookup/i18n/sl.po` (324 lines)
- `addons/privacy_lookup/i18n/sr@latin.po` (323 lines)
- `addons/privacy_lookup/i18n/sv.po` (324 lines)
- `addons/privacy_lookup/i18n/th.po` (322 lines)
- `addons/privacy_lookup/i18n/tr.po` (326 lines)
- `addons/privacy_lookup/i18n/uk.po` (323 lines)
- `addons/privacy_lookup/i18n/uz.po` (381 lines)
- `addons/privacy_lookup/i18n/vi.po` (323 lines)
- `addons/privacy_lookup/i18n/zh_CN.po` (322 lines)
- `addons/privacy_lookup/i18n/zh_TW.po` (324 lines)
- `addons/privacy_lookup/models/__init__.py` (5 lines)
- `addons/privacy_lookup/models/privacy_log.py` (48 lines)
- `addons/privacy_lookup/models/res_partner.py` (17 lines)
- `addons/privacy_lookup/security/ir.access.csv` (4 lines)
- `addons/privacy_lookup/tests/__init__.py` (4 lines)
- `addons/privacy_lookup/tests/test_privacy_wizard.py` (153 lines)
- `addons/privacy_lookup/views/privacy_log_views.xml` (73 lines)
- `addons/privacy_lookup/wizard/__init__.py` (4 lines)
- `addons/privacy_lookup/wizard/privacy_lookup_wizard.py` (327 lines)
- `addons/privacy_lookup/wizard/privacy_lookup_wizard_views.xml` (113 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
