# Module: payment_toss_payments

- **Module ID:** MOD-413
- **Path:** `addons/payment_toss_payments`
- **Manifest:** `addons/payment_toss_payments/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

A payment provider covering the South Korea market

 

Declared dependencies: `payment`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 3 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "payment"
  ],
  "data": [
    "data/payment_method_data.xml",
    "data/payment_provider_data.xml",
    "views/payment_provider_views.xml",
    "views/payment_toss_payments_templates.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "payment_toss_payments/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/payment_toss_payments/README.md` (67 lines)
- `addons/payment_toss_payments/__init__.py` (12 lines)
- `addons/payment_toss_payments/__manifest__.py` (21 lines)
- `addons/payment_toss_payments/const.py` (28 lines)
- `addons/payment_toss_payments/controllers/__init__.py` (1 lines)
- `addons/payment_toss_payments/controllers/main.py` (103 lines)
- `addons/payment_toss_payments/data/neutralize.sql` (3 lines)
- `addons/payment_toss_payments/data/payment_method_data.xml` (64 lines)
- `addons/payment_toss_payments/data/payment_provider_data.xml` (9 lines)
- `addons/payment_toss_payments/i18n/ar.po` (162 lines)
- `addons/payment_toss_payments/i18n/az.po` (160 lines)
- `addons/payment_toss_payments/i18n/bg.po` (160 lines)
- `addons/payment_toss_payments/i18n/bs.po` (161 lines)
- `addons/payment_toss_payments/i18n/ca.po` (160 lines)
- `addons/payment_toss_payments/i18n/cs.po` (160 lines)
- `addons/payment_toss_payments/i18n/da.po` (160 lines)
- `addons/payment_toss_payments/i18n/de.po` (161 lines)
- `addons/payment_toss_payments/i18n/el.po` (160 lines)
- `addons/payment_toss_payments/i18n/es.po` (161 lines)
- `addons/payment_toss_payments/i18n/es_419.po` (162 lines)
- `addons/payment_toss_payments/i18n/et.po` (160 lines)
- `addons/payment_toss_payments/i18n/fa.po` (160 lines)
- `addons/payment_toss_payments/i18n/fi.po` (161 lines)
- `addons/payment_toss_payments/i18n/fr.po` (161 lines)
- `addons/payment_toss_payments/i18n/he.po` (161 lines)
- `addons/payment_toss_payments/i18n/hi.po` (160 lines)
- `addons/payment_toss_payments/i18n/hr.po` (161 lines)
- `addons/payment_toss_payments/i18n/hu.po` (160 lines)
- `addons/payment_toss_payments/i18n/id.po` (161 lines)
- `addons/payment_toss_payments/i18n/it.po` (161 lines)
- `addons/payment_toss_payments/i18n/ja.po` (161 lines)
- `addons/payment_toss_payments/i18n/kab.po` (160 lines)
- `addons/payment_toss_payments/i18n/ko.po` (161 lines)
- `addons/payment_toss_payments/i18n/ku.po` (160 lines)
- `addons/payment_toss_payments/i18n/lo.po` (161 lines)
- `addons/payment_toss_payments/i18n/lt.po` (162 lines)
- `addons/payment_toss_payments/i18n/lv.po` (161 lines)
- `addons/payment_toss_payments/i18n/mn.po` (160 lines)
- `addons/payment_toss_payments/i18n/my.po` (160 lines)
- `addons/payment_toss_payments/i18n/nb.po` (160 lines)
- `addons/payment_toss_payments/i18n/nl.po` (161 lines)
- `addons/payment_toss_payments/i18n/payment_toss_payments.pot` (157 lines)
- `addons/payment_toss_payments/i18n/pl.po` (162 lines)
- `addons/payment_toss_payments/i18n/pt.po` (160 lines)
- `addons/payment_toss_payments/i18n/pt_BR.po` (162 lines)
- `addons/payment_toss_payments/i18n/ro.po` (161 lines)
- `addons/payment_toss_payments/i18n/ru.po` (162 lines)
- `addons/payment_toss_payments/i18n/sk.po` (160 lines)
- `addons/payment_toss_payments/i18n/sl.po` (161 lines)
- `addons/payment_toss_payments/i18n/sr@latin.po` (161 lines)
- `addons/payment_toss_payments/i18n/sv.po` (161 lines)
- `addons/payment_toss_payments/i18n/th.po` (161 lines)
- `addons/payment_toss_payments/i18n/tr.po` (160 lines)
- `addons/payment_toss_payments/i18n/uk.po` (161 lines)
- `addons/payment_toss_payments/i18n/uz.po` (160 lines)
- `addons/payment_toss_payments/i18n/vi.po` (160 lines)
- `addons/payment_toss_payments/i18n/zh_CN.po` (162 lines)
- `addons/payment_toss_payments/i18n/zh_TW.po` (161 lines)
- `addons/payment_toss_payments/models/__init__.py` (1 lines)
- `addons/payment_toss_payments/models/payment_provider.py` (114 lines)
- `addons/payment_toss_payments/models/payment_transaction.py` (107 lines)
- `addons/payment_toss_payments/static/description/icon.png` (155 lines)
- `addons/payment_toss_payments/static/src/interactions/payment_form.js` (124 lines)
- `addons/payment_toss_payments/tests/__init__.py` (1 lines)
- `addons/payment_toss_payments/tests/common.py` (39 lines)
- `addons/payment_toss_payments/tests/test_payment_transaction.py` (51 lines)
- `addons/payment_toss_payments/tests/test_processing_flows.py` (83 lines)
- `addons/payment_toss_payments/views/payment_provider_views.xml` (34 lines)
- `addons/payment_toss_payments/views/payment_toss_payments_templates.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
