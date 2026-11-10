# Module: l10n_fr_facturx_chorus_pro

- **Module ID:** MOD-191
- **Path:** `addons/l10n_fr_facturx_chorus_pro`
- **Manifest:** `addons/l10n_fr_facturx_chorus_pro/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Add support to fill three fields used when using Chorus Pro, especially when invoicing public services.


Declared dependencies: `account`, `account_edi_ubl_cii`, `l10n_fr_account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account",
    "account_edi_ubl_cii",
    "l10n_fr_account"
  ],
  "data": [
    "views/account_move_views.xml",
    "views/report_invoice.xml"
  ]
}
```

### Representative source files

- `addons/l10n_fr_facturx_chorus_pro/__init__.py` (4 lines)
- `addons/l10n_fr_facturx_chorus_pro/__manifest__.py` (21 lines)
- `addons/l10n_fr_facturx_chorus_pro/i18n/fr.po` (142 lines)
- `addons/l10n_fr_facturx_chorus_pro/i18n/l10n_fr_facturx_chorus_pro.pot` (130 lines)
- `addons/l10n_fr_facturx_chorus_pro/models/__init__.py` (5 lines)
- `addons/l10n_fr_facturx_chorus_pro/models/account_edi_xml_ubl_bis3.py` (94 lines)
- `addons/l10n_fr_facturx_chorus_pro/models/account_move.py` (10 lines)
- `addons/l10n_fr_facturx_chorus_pro/tests/__init__.py` (3 lines)
- `addons/l10n_fr_facturx_chorus_pro/tests/common.py` (26 lines)
- `addons/l10n_fr_facturx_chorus_pro/tests/test_files/export/bis3/invoice/be/test_invoice_customer_party_identifiers_partner_chorus_pro.xml` (140 lines)
- `addons/l10n_fr_facturx_chorus_pro/tests/test_files/export/bis3/invoice/fr/test_invoice_customer_party_identifiers_partner_chorus_pro.xml` (136 lines)
- `addons/l10n_fr_facturx_chorus_pro/tests/test_files/export/bis3/invoice/ignore_schema.xml` (26 lines)
- `addons/l10n_fr_facturx_chorus_pro/tests/test_ubl_export_bis3_be.py` (26 lines)
- `addons/l10n_fr_facturx_chorus_pro/tests/test_ubl_export_bis3_fr.py` (97 lines)
- `addons/l10n_fr_facturx_chorus_pro/views/account_move_views.xml` (19 lines)
- `addons/l10n_fr_facturx_chorus_pro/views/report_invoice.xml` (38 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
