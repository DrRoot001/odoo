# Module: account_payment

- **Module ID:** MOD-008
- **Path:** `addons/account_payment`
- **Manifest:** `addons/account_payment/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

Enable customers to pay invoices on the portal and post payments when transactions are processed.

No manifest description declared.

Declared dependencies: `account`, `payment`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 23 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 8 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 14 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 4 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 5 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account",
    "payment"
  ],
  "data": [
    "data/ir_config_parameter.xml",
    "data/portal_entry_data.xml",
    "views/account_payment_menus.xml",
    "views/account_portal_templates.xml",
    "views/account_move_views.xml",
    "views/account_journal_views.xml",
    "views/account_payment_views.xml",
    "views/payment_form_templates.xml",
    "views/payment_provider_views.xml",
    "views/payment_transaction_views.xml",
    "wizards/account_payment_register_views.xml",
    "wizards/payment_link_wizard_views.xml",
    "wizards/payment_refund_wizard_views.xml",
    "wizards/res_config_settings_views.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_unit_tests": [
      "account_payment/static/src/interactions/**/*",
      "account_payment/static/tests/interactions/**/*"
    ],
    "web.assets_frontend": [
      "account_payment/static/src/interactions/**/*"
    ]
  }
}
```

### Representative source files

- `addons/account_payment/__init__.py` (22 lines)
- `addons/account_payment/__manifest__.py` (42 lines)
- `addons/account_payment/controllers/__init__.py` (5 lines)
- `addons/account_payment/controllers/payment.py` (152 lines)
- `addons/account_payment/controllers/portal.py` (162 lines)
- `addons/account_payment/data/ir_config_parameter.xml` (9 lines)
- `addons/account_payment/data/portal_entry_data.xml` (9 lines)
- `addons/account_payment/i18n/account_payment.pot` (766 lines)
- `addons/account_payment/i18n/af.po` (775 lines)
- `addons/account_payment/i18n/ar.po` (820 lines)
- `addons/account_payment/i18n/az.po` (781 lines)
- `addons/account_payment/i18n/bg.po` (817 lines)
- `addons/account_payment/i18n/bs.po` (779 lines)
- `addons/account_payment/i18n/ca.po` (824 lines)
- `addons/account_payment/i18n/cs.po` (804 lines)
- `addons/account_payment/i18n/da.po` (825 lines)
- `addons/account_payment/i18n/de.po` (837 lines)
- `addons/account_payment/i18n/el.po` (814 lines)
- `addons/account_payment/i18n/es.po` (831 lines)
- `addons/account_payment/i18n/es_419.po` (822 lines)
- `addons/account_payment/i18n/et.po` (813 lines)
- `addons/account_payment/i18n/fa.po` (803 lines)
- `addons/account_payment/i18n/fi.po` (837 lines)
- `addons/account_payment/i18n/fr.po` (843 lines)
- `addons/account_payment/i18n/gu.po` (775 lines)
- `addons/account_payment/i18n/he.po` (803 lines)
- `addons/account_payment/i18n/hi.po` (799 lines)
- `addons/account_payment/i18n/hr.po` (791 lines)
- `addons/account_payment/i18n/hu.po` (803 lines)
- `addons/account_payment/i18n/id.po` (830 lines)
- `addons/account_payment/i18n/is.po` (776 lines)
- `addons/account_payment/i18n/it.po` (834 lines)
- `addons/account_payment/i18n/ja.po` (824 lines)
- `addons/account_payment/i18n/kab.po` (778 lines)
- `addons/account_payment/i18n/ko.po` (801 lines)
- `addons/account_payment/i18n/ku.po` (789 lines)
- `addons/account_payment/i18n/lo.po` (801 lines)
- `addons/account_payment/i18n/lt.po` (800 lines)
- `addons/account_payment/i18n/lv.po` (793 lines)
- `addons/account_payment/i18n/mn.po` (826 lines)
- `addons/account_payment/i18n/my.po` (777 lines)
- `addons/account_payment/i18n/nb.po` (782 lines)
- `addons/account_payment/i18n/nl.po` (829 lines)
- `addons/account_payment/i18n/pl.po` (838 lines)
- `addons/account_payment/i18n/pt.po` (822 lines)
- `addons/account_payment/i18n/pt_BR.po` (831 lines)
- `addons/account_payment/i18n/ro.po` (814 lines)
- `addons/account_payment/i18n/ru.po` (812 lines)
- `addons/account_payment/i18n/sk.po` (791 lines)
- `addons/account_payment/i18n/sl.po` (817 lines)
- `addons/account_payment/i18n/sq.po` (775 lines)
- `addons/account_payment/i18n/sr@latin.po` (805 lines)
- `addons/account_payment/i18n/sv.po` (845 lines)
- `addons/account_payment/i18n/th.po` (799 lines)
- `addons/account_payment/i18n/tr.po` (832 lines)
- `addons/account_payment/i18n/uk.po` (830 lines)
- `addons/account_payment/i18n/uz.po` (946 lines)
- `addons/account_payment/i18n/vi.po` (812 lines)
- `addons/account_payment/i18n/zh_CN.po` (805 lines)
- `addons/account_payment/i18n/zh_TW.po` (792 lines)
- `addons/account_payment/models/__init__.py` (9 lines)
- `addons/account_payment/models/account_journal.py` (21 lines)
- `addons/account_payment/models/account_move.py` (176 lines)
- `addons/account_payment/models/account_payment.py` (222 lines)
- `addons/account_payment/models/account_payment_method.py` (20 lines)
- `addons/account_payment/models/account_payment_method_line.py` (84 lines)
- `addons/account_payment/models/payment_provider.py` (187 lines)
- `addons/account_payment/models/payment_transaction.py` (262 lines)
- `addons/account_payment/security/ir.access.csv` (5 lines)
- `addons/account_payment/static/src/interactions/payment_form.js` (43 lines)
- `addons/account_payment/static/src/interactions/portal_invoice_page_payment.js` (19 lines)
- `addons/account_payment/static/src/interactions/portal_my_invoices_payment_list.js` (33 lines)
- `addons/account_payment/static/tests/interactions/portal_invoice_page_payment.test.js` (181 lines)
- `addons/account_payment/tests/__init__.py` (5 lines)
- `addons/account_payment/tests/common.py` (48 lines)
- `addons/account_payment/tests/test_account_payment.py` (570 lines)
- `addons/account_payment/tests/test_payment_flows.py` (256 lines)
- `addons/account_payment/tests/test_payment_provider.py` (54 lines)
- `addons/account_payment/views/account_journal_views.xml` (25 lines)
- `addons/account_payment/views/account_move_views.xml` (41 lines)
- `addons/account_payment/views/account_payment_menus.xml` (13 lines)
- `addons/account_payment/views/account_payment_views.xml` (42 lines)
- `addons/account_payment/views/account_portal_templates.xml` (337 lines)
- `addons/account_payment/views/payment_form_templates.xml` (12 lines)
- `addons/account_payment/views/payment_provider_views.xml` (33 lines)
- `addons/account_payment/views/payment_transaction_views.xml` (26 lines)
- `addons/account_payment/wizards/__init__.py` (6 lines)
- `addons/account_payment/wizards/account_payment_register.py` (86 lines)
- `addons/account_payment/wizards/account_payment_register_views.xml` (20 lines)
- `addons/account_payment/wizards/payment_link_wizard.py` (105 lines)
- `addons/account_payment/wizards/payment_link_wizard_views.xml` (47 lines)
- `addons/account_payment/wizards/payment_refund_wizard.py` (84 lines)
- `addons/account_payment/wizards/payment_refund_wizard_views.xml` (42 lines)
- `addons/account_payment/wizards/res_config_settings.py` (9 lines)
- `addons/account_payment/wizards/res_config_settings_views.xml` (15 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
