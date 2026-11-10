# Module: l10n_fr_pos_cert

- **Module ID:** MOD-197
- **Path:** `addons/l10n_fr_pos_cert`
- **Manifest:** `addons/l10n_fr_pos_cert/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This add-on brings the technical requirements of the French regulation CGI art. 286, I. 3° bis that stipulates certain criteria concerning the inalterability, security, storage and archiving of data related to sales to private individuals (B2C).
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Install it if you use the Point of Sale app to sell to individuals.

The module adds following features:

    Inalterability: deactivation of all the ways to cancel or modify key data of POS orders, invoices and journal entries

    Security: chaining algorithm to verify the inalterability

    Storage: automatic sales closings with computation of both period and cumulative totals (daily, monthly, annually)

    Access to download the mandatory Certificate of Conformity delivered by Odoo SA (only for Odoo Enterprise users)


Declared dependencies: `l10n_fr_account`, `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 16 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 8 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 11 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_fr_account",
    "point_of_sale"
  ],
  "data": [
    "views/pos_views.xml",
    "views/account_sale_closure.xml",
    "views/pos_inalterability_menuitem.xml",
    "views/res_config_settings_views.xml",
    "report/pos_hash_integrity.xml",
    "data/account_sale_closure_cron.xml",
    "receipt/pos_order_receipt.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_unit_tests": [
      "l10n_fr_pos_cert/static/tests/unit/**/*"
    ],
    "point_of_sale._assets_pos": [
      "l10n_fr_pos_cert/static/src/**/*"
    ],
    "web.assets_tests": [
      "l10n_fr_pos_cert/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_fr_pos_cert/__init__.py` (15 lines)
- `addons/l10n_fr_pos_cert/__manifest__.py` (49 lines)
- `addons/l10n_fr_pos_cert/data/account_sale_closure_cron.xml` (28 lines)
- `addons/l10n_fr_pos_cert/i18n/fr.po` (650 lines)
- `addons/l10n_fr_pos_cert/i18n/l10n_fr_pos_cert.pot` (586 lines)
- `addons/l10n_fr_pos_cert/models/__init__.py` (6 lines)
- `addons/l10n_fr_pos_cert/models/account_closing.py` (165 lines)
- `addons/l10n_fr_pos_cert/models/account_fiscal_position.py` (19 lines)
- `addons/l10n_fr_pos_cert/models/pos.py` (234 lines)
- `addons/l10n_fr_pos_cert/models/res_company.py` (99 lines)
- `addons/l10n_fr_pos_cert/receipt/__init__.py` (3 lines)
- `addons/l10n_fr_pos_cert/receipt/pos_order_receipt.py` (41 lines)
- `addons/l10n_fr_pos_cert/receipt/pos_order_receipt.xml` (26 lines)
- `addons/l10n_fr_pos_cert/report/__init__.py` (4 lines)
- `addons/l10n_fr_pos_cert/report/pos_hash_integrity.py` (20 lines)
- `addons/l10n_fr_pos_cert/report/pos_hash_integrity.xml` (112 lines)
- `addons/l10n_fr_pos_cert/security/ir.access.csv` (3 lines)
- `addons/l10n_fr_pos_cert/static/src/app/services/pos.js` (22 lines)
- `addons/l10n_fr_pos_cert/static/src/css/pos.css` (3 lines)
- `addons/l10n_fr_pos_cert/static/src/js/Chrome.js` (23 lines)
- `addons/l10n_fr_pos_cert/static/src/js/Popups/ClosePosPopup.js` (18 lines)
- `addons/l10n_fr_pos_cert/static/src/js/generate_printer_data.js` (17 lines)
- `addons/l10n_fr_pos_cert/static/src/js/pos_order_line.js` (23 lines)
- `addons/l10n_fr_pos_cert/static/src/xml/OrderSummary.xml` (18 lines)
- `addons/l10n_fr_pos_cert/static/tests/tours/l10n_fr_pos_cert_tour.js` (73 lines)
- `addons/l10n_fr_pos_cert/static/tests/unit/data/pos_config.data.js` (6 lines)
- `addons/l10n_fr_pos_cert/static/tests/unit/data/res_company.data.js` (26 lines)
- `addons/l10n_fr_pos_cert/static/tests/unit/data/res_country.data.js` (11 lines)
- `addons/l10n_fr_pos_cert/static/tests/unit/models/pos_order_line.test.js` (40 lines)
- `addons/l10n_fr_pos_cert/static/tests/unit/screens/feedback_screen.test.js` (13 lines)
- `addons/l10n_fr_pos_cert/tests/__init__.py` (6 lines)
- `addons/l10n_fr_pos_cert/tests/test_fr_pos.py` (17 lines)
- `addons/l10n_fr_pos_cert/tests/test_frontend.py` (44 lines)
- `addons/l10n_fr_pos_cert/tests/test_hash.py` (87 lines)
- `addons/l10n_fr_pos_cert/tests/test_string_to_hash.py` (116 lines)
- `addons/l10n_fr_pos_cert/views/account_sale_closure.xml` (67 lines)
- `addons/l10n_fr_pos_cert/views/pos_inalterability_menuitem.xml` (19 lines)
- `addons/l10n_fr_pos_cert/views/pos_views.xml` (15 lines)
- `addons/l10n_fr_pos_cert/views/res_config_settings_views.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
