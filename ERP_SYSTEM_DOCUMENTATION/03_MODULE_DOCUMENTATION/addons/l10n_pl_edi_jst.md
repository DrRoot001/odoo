# Module: l10n_pl_edi_jst

- **Module ID:** MOD-300
- **Path:** `addons/l10n_pl_edi_jst`
- **Manifest:** `addons/l10n_pl_edi_jst/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Support for Local Government Unit (LGU) in the FA(3) format

Export FA(3) compliant XML invoices and prepare for integration with KSeF.

Declared dependencies: `l10n_pl`, `l10n_pl_edi`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
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
    "l10n_pl_edi"
  ],
  "data": [
    "views/res_partner_views.xml",
    "data/fa3_template.xml"
  ]
}
```

### Representative source files

- `addons/l10n_pl_edi_jst/__init__.py` (1 lines)
- `addons/l10n_pl_edi_jst/__manifest__.py` (17 lines)
- `addons/l10n_pl_edi_jst/data/fa3_template.xml` (42 lines)
- `addons/l10n_pl_edi_jst/i18n/l10n_pl_edi_jst.pot` (73 lines)
- `addons/l10n_pl_edi_jst/i18n/pl.po` (73 lines)
- `addons/l10n_pl_edi_jst/models/__init__.py` (2 lines)
- `addons/l10n_pl_edi_jst/models/account_move.py` (30 lines)
- `addons/l10n_pl_edi_jst/models/res_partner.py` (12 lines)
- `addons/l10n_pl_edi_jst/tests/__init__.py` (1 lines)
- `addons/l10n_pl_edi_jst/tests/export_xmls/standert_fa3_format_with_jst.xml` (86 lines)
- `addons/l10n_pl_edi_jst/tests/test_l10n_pl_edi_jst.py` (40 lines)
- `addons/l10n_pl_edi_jst/views/res_partner_views.xml` (15 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
