# Module: l10n_ro_edi

- **Module ID:** MOD-305
- **Path:** `addons/l10n_ro_edi`
- **Manifest:** `addons/l10n_ro_edi/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

E-Invoice implementation for Romania


E-invoice implementation for Romania
    

Declared dependencies: `account_edi_ubl_cii`, `l10n_ro`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 22 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 11 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 15 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 2 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account_edi_ubl_cii",
    "l10n_ro"
  ],
  "data": [
    "data/ir_cron.xml",
    "data/l10n_ro.cpv.code.csv",
    "views/account_move_views.xml",
    "views/res_config_settings_views.xml",
    "views/product_views.xml",
    "wizard/account_move_fetch_invoices_wizard.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "l10n_ro_edi/static/src/components/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_ro_edi/__init__.py` (7 lines)
- `addons/l10n_ro_edi/__manifest__.py` (30 lines)
- `addons/l10n_ro_edi/controllers/__init__.py` (1 lines)
- `addons/l10n_ro_edi/controllers/main.py` (92 lines)
- `addons/l10n_ro_edi/data/ir_cron.xml` (25 lines)
- `addons/l10n_ro_edi/data/l10n_ro.cpv.code.csv` (9,455 lines)
- `addons/l10n_ro_edi/data/neutralize.sql` (7 lines)
- `addons/l10n_ro_edi/i18n/l10n_ro_edi.pot` (849 lines)
- `addons/l10n_ro_edi/i18n/ro.po` (920 lines)
- `addons/l10n_ro_edi/models/__init__.py` (10 lines)
- `addons/l10n_ro_edi/models/account_edi_xml_ubl_ciusro.py` (244 lines)
- `addons/l10n_ro_edi/models/account_move.py` (537 lines)
- `addons/l10n_ro_edi/models/account_move_send.py` (78 lines)
- `addons/l10n_ro_edi/models/ciusro_document.py` (58 lines)
- `addons/l10n_ro_edi/models/cpv_code.py` (19 lines)
- `addons/l10n_ro_edi/models/product.py` (11 lines)
- `addons/l10n_ro_edi/models/res_company.py` (169 lines)
- `addons/l10n_ro_edi/models/res_config_settings.py` (24 lines)
- `addons/l10n_ro_edi/models/res_partner.py` (43 lines)
- `addons/l10n_ro_edi/models/utils.py` (305 lines)
- `addons/l10n_ro_edi/security/ir.access.csv` (5 lines)
- `addons/l10n_ro_edi/static/src/components/fetch_invoices.js` (44 lines)
- `addons/l10n_ro_edi/static/src/components/fetch_invoices.xml` (8 lines)
- `addons/l10n_ro_edi/tests/__init__.py` (3 lines)
- `addons/l10n_ro_edi/tests/common.py` (90 lines)
- `addons/l10n_ro_edi/tests/test_files/from_odoo/ciusro_in_invoice.xml` (141 lines)
- `addons/l10n_ro_edi/tests/test_files/from_odoo/ciusro_out_invoice.xml` (174 lines)
- `addons/l10n_ro_edi/tests/test_files/from_odoo/ciusro_out_invoice_characters_limit.xml` (155 lines)
- `addons/l10n_ro_edi/tests/test_files/from_odoo/ciusro_out_invoice_cpv_code.xml` (179 lines)
- `addons/l10n_ro_edi/tests/test_files/from_odoo/ciusro_out_invoice_defaults.xml` (174 lines)
- `addons/l10n_ro_edi/tests/test_files/from_odoo/ciusro_out_invoice_different_currency.xml` (177 lines)
- `addons/l10n_ro_edi/tests/test_files/from_odoo/ciusro_out_invoice_no_prefix_company_registry.xml` (173 lines)
- `addons/l10n_ro_edi/tests/test_files/from_odoo/ciusro_out_invoice_no_prefix_vat.xml` (173 lines)
- `addons/l10n_ro_edi/tests/test_files/from_odoo/ciusro_out_refund.xml` (174 lines)
- `addons/l10n_ro_edi/tests/test_ro_edi.py` (274 lines)
- `addons/l10n_ro_edi/tests/test_xml_ubl_ro.py` (571 lines)
- `addons/l10n_ro_edi/views/account_move_views.xml` (118 lines)
- `addons/l10n_ro_edi/views/product_views.xml` (17 lines)
- `addons/l10n_ro_edi/views/res_config_settings_views.xml` (91 lines)
- `addons/l10n_ro_edi/wizard/__init__.py` (2 lines)
- `addons/l10n_ro_edi/wizard/account_move_fetch_invoices_wizard.py` (35 lines)
- `addons/l10n_ro_edi/wizard/account_move_fetch_invoices_wizard.xml` (28 lines)
- `addons/l10n_ro_edi/wizard/account_move_send_wizard.py` (16 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
