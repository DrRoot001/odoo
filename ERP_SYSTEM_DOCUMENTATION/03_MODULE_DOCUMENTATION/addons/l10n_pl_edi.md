# Module: l10n_pl_edi

- **Module ID:** MOD-299
- **Path:** `addons/l10n_pl_edi`
- **Manifest:** `addons/l10n_pl_edi/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['l10n_pl']`
- **License:** `LGPL-3`

## Purpose and dependencies

Support for FA(3) electronic invoices in Poland via KSeF

Export FA(3) compliant XML invoices and prepare for integration with KSeF.

Declared dependencies: `l10n_pl`, `certificate`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 15 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 7 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 19 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_pl",
    "certificate"
  ],
  "data": [
    "views/account_move_views.xml",
    "views/report_invoice.xml",
    "views/res_config_settings_views.xml",
    "data/ir_cron_data.xml",
    "data/fa3_template.xml"
  ],
  "demo": [
    "demo/account_invoice_demo.xml"
  ]
}
```

### Representative source files

- `addons/l10n_pl_edi/__init__.py` (2 lines)
- `addons/l10n_pl_edi/__manifest__.py` (23 lines)
- `addons/l10n_pl_edi/data/fa3_schema.xsd` (3,950 lines)
- `addons/l10n_pl_edi/data/fa3_template.xml` (352 lines)
- `addons/l10n_pl_edi/data/ir_cron_data.xml` (38 lines)
- `addons/l10n_pl_edi/data/neutralize.sql` (31 lines)
- `addons/l10n_pl_edi/demo/account_invoice_demo.xml` (14 lines)
- `addons/l10n_pl_edi/exceptions.py` (8 lines)
- `addons/l10n_pl_edi/i18n/l10n_pl_edi.pot` (722 lines)
- `addons/l10n_pl_edi/i18n/pl.po` (725 lines)
- `addons/l10n_pl_edi/models/__init__.py` (6 lines)
- `addons/l10n_pl_edi/models/account_journal.py` (16 lines)
- `addons/l10n_pl_edi/models/account_move.py` (814 lines)
- `addons/l10n_pl_edi/models/account_move_send.py` (137 lines)
- `addons/l10n_pl_edi/models/res_company.py` (43 lines)
- `addons/l10n_pl_edi/models/res_config_settings.py` (117 lines)
- `addons/l10n_pl_edi/models/res_partner.py` (20 lines)
- `addons/l10n_pl_edi/tests/__init__.py` (1 lines)
- `addons/l10n_pl_edi/tests/certificate/l10n_pl_edi_test.key` (8 lines)
- `addons/l10n_pl_edi/tests/certificate/l10n_pl_edi_test.pem` (18 lines)
- `addons/l10n_pl_edi/tests/export_xmls/fa3_bill.xml` (100 lines)
- `addons/l10n_pl_edi/tests/export_xmls/fa3_invoice_foreign_currency.xml` (72 lines)
- `addons/l10n_pl_edi/tests/export_xmls/full_paid_invoice.xml` (69 lines)
- `addons/l10n_pl_edi/tests/export_xmls/partial_paid_invoice_bank_cash.xml` (81 lines)
- `addons/l10n_pl_edi/tests/export_xmls/standard_fa3_format_credit_note_reverse_charge.xml` (86 lines)
- `addons/l10n_pl_edi/tests/export_xmls/standard_fa3_format_invoice_reverse_charge.xml` (81 lines)
- `addons/l10n_pl_edi/tests/export_xmls/standerd_fa3_credit_note.xml` (79 lines)
- `addons/l10n_pl_edi/tests/export_xmls/standert_fa3_format.xml` (75 lines)
- `addons/l10n_pl_edi/tests/import_xmls/fa3_standard_bill.xml` (100 lines)
- `addons/l10n_pl_edi/tests/import_xmls/invoice_from_foreign_country.xml` (82 lines)
- `addons/l10n_pl_edi/tests/import_xmls/invoice_with_discount.xml` (93 lines)
- `addons/l10n_pl_edi/tests/import_xmls/invoice_with_net_and_gross_unit_price.xml` (100 lines)
- `addons/l10n_pl_edi/tests/import_xmls/invoice_with_zero_value_line_missing_unit_prices.xml` (61 lines)
- `addons/l10n_pl_edi/tests/test_l10n_pl_edi.py` (1,168 lines)
- `addons/l10n_pl_edi/tools/__init__.py` (2 lines)
- `addons/l10n_pl_edi/tools/ksef_api_service.py` (367 lines)
- `addons/l10n_pl_edi/tools/xades_signer.py` (119 lines)
- `addons/l10n_pl_edi/views/account_move_views.xml` (52 lines)
- `addons/l10n_pl_edi/views/report_invoice.xml` (17 lines)
- `addons/l10n_pl_edi/views/res_config_settings_views.xml` (28 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
