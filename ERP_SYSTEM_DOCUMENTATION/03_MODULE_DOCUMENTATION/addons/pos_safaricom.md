# Module: pos_safaricom

- **Module ID:** MOD-449
- **Path:** `addons/pos_safaricom`
- **Manifest:** `addons/pos_safaricom/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Integrate your POS with the Safaricom Payment Provider

No manifest description declared.

Declared dependencies: `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 8 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 3 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "point_of_sale"
  ],
  "data": [
    "views/pos_payment_method_views.xml",
    "security/ir.access.csv",
    "receipt/pos_order_receipt.xml"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "pos_safaricom/static/src/**/*"
    ],
    "web.assets_unit_tests": [
      "pos_safaricom/static/tests/unit/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_safaricom/__init__.py` (1 lines)
- `addons/pos_safaricom/__manifest__.py` (21 lines)
- `addons/pos_safaricom/controllers/__init__.py` (1 lines)
- `addons/pos_safaricom/controllers/main.py` (76 lines)
- `addons/pos_safaricom/i18n/ar.po` (371 lines)
- `addons/pos_safaricom/i18n/az.po` (367 lines)
- `addons/pos_safaricom/i18n/bg.po` (367 lines)
- `addons/pos_safaricom/i18n/bs.po` (368 lines)
- `addons/pos_safaricom/i18n/ca.po` (367 lines)
- `addons/pos_safaricom/i18n/cs.po` (367 lines)
- `addons/pos_safaricom/i18n/da.po` (367 lines)
- `addons/pos_safaricom/i18n/de.po` (387 lines)
- `addons/pos_safaricom/i18n/el.po` (367 lines)
- `addons/pos_safaricom/i18n/es.po` (386 lines)
- `addons/pos_safaricom/i18n/es_419.po` (386 lines)
- `addons/pos_safaricom/i18n/et.po` (367 lines)
- `addons/pos_safaricom/i18n/fa.po` (367 lines)
- `addons/pos_safaricom/i18n/fi.po` (381 lines)
- `addons/pos_safaricom/i18n/fr.po` (386 lines)
- `addons/pos_safaricom/i18n/he.po` (368 lines)
- `addons/pos_safaricom/i18n/hi.po` (367 lines)
- `addons/pos_safaricom/i18n/hr.po` (368 lines)
- `addons/pos_safaricom/i18n/hu.po` (367 lines)
- `addons/pos_safaricom/i18n/id.po` (368 lines)
- `addons/pos_safaricom/i18n/it.po` (384 lines)
- `addons/pos_safaricom/i18n/ja.po` (379 lines)
- `addons/pos_safaricom/i18n/kab.po` (367 lines)
- `addons/pos_safaricom/i18n/ko.po` (367 lines)
- `addons/pos_safaricom/i18n/ku.po` (367 lines)
- `addons/pos_safaricom/i18n/lo.po` (374 lines)
- `addons/pos_safaricom/i18n/lt.po` (369 lines)
- `addons/pos_safaricom/i18n/lv.po` (368 lines)
- `addons/pos_safaricom/i18n/mn.po` (367 lines)
- `addons/pos_safaricom/i18n/my.po` (368 lines)
- `addons/pos_safaricom/i18n/nb.po` (367 lines)
- `addons/pos_safaricom/i18n/nl.po` (382 lines)
- `addons/pos_safaricom/i18n/pl.po` (384 lines)
- `addons/pos_safaricom/i18n/pos_safaricom.pot` (362 lines)
- `addons/pos_safaricom/i18n/pt.po` (367 lines)
- `addons/pos_safaricom/i18n/pt_BR.po` (383 lines)
- `addons/pos_safaricom/i18n/ro.po` (368 lines)
- `addons/pos_safaricom/i18n/ru.po` (370 lines)
- `addons/pos_safaricom/i18n/sk.po` (367 lines)
- `addons/pos_safaricom/i18n/sl.po` (368 lines)
- `addons/pos_safaricom/i18n/sr@latin.po` (368 lines)
- `addons/pos_safaricom/i18n/sv.po` (368 lines)
- `addons/pos_safaricom/i18n/th.po` (368 lines)
- `addons/pos_safaricom/i18n/tr.po` (367 lines)
- `addons/pos_safaricom/i18n/uk.po` (368 lines)
- `addons/pos_safaricom/i18n/uz.po` (367 lines)
- `addons/pos_safaricom/i18n/vi.po` (367 lines)
- `addons/pos_safaricom/i18n/zh_CN.po` (372 lines)
- `addons/pos_safaricom/i18n/zh_TW.po` (371 lines)
- `addons/pos_safaricom/models/__init__.py` (3 lines)
- `addons/pos_safaricom/models/pos_payment.py` (7 lines)
- `addons/pos_safaricom/models/pos_payment_method.py` (335 lines)
- `addons/pos_safaricom/models/transaction_lipa_na_mpesa.py` (12 lines)
- `addons/pos_safaricom/receipt/__init__.py` (1 lines)
- `addons/pos_safaricom/receipt/pos_order_receipt.py` (12 lines)
- `addons/pos_safaricom/receipt/pos_order_receipt.xml` (13 lines)
- `addons/pos_safaricom/security/ir.access.csv` (2 lines)
- `addons/pos_safaricom/static/src/app/components/popups/mpesa_transaction_popup.js` (76 lines)
- `addons/pos_safaricom/static/src/app/components/popups/mpesa_transaction_popup.xml` (69 lines)
- `addons/pos_safaricom/static/src/app/models/pos_payment.js` (8 lines)
- `addons/pos_safaricom/static/src/app/payment_safaricom.js` (209 lines)
- `addons/pos_safaricom/static/src/app/services/pos_store.js` (55 lines)
- `addons/pos_safaricom/static/tests/unit/customer_display/customer_display.test.js` (37 lines)
- `addons/pos_safaricom/static/tests/unit/data/pos_payment_method.data.js` (42 lines)
- `addons/pos_safaricom/static/tests/unit/data/transaction_lipa_na_mpesa.data.js` (20 lines)
- `addons/pos_safaricom/static/tests/unit/scenarios/safaricom_flow.test.js` (99 lines)
- `addons/pos_safaricom/tests/__init__.py` (1 lines)
- `addons/pos_safaricom/tests/test_pos_safaricom.py` (164 lines)
- `addons/pos_safaricom/views/pos_payment_method_views.xml` (44 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
