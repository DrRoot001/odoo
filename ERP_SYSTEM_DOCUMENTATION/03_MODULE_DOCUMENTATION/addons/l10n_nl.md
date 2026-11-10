# Module: l10n_nl

- **Module ID:** MOD-285
- **Path:** `addons/l10n_nl`
- **Manifest:** `addons/l10n_nl/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

No manifest description declared.

Declared dependencies: `account`, `account_edi_ubl_cii`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
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
    "data/account_account_tag.xml",
    "data/account_tax_report_data.xml",
    "data/res_country_group.xml",
    "views/res_config_settings_view.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_nl/README.md` (20 lines)
- `addons/l10n_nl/__init__.py` (6 lines)
- `addons/l10n_nl/__manifest__.py` (25 lines)
- `addons/l10n_nl/data/account_account_tag.xml` (358 lines)
- `addons/l10n_nl/data/account_tax_report_data.xml` (441 lines)
- `addons/l10n_nl/data/res_country_group.xml` (14 lines)
- `addons/l10n_nl/data/template/account.account-nl.csv` (351 lines)
- `addons/l10n_nl/data/template/account.fiscal.position-nl.csv` (22 lines)
- `addons/l10n_nl/data/template/account.tax-nl.csv` (145 lines)
- `addons/l10n_nl/data/template/account.tax.group-nl.csv` (4 lines)
- `addons/l10n_nl/demo/demo_company.xml` (43 lines)
- `addons/l10n_nl/i18n/l10n_nl.pot` (114 lines)
- `addons/l10n_nl/i18n/nl.po` (142 lines)
- `addons/l10n_nl/migrations/3.1/end-migrate_update_taxes.py` (8 lines)
- `addons/l10n_nl/migrations/3.3/post-migrate_update_taxes.py` (109 lines)
- `addons/l10n_nl/migrations/3.4/end-migrate.py` (7 lines)
- `addons/l10n_nl/migrations/9.0.2.0/pre-set_tags_and_taxes_updatable.py` (8 lines)
- `addons/l10n_nl/models/__init__.py` (6 lines)
- `addons/l10n_nl/models/account_chart_template.py` (14 lines)
- `addons/l10n_nl/models/account_journal.py` (20 lines)
- `addons/l10n_nl/models/res_company.py` (11 lines)
- `addons/l10n_nl/models/res_partner.py` (31 lines)
- `addons/l10n_nl/models/template_nl.py` (50 lines)
- `addons/l10n_nl/views/res_config_settings_view.xml` (18 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
