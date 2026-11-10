# Module: payment_mercado_pago

- **Module ID:** MOD-404
- **Path:** `addons/payment_mercado_pago`
- **Manifest:** `addons/payment_mercado_pago/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

A payment provider covering several countries in Latin America.

 

Declared dependencies: `payment`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 15 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 4 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "payment"
  ],
  "data": [
    "views/payment_form_templates.xml",
    "views/payment_mercado_pago_templates.xml",
    "views/payment_provider_views.xml",
    "data/payment_method_data.xml",
    "data/payment_provider_data.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "payment_mercado_pago/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/payment_mercado_pago/README.md` (54 lines)
- `addons/payment_mercado_pago/__init__.py` (12 lines)
- `addons/payment_mercado_pago/__manifest__.py` (22 lines)
- `addons/payment_mercado_pago/const.py` (115 lines)
- `addons/payment_mercado_pago/controllers/__init__.py` (3 lines)
- `addons/payment_mercado_pago/controllers/onboarding.py` (87 lines)
- `addons/payment_mercado_pago/controllers/payment.py` (123 lines)
- `addons/payment_mercado_pago/data/neutralize.sql` (3 lines)
- `addons/payment_mercado_pago/data/payment_method_data.xml` (210 lines)
- `addons/payment_mercado_pago/data/payment_provider_data.xml` (10 lines)
- `addons/payment_mercado_pago/i18n/ar.po` (486 lines)
- `addons/payment_mercado_pago/i18n/az.po` (467 lines)
- `addons/payment_mercado_pago/i18n/bg.po` (466 lines)
- `addons/payment_mercado_pago/i18n/bs.po` (476 lines)
- `addons/payment_mercado_pago/i18n/ca.po` (471 lines)
- `addons/payment_mercado_pago/i18n/cs.po` (467 lines)
- `addons/payment_mercado_pago/i18n/da.po` (505 lines)
- `addons/payment_mercado_pago/i18n/de.po` (500 lines)
- `addons/payment_mercado_pago/i18n/el.po` (467 lines)
- `addons/payment_mercado_pago/i18n/es.po` (494 lines)
- `addons/payment_mercado_pago/i18n/es_419.po` (490 lines)
- `addons/payment_mercado_pago/i18n/et.po` (466 lines)
- `addons/payment_mercado_pago/i18n/fa.po` (466 lines)
- `addons/payment_mercado_pago/i18n/fi.po` (501 lines)
- `addons/payment_mercado_pago/i18n/fr.po` (501 lines)
- `addons/payment_mercado_pago/i18n/he.po` (468 lines)
- `addons/payment_mercado_pago/i18n/hi.po` (473 lines)
- `addons/payment_mercado_pago/i18n/hr.po` (469 lines)
- `addons/payment_mercado_pago/i18n/hu.po` (467 lines)
- `addons/payment_mercado_pago/i18n/id.po` (495 lines)
- `addons/payment_mercado_pago/i18n/it.po` (499 lines)
- `addons/payment_mercado_pago/i18n/ja.po` (490 lines)
- `addons/payment_mercado_pago/i18n/kab.po` (473 lines)
- `addons/payment_mercado_pago/i18n/ko.po` (480 lines)
- `addons/payment_mercado_pago/i18n/ku.po` (466 lines)
- `addons/payment_mercado_pago/i18n/lo.po` (484 lines)
- `addons/payment_mercado_pago/i18n/lt.po` (468 lines)
- `addons/payment_mercado_pago/i18n/lv.po` (483 lines)
- `addons/payment_mercado_pago/i18n/mn.po` (467 lines)
- `addons/payment_mercado_pago/i18n/my.po` (466 lines)
- `addons/payment_mercado_pago/i18n/nb.po` (467 lines)
- `addons/payment_mercado_pago/i18n/nl.po` (495 lines)
- `addons/payment_mercado_pago/i18n/payment_mercado_pago.pot` (461 lines)
- `addons/payment_mercado_pago/i18n/pl.po` (534 lines)
- `addons/payment_mercado_pago/i18n/pt.po` (484 lines)
- `addons/payment_mercado_pago/i18n/pt_BR.po` (497 lines)
- `addons/payment_mercado_pago/i18n/ro.po` (483 lines)
- `addons/payment_mercado_pago/i18n/ru.po` (499 lines)
- `addons/payment_mercado_pago/i18n/sk.po` (480 lines)
- `addons/payment_mercado_pago/i18n/sl.po` (469 lines)
- `addons/payment_mercado_pago/i18n/sr@latin.po` (467 lines)
- `addons/payment_mercado_pago/i18n/sv.po` (486 lines)
- `addons/payment_mercado_pago/i18n/th.po` (477 lines)
- `addons/payment_mercado_pago/i18n/tr.po` (495 lines)
- `addons/payment_mercado_pago/i18n/uk.po` (483 lines)
- `addons/payment_mercado_pago/i18n/uz.po` (552 lines)
- `addons/payment_mercado_pago/i18n/vi.po` (493 lines)
- `addons/payment_mercado_pago/i18n/zh_CN.po` (479 lines)
- `addons/payment_mercado_pago/i18n/zh_TW.po` (476 lines)
- `addons/payment_mercado_pago/models/__init__.py` (3 lines)
- `addons/payment_mercado_pago/models/payment_provider.py` (326 lines)
- `addons/payment_mercado_pago/models/payment_token.py` (10 lines)
- `addons/payment_mercado_pago/models/payment_transaction.py` (307 lines)
- `addons/payment_mercado_pago/static/description/icon.png` (14 lines)
- `addons/payment_mercado_pago/static/description/icon.svg` (1 lines)
- `addons/payment_mercado_pago/static/description/icon_hi.png` (219 lines)
- `addons/payment_mercado_pago/static/src/interactions/payment_form.js` (165 lines)
- `addons/payment_mercado_pago/tests/__init__.py` (3 lines)
- `addons/payment_mercado_pago/tests/common.py` (27 lines)
- `addons/payment_mercado_pago/tests/test_payment_provider.py` (53 lines)
- `addons/payment_mercado_pago/tests/test_payment_transaction.py` (95 lines)
- `addons/payment_mercado_pago/tests/test_processing_flows.py` (49 lines)
- `addons/payment_mercado_pago/views/payment_form_templates.xml` (12 lines)
- `addons/payment_mercado_pago/views/payment_mercado_pago_templates.xml` (29 lines)
- `addons/payment_mercado_pago/views/payment_provider_views.xml` (75 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
