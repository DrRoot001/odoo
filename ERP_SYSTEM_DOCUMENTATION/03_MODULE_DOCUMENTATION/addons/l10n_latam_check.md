# Module: l10n_latam_check

- **Module ID:** MOD-259
- **Path:** `addons/l10n_latam_check`
- **Manifest:** `addons/l10n_latam_check/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Checks Management


Own Checks Management
---------------------

Extends 'Check Printing Base' module to manage own checks with more features:

* allow using own checks that are not printed but filled manually by the user
* allow to use deferred or electronic checks
  * printing is disabled
  * check number is set manually by the user
* add an optional "Check Cash-In Date" for post-dated checks (deferred payments)
* add a menu to track own checks

Third Party Checks Management
-----------------------------

Add new "Third party check Management" feature.

There are 2 main Payment Methods additions:

* New Third Party Checks:

  * Payments of this payment method represent the check you get from a customer when getting paid (from an invoice or a manual payment)

* Existing Third Party check.

  * Payments of this payment method are to track moves of the check, for eg:

    * Use a check to pay a vendor
    * Deposit the check on the bank
    * Get the check back from the bank (rejection)
    * Get the check back from the vendor (a rejection or return)
    * Transfer the check from one third party check journal to the other (one shop to another)

  * Those operations can be done with multiple checks at once


Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 18 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 8 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account"
  ],
  "data": [
    "data/account_payment_method_data.xml",
    "wizard/l10n_latam_payment_mass_transfer_views.xml",
    "views/account_payment_view.xml",
    "views/l10n_latam_check_view.xml",
    "views/report_payment_receipt_templates.xml",
    "wizard/account_payment_register_views.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/l10n_latam_check/__init__.py` (2 lines)
- `addons/l10n_latam_check/__manifest__.py` (56 lines)
- `addons/l10n_latam_check/data/account_payment_method_data.xml` (40 lines)
- `addons/l10n_latam_check/i18n/es_419.po` (1,042 lines)
- `addons/l10n_latam_check/i18n/l10n_latam_check.pot` (911 lines)
- `addons/l10n_latam_check/i18n/pt_BR.po` (1,045 lines)
- `addons/l10n_latam_check/models/__init__.py` (7 lines)
- `addons/l10n_latam_check/models/account_chart_template.py` (78 lines)
- `addons/l10n_latam_check/models/account_journal.py` (50 lines)
- `addons/l10n_latam_check/models/account_move.py` (12 lines)
- `addons/l10n_latam_check/models/account_move_line.py` (8 lines)
- `addons/l10n_latam_check/models/account_payment.py` (272 lines)
- `addons/l10n_latam_check/models/account_payment_method.py` (15 lines)
- `addons/l10n_latam_check/models/l10n_latam_check.py` (276 lines)
- `addons/l10n_latam_check/security/ir.access.csv` (6 lines)
- `addons/l10n_latam_check/tests/__init__.py` (3 lines)
- `addons/l10n_latam_check/tests/common.py` (30 lines)
- `addons/l10n_latam_check/tests/test_own_checks.py` (179 lines)
- `addons/l10n_latam_check/tests/test_third_party_checks.py` (559 lines)
- `addons/l10n_latam_check/views/account_payment_view.xml` (52 lines)
- `addons/l10n_latam_check/views/l10n_latam_check_view.xml` (239 lines)
- `addons/l10n_latam_check/views/report_payment_receipt_templates.xml` (41 lines)
- `addons/l10n_latam_check/wizard/__init__.py` (5 lines)
- `addons/l10n_latam_check/wizard/account_payment_register.py` (83 lines)
- `addons/l10n_latam_check/wizard/account_payment_register_views.xml` (52 lines)
- `addons/l10n_latam_check/wizard/l10n_latam_payment_mass_transfer.py` (150 lines)
- `addons/l10n_latam_check/wizard/l10n_latam_payment_mass_transfer_views.xml` (35 lines)
- `addons/l10n_latam_check/wizard/l10n_latam_payment_register_check.py` (52 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
