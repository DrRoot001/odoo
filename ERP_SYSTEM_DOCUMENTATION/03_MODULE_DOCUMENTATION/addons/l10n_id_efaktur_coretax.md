# Module: l10n_id_efaktur_coretax

- **Module ID:** MOD-222
- **Path:** `addons/l10n_id_efaktur_coretax`
- **Manifest:** `addons/l10n_id_efaktur_coretax/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


        E-invoicing feature provided by DJP (Indonesian Tax Office). As of January 1st 2025,
        Indonesia is using CoreTax system, which changes the file format and content of E-Faktur.
        We're changing from CSV files into XML.
        At the same time, due to tax regulation changes back and forth, for general E-Faktur now,
        TaxBase (DPP) has to be mulitplied by factor of 11/12 while multiplied to tax of 12% which
        is resulting to 11%.
    

Declared dependencies: `l10n_id`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 17 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 9 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 10 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_id"
  ],
  "data": [
    "data/l10n_id_efaktur_coretax.product.code.csv",
    "data/l10n_id_efaktur_coretax.uom.code.csv",
    "data/uom.uom.csv",
    "data/efaktur_templates.xml",
    "data/ir_action.xml",
    "views/product_template.xml",
    "views/product_code.xml",
    "views/uom_code.xml",
    "views/res_partner.xml",
    "views/account_move.xml",
    "views/efaktur_document.xml",
    "views/uom_uom.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/l10n_id_efaktur_coretax/__init__.py` (4 lines)
- `addons/l10n_id_efaktur_coretax/__manifest__.py` (39 lines)
- `addons/l10n_id_efaktur_coretax/controllers/__init__.py` (3 lines)
- `addons/l10n_id_efaktur_coretax/controllers/download_efaktur.py` (33 lines)
- `addons/l10n_id_efaktur_coretax/data/efaktur_templates.xml` (61 lines)
- `addons/l10n_id_efaktur_coretax/data/ir_action.xml` (10 lines)
- `addons/l10n_id_efaktur_coretax/data/l10n_id_efaktur_coretax.product.code.csv` (1,968 lines)
- `addons/l10n_id_efaktur_coretax/data/l10n_id_efaktur_coretax.uom.code.csv` (40 lines)
- `addons/l10n_id_efaktur_coretax/data/uom.uom.csv` (14 lines)
- `addons/l10n_id_efaktur_coretax/i18n/id.po` (1,464 lines)
- `addons/l10n_id_efaktur_coretax/i18n/l10n_id_efaktur_coretax.pot` (1,331 lines)
- `addons/l10n_id_efaktur_coretax/models/__init__.py` (10 lines)
- `addons/l10n_id_efaktur_coretax/models/account_move.py` (460 lines)
- `addons/l10n_id_efaktur_coretax/models/account_move_line.py` (80 lines)
- `addons/l10n_id_efaktur_coretax/models/efaktur_document.py` (95 lines)
- `addons/l10n_id_efaktur_coretax/models/product_code.py` (25 lines)
- `addons/l10n_id_efaktur_coretax/models/product_template.py` (25 lines)
- `addons/l10n_id_efaktur_coretax/models/res_partner.py` (42 lines)
- `addons/l10n_id_efaktur_coretax/models/uom_code.py` (15 lines)
- `addons/l10n_id_efaktur_coretax/models/uom_uom.py` (12 lines)
- `addons/l10n_id_efaktur_coretax/security/ir.access.csv` (5 lines)
- `addons/l10n_id_efaktur_coretax/tests/__init__.py` (3 lines)
- `addons/l10n_id_efaktur_coretax/tests/results/sample.xml` (42 lines)
- `addons/l10n_id_efaktur_coretax/tests/test_l10n_id_efaktur_coretax.py` (1,455 lines)
- `addons/l10n_id_efaktur_coretax/tests/test_l10n_id_efaktur_download.py` (94 lines)
- `addons/l10n_id_efaktur_coretax/tests/test_l10n_id_is_company.py` (109 lines)
- `addons/l10n_id_efaktur_coretax/views/account_move.xml` (42 lines)
- `addons/l10n_id_efaktur_coretax/views/efaktur_document.xml` (77 lines)
- `addons/l10n_id_efaktur_coretax/views/product_code.xml` (15 lines)
- `addons/l10n_id_efaktur_coretax/views/product_template.xml` (17 lines)
- `addons/l10n_id_efaktur_coretax/views/res_partner.xml` (24 lines)
- `addons/l10n_id_efaktur_coretax/views/uom_code.xml` (15 lines)
- `addons/l10n_id_efaktur_coretax/views/uom_uom.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
