# Module: l10n_fr_payment

- **Module ID:** MOD-193
- **Path:** `addons/l10n_fr_payment`
- **Manifest:** `addons/l10n_fr_payment/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Applies CAWL/Worldline branding rules for French companies.

No manifest description declared.

Declared dependencies: `l10n_fr`, `payment`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 5 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_fr",
    "payment"
  ]
}
```

### Representative source files

- `addons/l10n_fr_payment/__init__.py` (21 lines)
- `addons/l10n_fr_payment/__manifest__.py` (15 lines)
- `addons/l10n_fr_payment/i18n/fr.po` (52 lines)
- `addons/l10n_fr_payment/i18n/l10n_fr_payment.pot` (48 lines)
- `addons/l10n_fr_payment/models/__init__.py` (3 lines)
- `addons/l10n_fr_payment/models/payment_provider.py` (45 lines)
- `addons/l10n_fr_payment/models/res_company.py` (25 lines)
- `addons/l10n_fr_payment/static/description/worldline_cawl.png` (323 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
