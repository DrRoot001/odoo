# Module: l10n_jp

- **Module ID:** MOD-248
- **Path:** `addons/l10n_jp`
- **Manifest:** `addons/l10n_jp/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.



Overview:
---------

* Chart of Accounts and Taxes template for companies in Japan.
* This probably does not cover all the necessary accounts for a company. You are expected to add/delete/modify accounts based on this template.

Note:
-----

* Fiscal positions '内税' and '外税' have been added to handle special requirements which might arise from POS implementation. [1]  Under normal circumstances, you might not need to use those at all.

[1] See https://github.com/odoo/odoo/pull/6470 for detail.

    

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 5 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 12 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account"
  ],
  "data": [
    "data/account.account.tag.csv",
    "data/account_report_jct_accumulation_form.xml",
    "data/account_report_jct_accumulation_schedule_1_3.xml",
    "data/account_report_jct_accumulation_schedule_2_3.xml",
    "data/account_report_jct_accumulation_schedule_4_3.xml",
    "data/account_report_jct_accumulation_schedule_5_3.xml",
    "data/account_report_jct_deduction_form.xml",
    "data/account_report_jct_deduction_schedule_1_3.xml",
    "data/account_report_jct_deduction_schedule_2_3.xml",
    "data/account_report_jct_deduction_schedule_4_3.xml",
    "data/account_report_jct_deduction_schedule_5_3.xml",
    "data/account_report_jct_return.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_jp/__init__.py` (2 lines)
- `addons/l10n_jp/__manifest__.py` (48 lines)
- `addons/l10n_jp/data/account.account.tag.csv` (5 lines)
- `addons/l10n_jp/data/account_report_jct_accumulation_form.xml` (1,049 lines)
- `addons/l10n_jp/data/account_report_jct_accumulation_schedule_1_3.xml` (437 lines)
- `addons/l10n_jp/data/account_report_jct_accumulation_schedule_2_3.xml` (886 lines)
- `addons/l10n_jp/data/account_report_jct_accumulation_schedule_4_3.xml` (370 lines)
- `addons/l10n_jp/data/account_report_jct_accumulation_schedule_5_3.xml` (1,904 lines)
- `addons/l10n_jp/data/account_report_jct_deduction_form.xml` (1,049 lines)
- `addons/l10n_jp/data/account_report_jct_deduction_schedule_1_3.xml` (421 lines)
- `addons/l10n_jp/data/account_report_jct_deduction_schedule_2_3.xml` (1,030 lines)
- `addons/l10n_jp/data/account_report_jct_deduction_schedule_4_3.xml` (370 lines)
- `addons/l10n_jp/data/account_report_jct_deduction_schedule_5_3.xml` (2,149 lines)
- `addons/l10n_jp/data/account_report_jct_return.xml` (36 lines)
- `addons/l10n_jp/data/template/account.account-jp.csv` (209 lines)
- `addons/l10n_jp/data/template/account.depreciation.model-jp.csv` (39 lines)
- `addons/l10n_jp/data/template/account.fiscal.position-jp.csv` (4 lines)
- `addons/l10n_jp/data/template/account.tax-jp.csv` (271 lines)
- `addons/l10n_jp/data/template/account.tax.group-jp.csv` (6 lines)
- `addons/l10n_jp/demo/demo_company.xml` (36 lines)
- `addons/l10n_jp/i18n/ja.po` (69 lines)
- `addons/l10n_jp/i18n/l10n_jp.pot` (62 lines)
- `addons/l10n_jp/migrations/2.3/pre-migrate.py` (27 lines)
- `addons/l10n_jp/models/__init__.py` (2 lines)
- `addons/l10n_jp/models/template_jp.py` (82 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
