# Module: auth_ldap

- **Module ID:** MOD-020
- **Path:** `addons/auth_ldap`
- **Manifest:** `addons/auth_ldap/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

No manifest description declared.

Declared dependencies: `base`, `base_setup`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base",
    "base_setup"
  ],
  "data": [
    "views/ldap_installer_views.xml",
    "views/res_config_settings_views.xml",
    "security/ir.access.csv"
  ],
  "external_dependencies": {
    "python": [
      "python-ldap"
    ],
    "apt": {
      "python-ldap": "python3-ldap"
    }
  }
}
```

### Representative source files

- `addons/auth_ldap/README.rst` (66 lines)
- `addons/auth_ldap/__init__.py` (3 lines)
- `addons/auth_ldap/__manifest__.py` (21 lines)
- `addons/auth_ldap/i18n/af.po` (382 lines)
- `addons/auth_ldap/i18n/am.po` (381 lines)
- `addons/auth_ldap/i18n/ar.po` (416 lines)
- `addons/auth_ldap/i18n/auth_ldap.pot` (352 lines)
- `addons/auth_ldap/i18n/az.po` (382 lines)
- `addons/auth_ldap/i18n/bg.po` (393 lines)
- `addons/auth_ldap/i18n/bs.po` (386 lines)
- `addons/auth_ldap/i18n/ca.po` (417 lines)
- `addons/auth_ldap/i18n/cs.po` (417 lines)
- `addons/auth_ldap/i18n/da.po` (417 lines)
- `addons/auth_ldap/i18n/de.po` (516 lines)
- `addons/auth_ldap/i18n/el.po` (405 lines)
- `addons/auth_ldap/i18n/es.po` (510 lines)
- `addons/auth_ldap/i18n/es_419.po` (509 lines)
- `addons/auth_ldap/i18n/es_CL.po` (67 lines)
- `addons/auth_ldap/i18n/et.po` (399 lines)
- `addons/auth_ldap/i18n/eu.po` (381 lines)
- `addons/auth_ldap/i18n/fa.po` (388 lines)
- `addons/auth_ldap/i18n/fi.po` (512 lines)
- `addons/auth_ldap/i18n/fo.po` (381 lines)
- `addons/auth_ldap/i18n/fr.po` (517 lines)
- `addons/auth_ldap/i18n/fr_BE.po` (58 lines)
- `addons/auth_ldap/i18n/fr_CA.po` (61 lines)
- `addons/auth_ldap/i18n/gl.po` (381 lines)
- `addons/auth_ldap/i18n/gu.po` (383 lines)
- `addons/auth_ldap/i18n/he.po` (403 lines)
- `addons/auth_ldap/i18n/hi.po` (382 lines)
- `addons/auth_ldap/i18n/hr.po` (396 lines)
- `addons/auth_ldap/i18n/hu.po` (399 lines)
- `addons/auth_ldap/i18n/id.po` (508 lines)
- `addons/auth_ldap/i18n/is.po` (384 lines)
- `addons/auth_ldap/i18n/it.po` (514 lines)
- `addons/auth_ldap/i18n/ja.po` (492 lines)
- `addons/auth_ldap/i18n/ka.po` (381 lines)
- `addons/auth_ldap/i18n/kab.po` (383 lines)
- `addons/auth_ldap/i18n/km.po` (382 lines)
- `addons/auth_ldap/i18n/ko.po` (412 lines)
- `addons/auth_ldap/i18n/ku.po` (382 lines)
- `addons/auth_ldap/i18n/lo.po` (470 lines)
- `addons/auth_ldap/i18n/lt.po` (403 lines)
- `addons/auth_ldap/i18n/lv.po` (384 lines)
- `addons/auth_ldap/i18n/mk.po` (381 lines)
- `addons/auth_ldap/i18n/ml_IN.po` (381 lines)
- `addons/auth_ldap/i18n/mn.po` (397 lines)
- `addons/auth_ldap/i18n/my.po` (383 lines)
- `addons/auth_ldap/i18n/nb.po` (394 lines)
- `addons/auth_ldap/i18n/nl.po` (492 lines)
- `addons/auth_ldap/i18n/pl.po` (511 lines)
- `addons/auth_ldap/i18n/pt.po` (413 lines)
- `addons/auth_ldap/i18n/pt_BR.po` (515 lines)
- `addons/auth_ldap/i18n/ro.po` (413 lines)
- `addons/auth_ldap/i18n/ru.po` (417 lines)
- `addons/auth_ldap/i18n/sk.po` (395 lines)
- `addons/auth_ldap/i18n/sl.po` (411 lines)
- `addons/auth_ldap/i18n/sq.po` (381 lines)
- `addons/auth_ldap/i18n/sr@latin.po` (415 lines)
- `addons/auth_ldap/i18n/sv.po` (418 lines)
- `addons/auth_ldap/i18n/ta.po` (382 lines)
- `addons/auth_ldap/i18n/th.po` (465 lines)
- `addons/auth_ldap/i18n/tr.po` (414 lines)
- `addons/auth_ldap/i18n/uk.po` (418 lines)
- `addons/auth_ldap/i18n/uz.po` (457 lines)
- `addons/auth_ldap/i18n/vi.po` (416 lines)
- `addons/auth_ldap/i18n/zh_CN.po` (406 lines)
- `addons/auth_ldap/i18n/zh_TW.po` (401 lines)
- `addons/auth_ldap/models/__init__.py` (6 lines)
- `addons/auth_ldap/models/res_company.py` (11 lines)
- `addons/auth_ldap/models/res_company_ldap.py` (377 lines)
- `addons/auth_ldap/models/res_config_settings.py` (10 lines)
- `addons/auth_ldap/models/res_users.py` (69 lines)
- `addons/auth_ldap/security/ir.access.csv` (2 lines)
- `addons/auth_ldap/tests/__init__.py` (1 lines)
- `addons/auth_ldap/tests/test_auth_ldap.py` (292 lines)
- `addons/auth_ldap/views/ldap_installer_views.xml` (60 lines)
- `addons/auth_ldap/views/res_config_settings_views.xml` (16 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
