# Module: pos_mercado_pago

- **Module ID:** MOD-437
- **Path:** `addons/pos_mercado_pago`
- **Manifest:** `addons/pos_mercado_pago/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Integrate your POS with the Mercado Pago Smart Point terminal

No manifest description declared.

Declared dependencies: `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "point_of_sale"
  ],
  "data": [
    "views/pos_payment_method_views.xml"
  ],
  "assets": {
    "point_of_sale.payment_terminals": [
      "pos_mercado_pago/static/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_mercado_pago/__init__.py` (2 lines)
- `addons/pos_mercado_pago/__manifest__.py` (17 lines)
- `addons/pos_mercado_pago/controllers/__init__.py` (3 lines)
- `addons/pos_mercado_pago/controllers/main.py` (93 lines)
- `addons/pos_mercado_pago/data/neutralize.sql` (4 lines)
- `addons/pos_mercado_pago/i18n/ar.po` (246 lines)
- `addons/pos_mercado_pago/i18n/az.po` (237 lines)
- `addons/pos_mercado_pago/i18n/bg.po` (237 lines)
- `addons/pos_mercado_pago/i18n/bs.po` (239 lines)
- `addons/pos_mercado_pago/i18n/ca.po` (240 lines)
- `addons/pos_mercado_pago/i18n/cs.po` (238 lines)
- `addons/pos_mercado_pago/i18n/da.po` (245 lines)
- `addons/pos_mercado_pago/i18n/de.po` (254 lines)
- `addons/pos_mercado_pago/i18n/el.po` (238 lines)
- `addons/pos_mercado_pago/i18n/es.po` (245 lines)
- `addons/pos_mercado_pago/i18n/es_419.po` (247 lines)
- `addons/pos_mercado_pago/i18n/et.po` (237 lines)
- `addons/pos_mercado_pago/i18n/fa.po` (237 lines)
- `addons/pos_mercado_pago/i18n/fi.po` (247 lines)
- `addons/pos_mercado_pago/i18n/fr.po` (248 lines)
- `addons/pos_mercado_pago/i18n/he.po` (238 lines)
- `addons/pos_mercado_pago/i18n/hi.po` (237 lines)
- `addons/pos_mercado_pago/i18n/hr.po` (238 lines)
- `addons/pos_mercado_pago/i18n/hu.po` (238 lines)
- `addons/pos_mercado_pago/i18n/id.po` (245 lines)
- `addons/pos_mercado_pago/i18n/it.po` (247 lines)
- `addons/pos_mercado_pago/i18n/ja.po` (245 lines)
- `addons/pos_mercado_pago/i18n/kab.po` (238 lines)
- `addons/pos_mercado_pago/i18n/ko.po` (244 lines)
- `addons/pos_mercado_pago/i18n/ku.po` (237 lines)
- `addons/pos_mercado_pago/i18n/lo.po` (245 lines)
- `addons/pos_mercado_pago/i18n/lt.po` (239 lines)
- `addons/pos_mercado_pago/i18n/lv.po` (238 lines)
- `addons/pos_mercado_pago/i18n/mn.po` (237 lines)
- `addons/pos_mercado_pago/i18n/my.po` (237 lines)
- `addons/pos_mercado_pago/i18n/nb.po` (238 lines)
- `addons/pos_mercado_pago/i18n/nl.po` (249 lines)
- `addons/pos_mercado_pago/i18n/pl.po` (247 lines)
- `addons/pos_mercado_pago/i18n/pos_mercado_pago.pot` (234 lines)
- `addons/pos_mercado_pago/i18n/pt.po` (245 lines)
- `addons/pos_mercado_pago/i18n/pt_BR.po` (252 lines)
- `addons/pos_mercado_pago/i18n/ro.po` (247 lines)
- `addons/pos_mercado_pago/i18n/ru.po` (249 lines)
- `addons/pos_mercado_pago/i18n/sk.po` (237 lines)
- `addons/pos_mercado_pago/i18n/sl.po` (239 lines)
- `addons/pos_mercado_pago/i18n/sr@latin.po` (238 lines)
- `addons/pos_mercado_pago/i18n/sv.po` (245 lines)
- `addons/pos_mercado_pago/i18n/th.po` (244 lines)
- `addons/pos_mercado_pago/i18n/tr.po` (246 lines)
- `addons/pos_mercado_pago/i18n/uk.po` (238 lines)
- `addons/pos_mercado_pago/i18n/uz.po` (274 lines)
- `addons/pos_mercado_pago/i18n/vi.po` (246 lines)
- `addons/pos_mercado_pago/i18n/zh_CN.po` (244 lines)
- `addons/pos_mercado_pago/i18n/zh_TW.po` (245 lines)
- `addons/pos_mercado_pago/models/__init__.py` (2 lines)
- `addons/pos_mercado_pago/models/mercado_pago_pos_request.py` (51 lines)
- `addons/pos_mercado_pago/models/pos_payment_method.py` (141 lines)
- `addons/pos_mercado_pago/static/src/app/utils/payment/payment_mercado_pago.js` (267 lines)
- `addons/pos_mercado_pago/tests/__init__.py` (2 lines)
- `addons/pos_mercado_pago/tests/test_mercado_pago_orders.py` (146 lines)
- `addons/pos_mercado_pago/tests/test_webhook_controller.py` (137 lines)
- `addons/pos_mercado_pago/views/pos_payment_method_views.xml` (23 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
