# Module: account_payment_custom

- **Module ID:** MOD-009
- **Path:** `addons/account_payment_custom`
- **Manifest:** `addons/account_payment_custom/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Bridge between payment_custom and account_payment.

No manifest description declared.

Declared dependencies: `account_payment`, `payment_custom`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 15 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account_payment",
    "payment_custom"
  ],
  "data": [
    "data/account_payment_method.xml",
    "data/ir_cron.xml"
  ]
}
```

### Representative source files

- `addons/account_payment_custom/__init__.py` (3 lines)
- `addons/account_payment_custom/__manifest__.py` (13 lines)
- `addons/account_payment_custom/const.py` (9 lines)
- `addons/account_payment_custom/controllers/__init__.py` (3 lines)
- `addons/account_payment_custom/controllers/portal.py` (10 lines)
- `addons/account_payment_custom/data/account_payment_method.xml` (10 lines)
- `addons/account_payment_custom/data/ir_cron.xml` (15 lines)
- `addons/account_payment_custom/i18n/account_payment_custom.pot` (78 lines)
- `addons/account_payment_custom/i18n/ar.po` (83 lines)
- `addons/account_payment_custom/i18n/az.po` (81 lines)
- `addons/account_payment_custom/i18n/bg.po` (81 lines)
- `addons/account_payment_custom/i18n/bs.po` (82 lines)
- `addons/account_payment_custom/i18n/ca.po` (81 lines)
- `addons/account_payment_custom/i18n/cs.po` (81 lines)
- `addons/account_payment_custom/i18n/da.po` (85 lines)
- `addons/account_payment_custom/i18n/de.po` (86 lines)
- `addons/account_payment_custom/i18n/el.po` (81 lines)
- `addons/account_payment_custom/i18n/es.po` (82 lines)
- `addons/account_payment_custom/i18n/es_419.po` (85 lines)
- `addons/account_payment_custom/i18n/et.po` (81 lines)
- `addons/account_payment_custom/i18n/fa.po` (81 lines)
- `addons/account_payment_custom/i18n/fi.po` (85 lines)
- `addons/account_payment_custom/i18n/fr.po` (85 lines)
- `addons/account_payment_custom/i18n/he.po` (82 lines)
- `addons/account_payment_custom/i18n/hi.po` (81 lines)
- `addons/account_payment_custom/i18n/hr.po` (82 lines)
- `addons/account_payment_custom/i18n/hu.po` (81 lines)
- `addons/account_payment_custom/i18n/id.po` (86 lines)
- `addons/account_payment_custom/i18n/it.po` (85 lines)
- `addons/account_payment_custom/i18n/ja.po` (86 lines)
- `addons/account_payment_custom/i18n/kab.po` (81 lines)
- `addons/account_payment_custom/i18n/ko.po` (81 lines)
- `addons/account_payment_custom/i18n/ku.po` (81 lines)
- `addons/account_payment_custom/i18n/lo.po` (81 lines)
- `addons/account_payment_custom/i18n/lt.po` (83 lines)
- `addons/account_payment_custom/i18n/lv.po` (82 lines)
- `addons/account_payment_custom/i18n/mn.po` (85 lines)
- `addons/account_payment_custom/i18n/my.po` (81 lines)
- `addons/account_payment_custom/i18n/nb.po` (81 lines)
- `addons/account_payment_custom/i18n/nl.po` (86 lines)
- `addons/account_payment_custom/i18n/pl.po` (83 lines)
- `addons/account_payment_custom/i18n/pt.po` (81 lines)
- `addons/account_payment_custom/i18n/pt_BR.po` (85 lines)
- `addons/account_payment_custom/i18n/ro.po` (82 lines)
- `addons/account_payment_custom/i18n/ru.po` (82 lines)
- `addons/account_payment_custom/i18n/sk.po` (81 lines)
- `addons/account_payment_custom/i18n/sl.po` (82 lines)
- `addons/account_payment_custom/i18n/sr@latin.po` (82 lines)
- `addons/account_payment_custom/i18n/sv.po` (85 lines)
- `addons/account_payment_custom/i18n/th.po` (81 lines)
- `addons/account_payment_custom/i18n/tr.po` (82 lines)
- `addons/account_payment_custom/i18n/uk.po` (86 lines)
- `addons/account_payment_custom/i18n/uz.po` (81 lines)
- `addons/account_payment_custom/i18n/vi.po` (81 lines)
- `addons/account_payment_custom/i18n/zh_CN.po` (85 lines)
- `addons/account_payment_custom/i18n/zh_TW.po` (82 lines)
- `addons/account_payment_custom/models/__init__.py` (8 lines)
- `addons/account_payment_custom/models/account_bank_statement_line.py` (61 lines)
- `addons/account_payment_custom/models/account_payment_method.py` (13 lines)
- `addons/account_payment_custom/models/payment_provider.py` (76 lines)
- `addons/account_payment_custom/models/payment_transaction.py` (13 lines)
- `addons/account_payment_custom/tests/__init__.py` (3 lines)
- `addons/account_payment_custom/tests/common.py` (23 lines)
- `addons/account_payment_custom/tests/test_account_bank_statement_line.py` (37 lines)
- `addons/account_payment_custom/tests/test_payment_provider.py` (51 lines)
- `addons/account_payment_custom/tests/test_portal.py` (39 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
