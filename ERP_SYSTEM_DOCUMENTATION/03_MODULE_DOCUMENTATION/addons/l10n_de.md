# Module: l10n_de

- **Module ID:** MOD-157
- **Path:** `addons/l10n_de`
- **Manifest:** `addons/l10n_de/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Dieses  Modul beinhaltet einen deutschen Kontenrahmen basierend auf dem SKR03 oder SKR04.
=========================================================================================

German accounting chart and localization.
By default, the audit trail is enabled for GoBD compliance.
    

Declared dependencies: `l10n_din5008`, `account`, `account_edi_ubl_cii`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 18 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 10 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_din5008",
    "account",
    "account_edi_ubl_cii"
  ],
  "data": [
    "data/account_account_tags_data.xml",
    "views/account_view.xml",
    "views/res_company_views.xml",
    "wizard/account_secure_entries_wizard.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_de/__init__.py` (8 lines)
- `addons/l10n_de/__manifest__.py` (35 lines)
- `addons/l10n_de/data/account_account_tags_data.xml` (1,176 lines)
- `addons/l10n_de/data/template/account.account-de_skr03.csv` (1,305 lines)
- `addons/l10n_de/data/template/account.account-de_skr04.csv` (1,223 lines)
- `addons/l10n_de/data/template/account.depreciation.model-de_skr03.csv` (17 lines)
- `addons/l10n_de/data/template/account.depreciation.model-de_skr04.csv` (17 lines)
- `addons/l10n_de/data/template/account.fiscal.position-de_skr03.csv` (31 lines)
- `addons/l10n_de/data/template/account.fiscal.position-de_skr04.csv` (31 lines)
- `addons/l10n_de/data/template/account.tax-de_skr03.csv` (243 lines)
- `addons/l10n_de/data/template/account.tax-de_skr04.csv` (243 lines)
- `addons/l10n_de/data/template/account.tax.group-de_skr03.csv` (7 lines)
- `addons/l10n_de/data/template/account.tax.group-de_skr04.csv` (7 lines)
- `addons/l10n_de/demo/demo_company.xml` (43 lines)
- `addons/l10n_de/i18n/de.po` (178 lines)
- `addons/l10n_de/i18n/l10n_de.pot` (153 lines)
- `addons/l10n_de/migrations/1.1/post-migrate_update_amls.py` (39 lines)
- `addons/l10n_de/migrations/2.0/pre-migrate.py` (57 lines)
- `addons/l10n_de/migrations/3.0/pre-migrate.py` (22 lines)
- `addons/l10n_de/models/__init__.py` (12 lines)
- `addons/l10n_de/models/account_account.py` (19 lines)
- `addons/l10n_de/models/account_journal.py` (18 lines)
- `addons/l10n_de/models/account_move.py` (34 lines)
- `addons/l10n_de/models/chart_template.py` (24 lines)
- `addons/l10n_de/models/datev.py` (37 lines)
- `addons/l10n_de/models/ir_actions_report.py` (10 lines)
- `addons/l10n_de/models/res_company.py` (60 lines)
- `addons/l10n_de/models/template_de_skr03.py` (387 lines)
- `addons/l10n_de/models/template_de_skr04.py` (369 lines)
- `addons/l10n_de/tests/__init__.py` (2 lines)
- `addons/l10n_de/tests/test_account_move.py` (57 lines)
- `addons/l10n_de/tests/test_audit_trail.py` (20 lines)
- `addons/l10n_de/views/account_view.xml` (13 lines)
- `addons/l10n_de/views/res_company_views.xml` (14 lines)
- `addons/l10n_de/wizard/account_secure_entries_wizard.xml` (19 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
