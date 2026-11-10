# Module: l10n_my_edi_pos

- **Module ID:** MOD-280
- **Path:** `addons/l10n_my_edi_pos`
- **Manifest:** `addons/l10n_my_edi_pos/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Consolidated E-invoicing using MyInvois


    This modules allows the user to send consolidated invoices to the MyInvois system when using the POS app.
    

Declared dependencies: `l10n_my_edi`, `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 13 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 10 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_my_edi",
    "point_of_sale"
  ],
  "data": [
    "views/myinvois_document_pos_views.xml",
    "views/pos_order_views.xml",
    "views/product_view.xml",
    "views/res_partner_view.xml",
    "views/portal_address_templates.xml",
    "views/ticket_validation_screen.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "l10n_my_edi_pos/static/src/interactions/address.js"
    ]
  }
}
```

### Representative source files

- `addons/l10n_my_edi_pos/__init__.py` (4 lines)
- `addons/l10n_my_edi_pos/__manifest__.py` (29 lines)
- `addons/l10n_my_edi_pos/controllers/__init__.py` (1 lines)
- `addons/l10n_my_edi_pos/controllers/portal.py` (112 lines)
- `addons/l10n_my_edi_pos/i18n/l10n_my_edi_pos.pot` (317 lines)
- `addons/l10n_my_edi_pos/i18n/ms.po` (325 lines)
- `addons/l10n_my_edi_pos/models/__init__.py` (5 lines)
- `addons/l10n_my_edi_pos/models/account_edi_xml_ubl_my.py` (433 lines)
- `addons/l10n_my_edi_pos/models/myinvois_document_pos.py` (256 lines)
- `addons/l10n_my_edi_pos/models/pos_order.py` (141 lines)
- `addons/l10n_my_edi_pos/models/res_partner.py` (11 lines)
- `addons/l10n_my_edi_pos/static/src/interactions/address.js` (100 lines)
- `addons/l10n_my_edi_pos/tests/__init__.py` (2 lines)
- `addons/l10n_my_edi_pos/tests/expected_xmls/consolidated_invoice.xml` (246 lines)
- `addons/l10n_my_edi_pos/tests/expected_xmls/consolidated_invoice_refund.xml` (177 lines)
- `addons/l10n_my_edi_pos/tests/expected_xmls/consolidated_invoice_tax_included.xml` (142 lines)
- `addons/l10n_my_edi_pos/tests/expected_xmls/consolidated_invoice_tax_included_with_discount.xml` (147 lines)
- `addons/l10n_my_edi_pos/tests/test_myinvois_pos.py` (1,319 lines)
- `addons/l10n_my_edi_pos/views/myinvois_document_pos_views.xml` (86 lines)
- `addons/l10n_my_edi_pos/views/portal_address_templates.xml` (22 lines)
- `addons/l10n_my_edi_pos/views/pos_order_views.xml` (76 lines)
- `addons/l10n_my_edi_pos/views/product_view.xml` (13 lines)
- `addons/l10n_my_edi_pos/views/res_partner_view.xml` (26 lines)
- `addons/l10n_my_edi_pos/views/ticket_validation_screen.xml` (71 lines)
- `addons/l10n_my_edi_pos/wizard/__init__.py` (3 lines)
- `addons/l10n_my_edi_pos/wizard/myinvois_consolidate_invoice_wizard.py` (66 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
