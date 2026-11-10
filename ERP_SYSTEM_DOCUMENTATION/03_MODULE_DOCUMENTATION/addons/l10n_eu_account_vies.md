# Module: l10n_eu_account_vies

- **Module ID:** MOD-185
- **Path:** `addons/l10n_eu_account_vies`
- **Manifest:** `addons/l10n_eu_account_vies/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


VAT validation for Partner's VAT numbers.
=========================================

After installing this module, values entered in the VAT field of Partners will
be validated using VIES for all supported countries. The country is inferred from the
2-letter country code that prefixes the VAT number, e.g. ``BE0477472701``
will be validated using the Belgian rules.

    * When the "VAT VIES Check" option is enabled (in the configuration of the user's
      Company), VAT numbers will be submitted to the online EU VIES database,
      which will truly verify that the number is valid and currently
      allocated to a EU company. This is a little bit slower than the simple
      off-line check, requires an Internet connection, and may not be available
      all the time. If the service is not available or does not support the
      requested country (e.g. for non-EU countries), a simple check will be performed
      instead.

Supported countries currently include EU countries, and a few non-EU countries
such as Chile, Colombia, Mexico, Norway or Russia. For unsupported countries,
only the country code will be validated.
    

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account"
  ],
  "data": [
    "data/ir_cron.xml",
    "views/res_partner_views.xml"
  ]
}
```

### Representative source files

- `addons/l10n_eu_account_vies/__init__.py` (7 lines)
- `addons/l10n_eu_account_vies/__manifest__.py` (34 lines)
- `addons/l10n_eu_account_vies/controllers/__init__.py` (1 lines)
- `addons/l10n_eu_account_vies/controllers/webhook.py` (23 lines)
- `addons/l10n_eu_account_vies/data/ir_cron.xml` (16 lines)
- `addons/l10n_eu_account_vies/data/neutralize.sql` (13 lines)
- `addons/l10n_eu_account_vies/i18n/bg.po` (126 lines)
- `addons/l10n_eu_account_vies/i18n/cs.po` (126 lines)
- `addons/l10n_eu_account_vies/i18n/da.po` (126 lines)
- `addons/l10n_eu_account_vies/i18n/de.po` (155 lines)
- `addons/l10n_eu_account_vies/i18n/el.po` (126 lines)
- `addons/l10n_eu_account_vies/i18n/es.po` (130 lines)
- `addons/l10n_eu_account_vies/i18n/et.po` (126 lines)
- `addons/l10n_eu_account_vies/i18n/fi.po` (157 lines)
- `addons/l10n_eu_account_vies/i18n/fr.po` (126 lines)
- `addons/l10n_eu_account_vies/i18n/hr.po` (126 lines)
- `addons/l10n_eu_account_vies/i18n/hu.po` (126 lines)
- `addons/l10n_eu_account_vies/i18n/it.po` (160 lines)
- `addons/l10n_eu_account_vies/i18n/l10n_eu_account_vies.pot` (126 lines)
- `addons/l10n_eu_account_vies/i18n/lt.po` (126 lines)
- `addons/l10n_eu_account_vies/i18n/lv.po` (126 lines)
- `addons/l10n_eu_account_vies/i18n/nl.po` (162 lines)
- `addons/l10n_eu_account_vies/i18n/pl.po` (126 lines)
- `addons/l10n_eu_account_vies/i18n/pt.po` (126 lines)
- `addons/l10n_eu_account_vies/i18n/ro.po` (126 lines)
- `addons/l10n_eu_account_vies/i18n/sk.po` (126 lines)
- `addons/l10n_eu_account_vies/i18n/sl.po` (126 lines)
- `addons/l10n_eu_account_vies/i18n/sv.po` (130 lines)
- `addons/l10n_eu_account_vies/models/__init__.py` (2 lines)
- `addons/l10n_eu_account_vies/models/res_country.py` (16 lines)
- `addons/l10n_eu_account_vies/models/res_partner.py` (208 lines)
- `addons/l10n_eu_account_vies/tests/__init__.py` (2 lines)
- `addons/l10n_eu_account_vies/tests/test_vat_numbers.py` (76 lines)
- `addons/l10n_eu_account_vies/tests/test_vies_iap.py` (163 lines)
- `addons/l10n_eu_account_vies/views/res_partner_views.xml` (19 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
