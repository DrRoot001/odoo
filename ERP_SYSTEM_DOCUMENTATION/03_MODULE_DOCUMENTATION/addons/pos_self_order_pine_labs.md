# Module: pos_self_order_pine_labs

- **Module ID:** MOD-458
- **Path:** `addons/pos_self_order_pine_labs`
- **Manifest:** `addons/pos_self_order_pine_labs/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

An addon for the Self Order App (KIOSK) that allows customers to pay using the Pine Labs POS Terminal.

No manifest description declared.

Declared dependencies: `pos_pine_labs`, `pos_self_order`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 3 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 2 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "pos_pine_labs",
    "pos_self_order"
  ],
  "assets": {
    "pos_self_order.assets": [
      "pos_self_order_pine_labs/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_self_order_pine_labs/__init__.py` (4 lines)
- `addons/pos_self_order_pine_labs/__manifest__.py` (16 lines)
- `addons/pos_self_order_pine_labs/controllers/__init__.py` (3 lines)
- `addons/pos_self_order_pine_labs/controllers/orders.py` (73 lines)
- `addons/pos_self_order_pine_labs/i18n/ar.po` (54 lines)
- `addons/pos_self_order_pine_labs/i18n/az.po` (52 lines)
- `addons/pos_self_order_pine_labs/i18n/bg.po` (52 lines)
- `addons/pos_self_order_pine_labs/i18n/bs.po` (54 lines)
- `addons/pos_self_order_pine_labs/i18n/ca.po` (52 lines)
- `addons/pos_self_order_pine_labs/i18n/cs.po` (53 lines)
- `addons/pos_self_order_pine_labs/i18n/da.po` (52 lines)
- `addons/pos_self_order_pine_labs/i18n/de.po` (55 lines)
- `addons/pos_self_order_pine_labs/i18n/el.po` (52 lines)
- `addons/pos_self_order_pine_labs/i18n/es.po` (53 lines)
- `addons/pos_self_order_pine_labs/i18n/es_419.po` (54 lines)
- `addons/pos_self_order_pine_labs/i18n/et.po` (52 lines)
- `addons/pos_self_order_pine_labs/i18n/fa.po` (52 lines)
- `addons/pos_self_order_pine_labs/i18n/fi.po` (53 lines)
- `addons/pos_self_order_pine_labs/i18n/fr.po` (53 lines)
- `addons/pos_self_order_pine_labs/i18n/he.po` (53 lines)
- `addons/pos_self_order_pine_labs/i18n/hi.po` (52 lines)
- `addons/pos_self_order_pine_labs/i18n/hr.po` (53 lines)
- `addons/pos_self_order_pine_labs/i18n/hu.po` (52 lines)
- `addons/pos_self_order_pine_labs/i18n/id.po` (53 lines)
- `addons/pos_self_order_pine_labs/i18n/it.po` (53 lines)
- `addons/pos_self_order_pine_labs/i18n/ja.po` (53 lines)
- `addons/pos_self_order_pine_labs/i18n/kab.po` (53 lines)
- `addons/pos_self_order_pine_labs/i18n/ko.po` (53 lines)
- `addons/pos_self_order_pine_labs/i18n/ku.po` (52 lines)
- `addons/pos_self_order_pine_labs/i18n/lo.po` (52 lines)
- `addons/pos_self_order_pine_labs/i18n/lt.po` (54 lines)
- `addons/pos_self_order_pine_labs/i18n/lv.po` (53 lines)
- `addons/pos_self_order_pine_labs/i18n/mn.po` (52 lines)
- `addons/pos_self_order_pine_labs/i18n/my.po` (52 lines)
- `addons/pos_self_order_pine_labs/i18n/nb.po` (52 lines)
- `addons/pos_self_order_pine_labs/i18n/nl.po` (54 lines)
- `addons/pos_self_order_pine_labs/i18n/pl.po` (53 lines)
- `addons/pos_self_order_pine_labs/i18n/pos_self_order_pine_labs.pot` (49 lines)
- `addons/pos_self_order_pine_labs/i18n/pt.po` (52 lines)
- `addons/pos_self_order_pine_labs/i18n/pt_BR.po` (56 lines)
- `addons/pos_self_order_pine_labs/i18n/ro.po` (54 lines)
- `addons/pos_self_order_pine_labs/i18n/ru.po` (54 lines)
- `addons/pos_self_order_pine_labs/i18n/sk.po` (52 lines)
- `addons/pos_self_order_pine_labs/i18n/sl.po` (53 lines)
- `addons/pos_self_order_pine_labs/i18n/sr@latin.po` (53 lines)
- `addons/pos_self_order_pine_labs/i18n/sv.po` (53 lines)
- `addons/pos_self_order_pine_labs/i18n/th.po` (53 lines)
- `addons/pos_self_order_pine_labs/i18n/tr.po` (55 lines)
- `addons/pos_self_order_pine_labs/i18n/uk.po` (53 lines)
- `addons/pos_self_order_pine_labs/i18n/uz.po` (63 lines)
- `addons/pos_self_order_pine_labs/i18n/vi.po` (53 lines)
- `addons/pos_self_order_pine_labs/i18n/zh_CN.po` (53 lines)
- `addons/pos_self_order_pine_labs/i18n/zh_TW.po` (53 lines)
- `addons/pos_self_order_pine_labs/models/__init__.py` (3 lines)
- `addons/pos_self_order_pine_labs/models/pos_payment_method.py` (40 lines)
- `addons/pos_self_order_pine_labs/static/src/app/pages/payment_page.js` (16 lines)
- `addons/pos_self_order_pine_labs/static/src/app/pine_labs.js` (175 lines)
- `addons/pos_self_order_pine_labs/static/src/app/services/self_order_service.js` (41 lines)
- `addons/pos_self_order_pine_labs/tests/__init__.py` (3 lines)
- `addons/pos_self_order_pine_labs/tests/test_pine_labs_payment_status.py` (151 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
