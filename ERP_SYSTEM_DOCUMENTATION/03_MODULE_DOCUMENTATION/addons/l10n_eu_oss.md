# Module: l10n_eu_oss

- **Module ID:** MOD-186
- **Path:** `addons/l10n_eu_oss`
- **Manifest:** `addons/l10n_eu_oss/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


EU One Stop Shop (OSS) VAT
==========================

From July 1st 2021, EU businesses that are selling goods within the EU above EUR 10 000 to buyers located in another EU Member State need to register and pay VAT in the buyers’ Member State.
Below this new EU-wide threshold you can continue to apply the domestic rules for VAT on your cross-border sales. In order to simplify the application of this EU directive, the One Stop Shop (OSS) registration scheme allows businesses to make a unique tax declaration.

This module makes it possible by helping with the creation of the required EU fiscal positions and taxes in order to automatically apply and record the required taxes.

All you have to do is check that the proposed mapping is suitable for the products and services you sell.

References
++++++++++
Council Directive (EU) 2017/2455 Council Directive (EU) 2019/1995
Council Implementing Regulation (EU) 2019/2026

    

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 11 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 7 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account"
  ],
  "data": [
    "data/account_account_tag.xml"
  ]
}
```

### Representative source files

- `addons/l10n_eu_oss/__init__.py` (7 lines)
- `addons/l10n_eu_oss/__manifest__.py` (30 lines)
- `addons/l10n_eu_oss/data/account_account_tag.xml` (34 lines)
- `addons/l10n_eu_oss/i18n/bg.po` (87 lines)
- `addons/l10n_eu_oss/i18n/cs.po` (86 lines)
- `addons/l10n_eu_oss/i18n/da.po` (101 lines)
- `addons/l10n_eu_oss/i18n/de.po` (128 lines)
- `addons/l10n_eu_oss/i18n/el.po` (87 lines)
- `addons/l10n_eu_oss/i18n/es.po` (116 lines)
- `addons/l10n_eu_oss/i18n/et.po` (87 lines)
- `addons/l10n_eu_oss/i18n/fi.po` (124 lines)
- `addons/l10n_eu_oss/i18n/fr.po` (100 lines)
- `addons/l10n_eu_oss/i18n/hr.po` (88 lines)
- `addons/l10n_eu_oss/i18n/hu.po` (87 lines)
- `addons/l10n_eu_oss/i18n/it.po` (126 lines)
- `addons/l10n_eu_oss/i18n/l10n_eu_oss.pot` (75 lines)
- `addons/l10n_eu_oss/i18n/lt.po` (88 lines)
- `addons/l10n_eu_oss/i18n/lv.po` (87 lines)
- `addons/l10n_eu_oss/i18n/nl.po` (100 lines)
- `addons/l10n_eu_oss/i18n/pl.po` (87 lines)
- `addons/l10n_eu_oss/i18n/pt.po` (87 lines)
- `addons/l10n_eu_oss/i18n/ro.po` (89 lines)
- `addons/l10n_eu_oss/i18n/sk.po` (87 lines)
- `addons/l10n_eu_oss/i18n/sl.po` (88 lines)
- `addons/l10n_eu_oss/i18n/sv.po` (101 lines)
- `addons/l10n_eu_oss/models/__init__.py` (9 lines)
- `addons/l10n_eu_oss/models/eu_account_map.py` (15 lines)
- `addons/l10n_eu_oss/models/eu_field_map.py` (25 lines)
- `addons/l10n_eu_oss/models/eu_tag_map.py` (238 lines)
- `addons/l10n_eu_oss/models/eu_tax_map.py` (2,409 lines)
- `addons/l10n_eu_oss/models/res_company.py` (253 lines)
- `addons/l10n_eu_oss/models/res_config_settings.py` (16 lines)
- `addons/l10n_eu_oss/tests/__init__.py` (3 lines)
- `addons/l10n_eu_oss/tests/test_oss.py` (206 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
