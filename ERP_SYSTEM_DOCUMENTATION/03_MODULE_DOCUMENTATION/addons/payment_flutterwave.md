# Module: payment_flutterwave

- **Module ID:** MOD-402
- **Path:** `addons/payment_flutterwave`
- **Manifest:** `addons/payment_flutterwave/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

A Nigerian payment provider covering several African countries.

 

Declared dependencies: `payment`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 14 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
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
    "views/payment_provider_views.xml",
    "data/payment_method_data.xml",
    "data/payment_provider_data.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "payment_flutterwave/static/src/interactions/payment_form.js"
    ]
  }
}
```

### Representative source files

- `addons/payment_flutterwave/README.md` (39 lines)
- `addons/payment_flutterwave/__init__.py` (12 lines)
- `addons/payment_flutterwave/__manifest__.py` (22 lines)
- `addons/payment_flutterwave/const.py` (43 lines)
- `addons/payment_flutterwave/controllers/__init__.py` (3 lines)
- `addons/payment_flutterwave/controllers/main.py` (91 lines)
- `addons/payment_flutterwave/data/neutralize.sql` (5 lines)
- `addons/payment_flutterwave/data/payment_method_data.xml` (154 lines)
- `addons/payment_flutterwave/data/payment_provider_data.xml` (10 lines)
- `addons/payment_flutterwave/i18n/ar.po` (188 lines)
- `addons/payment_flutterwave/i18n/az.po` (185 lines)
- `addons/payment_flutterwave/i18n/bg.po` (185 lines)
- `addons/payment_flutterwave/i18n/bs.po` (186 lines)
- `addons/payment_flutterwave/i18n/ca.po` (186 lines)
- `addons/payment_flutterwave/i18n/cs.po` (186 lines)
- `addons/payment_flutterwave/i18n/da.po` (187 lines)
- `addons/payment_flutterwave/i18n/de.po` (189 lines)
- `addons/payment_flutterwave/i18n/el.po` (186 lines)
- `addons/payment_flutterwave/i18n/es.po` (187 lines)
- `addons/payment_flutterwave/i18n/es_419.po` (186 lines)
- `addons/payment_flutterwave/i18n/et.po` (185 lines)
- `addons/payment_flutterwave/i18n/fa.po` (185 lines)
- `addons/payment_flutterwave/i18n/fi.po` (186 lines)
- `addons/payment_flutterwave/i18n/fr.po` (186 lines)
- `addons/payment_flutterwave/i18n/he.po` (186 lines)
- `addons/payment_flutterwave/i18n/hi.po` (185 lines)
- `addons/payment_flutterwave/i18n/hr.po` (186 lines)
- `addons/payment_flutterwave/i18n/hu.po` (186 lines)
- `addons/payment_flutterwave/i18n/id.po` (187 lines)
- `addons/payment_flutterwave/i18n/it.po` (188 lines)
- `addons/payment_flutterwave/i18n/ja.po` (186 lines)
- `addons/payment_flutterwave/i18n/kab.po` (185 lines)
- `addons/payment_flutterwave/i18n/ko.po` (187 lines)
- `addons/payment_flutterwave/i18n/ku.po` (185 lines)
- `addons/payment_flutterwave/i18n/lo.po` (186 lines)
- `addons/payment_flutterwave/i18n/lt.po` (187 lines)
- `addons/payment_flutterwave/i18n/lv.po` (185 lines)
- `addons/payment_flutterwave/i18n/mn.po` (185 lines)
- `addons/payment_flutterwave/i18n/my.po` (185 lines)
- `addons/payment_flutterwave/i18n/nb.po` (186 lines)
- `addons/payment_flutterwave/i18n/nl.po` (189 lines)
- `addons/payment_flutterwave/i18n/payment_flutterwave.pot` (181 lines)
- `addons/payment_flutterwave/i18n/pl.po` (188 lines)
- `addons/payment_flutterwave/i18n/pt.po` (188 lines)
- `addons/payment_flutterwave/i18n/pt_BR.po` (190 lines)
- `addons/payment_flutterwave/i18n/ro.po` (186 lines)
- `addons/payment_flutterwave/i18n/ru.po` (191 lines)
- `addons/payment_flutterwave/i18n/sk.po` (184 lines)
- `addons/payment_flutterwave/i18n/sl.po` (187 lines)
- `addons/payment_flutterwave/i18n/sr@latin.po` (186 lines)
- `addons/payment_flutterwave/i18n/sv.po` (187 lines)
- `addons/payment_flutterwave/i18n/th.po` (187 lines)
- `addons/payment_flutterwave/i18n/tr.po` (189 lines)
- `addons/payment_flutterwave/i18n/uk.po` (188 lines)
- `addons/payment_flutterwave/i18n/uz.po` (210 lines)
- `addons/payment_flutterwave/i18n/vi.po` (187 lines)
- `addons/payment_flutterwave/i18n/zh_CN.po` (188 lines)
- `addons/payment_flutterwave/i18n/zh_TW.po` (188 lines)
- `addons/payment_flutterwave/models/__init__.py` (3 lines)
- `addons/payment_flutterwave/models/payment_provider.py` (109 lines)
- `addons/payment_flutterwave/models/payment_token.py` (11 lines)
- `addons/payment_flutterwave/models/payment_transaction.py` (211 lines)
- `addons/payment_flutterwave/static/description/icon.png` (14 lines)
- `addons/payment_flutterwave/static/description/icon.svg` (1 lines)
- `addons/payment_flutterwave/static/description/icon_hi.png` (126 lines)
- `addons/payment_flutterwave/static/src/interactions/payment_form.js` (25 lines)
- `addons/payment_flutterwave/tests/__init__.py` (3 lines)
- `addons/payment_flutterwave/tests/common.py` (35 lines)
- `addons/payment_flutterwave/tests/test_payment_provider.py` (30 lines)
- `addons/payment_flutterwave/tests/test_payment_transaction.py` (65 lines)
- `addons/payment_flutterwave/tests/test_processing_flows.py` (70 lines)
- `addons/payment_flutterwave/views/payment_provider_views.xml` (34 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
