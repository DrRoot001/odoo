# Module: l10n_it_edi_doi

- **Module ID:** MOD-242
- **Path:** `addons/l10n_it_edi_doi`
- **Manifest:** `addons/l10n_it_edi_doi/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


    Add support for the Declaration of Intent (Dichiarazione di Intento) to the Italian localization.
    

Declared dependencies: `l10n_it_edi`, `sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 14 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 9 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 7 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_it_edi",
    "sale"
  ],
  "data": [
    "data/invoice_it_template.xml",
    "views/l10n_it_edi_doi_declaration_of_intent_views.xml",
    "views/account_move_views.xml",
    "views/report_invoice.xml",
    "views/res_partner_views.xml",
    "views/sale_ir_actions_report_templates.xml",
    "views/sale_order_views.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/l10n_it_edi_doi/__init__.py` (3 lines)
- `addons/l10n_it_edi_doi/__manifest__.py` (27 lines)
- `addons/l10n_it_edi_doi/data/invoice_it_template.xml` (16 lines)
- `addons/l10n_it_edi_doi/data/template/account.fiscal.position-it.csv` (2 lines)
- `addons/l10n_it_edi_doi/data/template/account.tax-it.csv` (5 lines)
- `addons/l10n_it_edi_doi/i18n/it.po` (846 lines)
- `addons/l10n_it_edi_doi/i18n/l10n_it_edi_doi.pot` (782 lines)
- `addons/l10n_it_edi_doi/models/__init__.py` (9 lines)
- `addons/l10n_it_edi_doi/models/account_chart_template.py` (26 lines)
- `addons/l10n_it_edi_doi/models/account_fiscal_position.py` (14 lines)
- `addons/l10n_it_edi_doi/models/account_move.py` (210 lines)
- `addons/l10n_it_edi_doi/models/account_tax.py` (12 lines)
- `addons/l10n_it_edi_doi/models/declaration_of_intent.py` (313 lines)
- `addons/l10n_it_edi_doi/models/res_company.py` (17 lines)
- `addons/l10n_it_edi_doi/models/res_partner.py` (28 lines)
- `addons/l10n_it_edi_doi/models/sale_order.py` (256 lines)
- `addons/l10n_it_edi_doi/security/ir.access.csv` (3 lines)
- `addons/l10n_it_edi_doi/tests/__init__.py` (3 lines)
- `addons/l10n_it_edi_doi/tests/common.py` (35 lines)
- `addons/l10n_it_edi_doi/tests/test_amounts_and_warnings.py` (528 lines)
- `addons/l10n_it_edi_doi/views/account_move_views.xml` (80 lines)
- `addons/l10n_it_edi_doi/views/l10n_it_edi_doi_declaration_of_intent_views.xml` (131 lines)
- `addons/l10n_it_edi_doi/views/report_invoice.xml` (10 lines)
- `addons/l10n_it_edi_doi/views/res_partner_views.xml` (38 lines)
- `addons/l10n_it_edi_doi/views/sale_ir_actions_report_templates.xml` (10 lines)
- `addons/l10n_it_edi_doi/views/sale_order_views.xml` (81 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
