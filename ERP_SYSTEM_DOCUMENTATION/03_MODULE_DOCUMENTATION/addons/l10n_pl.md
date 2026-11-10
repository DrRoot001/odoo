# Module: l10n_pl

- **Module ID:** MOD-298
- **Path:** `addons/l10n_pl`
- **Manifest:** `addons/l10n_pl/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the module to manage the accounting chart and taxes for Poland in Odoo.
==================================================================================

To jest moduł do tworzenia wzorcowego planu kont, podatków, obszarów podatkowych i
rejestrów podatkowych. Moduł ustawia też konta do kupna i sprzedaży towarów
zakładając, że wszystkie towary są w obrocie hurtowym.

Niniejszy moduł jest przeznaczony dla odoo 8.0.
Wewnętrzny numer wersji OpenGLOBE 1.02
    

Declared dependencies: `account`, `account_edi_ubl_cii`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 20 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 10 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 8 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account",
    "account_edi_ubl_cii"
  ],
  "data": [
    "data/l10n_pl.l10n_pl_tax_office.csv",
    "data/account.account.tag.csv",
    "data/account_tax_report_data.xml",
    "views/account_move_views.xml",
    "views/account_payment_view.xml",
    "views/product_views.xml",
    "views/res_config_settings_views.xml",
    "views/res_partner_views.xml",
    "wizard/account_payment_register_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_pl/__init__.py` (10 lines)
- `addons/l10n_pl/__manifest__.py` (43 lines)
- `addons/l10n_pl/data/account.account.tag.csv` (10 lines)
- `addons/l10n_pl/data/account_tax_report_data.xml` (628 lines)
- `addons/l10n_pl/data/l10n_pl.l10n_pl_tax_office.csv` (401 lines)
- `addons/l10n_pl/data/template/account.account-pl.csv` (240 lines)
- `addons/l10n_pl/data/template/account.fiscal.position-pl.csv` (5 lines)
- `addons/l10n_pl/data/template/account.tax-pl.csv` (129 lines)
- `addons/l10n_pl/data/template/account.tax.group-pl.csv` (5 lines)
- `addons/l10n_pl/demo/demo_company.xml` (43 lines)
- `addons/l10n_pl/i18n/l10n_pl.pot` (459 lines)
- `addons/l10n_pl/i18n/pl.po` (486 lines)
- `addons/l10n_pl/migrations/2.1/end-migrate.py` (13 lines)
- `addons/l10n_pl/migrations/9.0.2.0/pre-set_tags_and_taxes_updatable.py` (6 lines)
- `addons/l10n_pl/models/__init__.py` (10 lines)
- `addons/l10n_pl/models/account_move.py` (39 lines)
- `addons/l10n_pl/models/account_payment.py` (70 lines)
- `addons/l10n_pl/models/bank_account_verification.py` (330 lines)
- `addons/l10n_pl/models/l10n_pl_tax_office.py` (21 lines)
- `addons/l10n_pl/models/product.py` (25 lines)
- `addons/l10n_pl/models/res_company.py` (7 lines)
- `addons/l10n_pl/models/res_config_settings.py` (10 lines)
- `addons/l10n_pl/models/res_partner.py` (14 lines)
- `addons/l10n_pl/models/template_pl.py` (45 lines)
- `addons/l10n_pl/security/ir.access.csv` (3 lines)
- `addons/l10n_pl/tests/__init__.py` (2 lines)
- `addons/l10n_pl/tests/test_bank_account_verification.py` (518 lines)
- `addons/l10n_pl/tests/test_taxable_supply_date_with_lock_dates.py` (301 lines)
- `addons/l10n_pl/tests/utils/fake_response.json` (175 lines)
- `addons/l10n_pl/tests/utils/utils.py` (24 lines)
- `addons/l10n_pl/views/account_move_views.xml` (27 lines)
- `addons/l10n_pl/views/account_payment_view.xml` (19 lines)
- `addons/l10n_pl/views/product_views.xml` (15 lines)
- `addons/l10n_pl/views/res_config_settings_views.xml` (19 lines)
- `addons/l10n_pl/views/res_partner_views.xml` (19 lines)
- `addons/l10n_pl/wizard/__init__.py` (1 lines)
- `addons/l10n_pl/wizard/account_payment_register.py` (99 lines)
- `addons/l10n_pl/wizard/account_payment_register_views.xml` (32 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
