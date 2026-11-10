# Module: account_payment_interco

- **Module ID:** MOD-010
- **Path:** `addons/account_payment_interco`
- **Manifest:** `addons/account_payment_interco/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Enable Intercompany payments to reconcile with their invoices on post.

No manifest description declared.

Declared dependencies: `account_payment`.

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
    "account_payment"
  ],
  "data": [
    "views/res_config_settings_views.xml"
  ]
}
```

### Representative source files

- `addons/account_payment_interco/__init__.py` (1 lines)
- `addons/account_payment_interco/__manifest__.py` (11 lines)
- `addons/account_payment_interco/i18n/account_payment_interco.pot` (117 lines)
- `addons/account_payment_interco/i18n/ar.po` (125 lines)
- `addons/account_payment_interco/i18n/az.po` (117 lines)
- `addons/account_payment_interco/i18n/bg.po` (117 lines)
- `addons/account_payment_interco/i18n/bs.po` (117 lines)
- `addons/account_payment_interco/i18n/ca.po` (121 lines)
- `addons/account_payment_interco/i18n/cs.po` (117 lines)
- `addons/account_payment_interco/i18n/da.po` (117 lines)
- `addons/account_payment_interco/i18n/de.po` (128 lines)
- `addons/account_payment_interco/i18n/el.po` (117 lines)
- `addons/account_payment_interco/i18n/es.po` (125 lines)
- `addons/account_payment_interco/i18n/es_419.po` (125 lines)
- `addons/account_payment_interco/i18n/et.po` (117 lines)
- `addons/account_payment_interco/i18n/fa.po` (117 lines)
- `addons/account_payment_interco/i18n/fi.po` (123 lines)
- `addons/account_payment_interco/i18n/fr.po` (128 lines)
- `addons/account_payment_interco/i18n/he.po` (117 lines)
- `addons/account_payment_interco/i18n/hi.po` (117 lines)
- `addons/account_payment_interco/i18n/hr.po` (117 lines)
- `addons/account_payment_interco/i18n/hu.po` (117 lines)
- `addons/account_payment_interco/i18n/id.po` (117 lines)
- `addons/account_payment_interco/i18n/it.po` (129 lines)
- `addons/account_payment_interco/i18n/ja.po` (121 lines)
- `addons/account_payment_interco/i18n/kab.po` (117 lines)
- `addons/account_payment_interco/i18n/ko.po` (117 lines)
- `addons/account_payment_interco/i18n/ku.po` (117 lines)
- `addons/account_payment_interco/i18n/lo.po` (117 lines)
- `addons/account_payment_interco/i18n/lt.po` (117 lines)
- `addons/account_payment_interco/i18n/lv.po` (117 lines)
- `addons/account_payment_interco/i18n/mn.po` (117 lines)
- `addons/account_payment_interco/i18n/my.po` (121 lines)
- `addons/account_payment_interco/i18n/nb.po` (117 lines)
- `addons/account_payment_interco/i18n/nl.po` (128 lines)
- `addons/account_payment_interco/i18n/pl.po` (124 lines)
- `addons/account_payment_interco/i18n/pt.po` (117 lines)
- `addons/account_payment_interco/i18n/pt_BR.po` (126 lines)
- `addons/account_payment_interco/i18n/ro.po` (117 lines)
- `addons/account_payment_interco/i18n/ru.po` (117 lines)
- `addons/account_payment_interco/i18n/sk.po` (117 lines)
- `addons/account_payment_interco/i18n/sl.po` (117 lines)
- `addons/account_payment_interco/i18n/sr@latin.po` (117 lines)
- `addons/account_payment_interco/i18n/sv.po` (124 lines)
- `addons/account_payment_interco/i18n/th.po` (117 lines)
- `addons/account_payment_interco/i18n/tr.po` (123 lines)
- `addons/account_payment_interco/i18n/uk.po` (129 lines)
- `addons/account_payment_interco/i18n/uz.po` (117 lines)
- `addons/account_payment_interco/i18n/vi.po` (117 lines)
- `addons/account_payment_interco/i18n/zh_CN.po` (122 lines)
- `addons/account_payment_interco/i18n/zh_TW.po` (117 lines)
- `addons/account_payment_interco/models/__init__.py` (4 lines)
- `addons/account_payment_interco/models/account_move.py` (138 lines)
- `addons/account_payment_interco/models/res_company.py` (26 lines)
- `addons/account_payment_interco/models/res_config_settings.py` (24 lines)
- `addons/account_payment_interco/tests/__init__.py` (1 lines)
- `addons/account_payment_interco/tests/test_interco_clearing.py` (325 lines)
- `addons/account_payment_interco/views/res_config_settings_views.xml` (54 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
