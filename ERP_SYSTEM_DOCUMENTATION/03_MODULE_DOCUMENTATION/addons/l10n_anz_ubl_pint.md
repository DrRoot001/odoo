# Module: l10n_anz_ubl_pint

- **Module ID:** MOD-119
- **Path:** `addons/l10n_anz_ubl_pint`
- **Manifest:** `addons/l10n_anz_ubl_pint/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


    The UBL PINT e-invoicing format for Australia & New Zealand is based on the Peppol International (PINT) model for Billing.
    

Declared dependencies: `account_edi_ubl_cii`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account_edi_ubl_cii"
  ]
}
```

### Representative source files

- `addons/l10n_anz_ubl_pint/__init__.py` (6 lines)
- `addons/l10n_anz_ubl_pint/__manifest__.py` (13 lines)
- `addons/l10n_anz_ubl_pint/models/__init__.py` (4 lines)
- `addons/l10n_anz_ubl_pint/models/account_edi_xml_pint_anz.py` (153 lines)
- `addons/l10n_anz_ubl_pint/models/account_move.py` (14 lines)
- `addons/l10n_anz_ubl_pint/models/res_partner.py` (20 lines)
- `addons/l10n_anz_ubl_pint/tests/__init__.py` (1 lines)
- `addons/l10n_anz_ubl_pint/tests/expected_xmls/invoice.xml` (143 lines)
- `addons/l10n_anz_ubl_pint/tests/test_anz_ubl_pint.py` (87 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
