# Module: l10n_cn

- **Module ID:** MOD-151
- **Path:** `addons/l10n_cn`
- **Manifest:** `addons/l10n_cn/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Includes the following data for the Chinese localization
========================================================

Account Type/科目类型

State Data/省份数据

    科目类型\会计科目表模板\增值税\辅助核算类别\管理会计凭证簿\财务会计凭证簿

    添加中文省份数据

    增加小企业会计科目表

    修改小企业会计科目表

    修改小企业会计税率

    增加大企业会计科目表

We added the option to print a voucher which will also
print the amount in words (special Chinese characters for numbers)
correctly when the cn2an library is installed. (e.g. with pip3 install cn2an)
    

Declared dependencies: `base`, `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 15 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 9 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 11 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base",
    "account"
  ],
  "data": [
    "data/account_tax_report_data.xml",
    "data/res_city_data.xml",
    "data/res_country_data.xml",
    "views/account_move_view.xml",
    "views/account_report.xml",
    "views/report_voucher.xml",
    "views/account_move_line_view.xml",
    "views/res_config_settings_views.xml",
    "views/balance_deduction_view.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "demo/demo_company.xml",
    "demo/demo_company_asbe.xml"
  ]
}
```

### Representative source files

- `addons/l10n_cn/__init__.py` (7 lines)
- `addons/l10n_cn/__manifest__.py` (58 lines)
- `addons/l10n_cn/data/account_tax_report_data.xml` (4,301 lines)
- `addons/l10n_cn/data/res_city_data.xml` (17,105 lines)
- `addons/l10n_cn/data/res_country_data.xml` (6 lines)
- `addons/l10n_cn/data/template/account.account-cn.csv` (68 lines)
- `addons/l10n_cn/data/template/account.account-cn_common.csv` (90 lines)
- `addons/l10n_cn/data/template/account.account-cn_large_bis.csv` (198 lines)
- `addons/l10n_cn/data/template/account.depreciation.model-cn_common.csv` (6 lines)
- `addons/l10n_cn/data/template/account.fiscal.position-cn_common.csv` (5 lines)
- `addons/l10n_cn/data/template/account.tax-cn_common.csv` (246 lines)
- `addons/l10n_cn/data/template/account.tax.group-cn_common.csv` (8 lines)
- `addons/l10n_cn/demo/demo_company.xml` (36 lines)
- `addons/l10n_cn/demo/demo_company_asbe.xml` (36 lines)
- `addons/l10n_cn/i18n/l10n_cn.pot` (14,836 lines)
- `addons/l10n_cn/i18n/zh_CN.po` (14,844 lines)
- `addons/l10n_cn/models/__init__.py` (9 lines)
- `addons/l10n_cn/models/account_move.py` (221 lines)
- `addons/l10n_cn/models/account_move_line.py` (159 lines)
- `addons/l10n_cn/models/balance_deduction.py` (93 lines)
- `addons/l10n_cn/models/res_company.py` (19 lines)
- `addons/l10n_cn/models/res_config_settings.py` (18 lines)
- `addons/l10n_cn/models/template_cn.py` (54 lines)
- `addons/l10n_cn/models/template_cn_common.py` (45 lines)
- `addons/l10n_cn/models/template_cn_large_bis.py` (53 lines)
- `addons/l10n_cn/security/ir.access.csv` (4 lines)
- `addons/l10n_cn/tests/__init__.py` (1 lines)
- `addons/l10n_cn/tests/test_balance_deduction.py` (513 lines)
- `addons/l10n_cn/views/account_move_line_view.xml` (41 lines)
- `addons/l10n_cn/views/account_move_view.xml` (46 lines)
- `addons/l10n_cn/views/account_report.xml` (15 lines)
- `addons/l10n_cn/views/balance_deduction_view.xml` (93 lines)
- `addons/l10n_cn/views/report_voucher.xml` (133 lines)
- `addons/l10n_cn/views/res_config_settings_views.xml` (24 lines)
- `addons/l10n_cn/wizard/__init__.py` (1 lines)
- `addons/l10n_cn/wizard/account_move_reversal.py` (19 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
