# Module: pos_mollie

- **Module ID:** MOD-438
- **Path:** `addons/pos_mollie`
- **Manifest:** `addons/pos_mollie/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Integrate your POS with a Mollie payment terminal

No manifest description declared.

Declared dependencies: `point_of_sale`, `payment_mollie`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 4 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "point_of_sale",
    "payment_mollie"
  ],
  "data": [
    "views/pos_payment_method_views.xml"
  ],
  "assets": {
    "point_of_sale.payment_terminals": [
      "pos_mollie/static/src/**/*"
    ],
    "web.assets_unit_tests": [
      "pos_mollie/static/tests/unit/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_mollie/__init__.py` (2 lines)
- `addons/pos_mollie/__manifest__.py` (20 lines)
- `addons/pos_mollie/controllers/__init__.py` (1 lines)
- `addons/pos_mollie/controllers/webhook.py` (52 lines)
- `addons/pos_mollie/i18n/ar.po` (119 lines)
- `addons/pos_mollie/i18n/az.po` (115 lines)
- `addons/pos_mollie/i18n/bg.po` (115 lines)
- `addons/pos_mollie/i18n/bs.po` (116 lines)
- `addons/pos_mollie/i18n/ca.po` (115 lines)
- `addons/pos_mollie/i18n/cs.po` (115 lines)
- `addons/pos_mollie/i18n/da.po` (115 lines)
- `addons/pos_mollie/i18n/de.po` (122 lines)
- `addons/pos_mollie/i18n/el.po` (115 lines)
- `addons/pos_mollie/i18n/es.po` (118 lines)
- `addons/pos_mollie/i18n/es_419.po` (121 lines)
- `addons/pos_mollie/i18n/et.po` (115 lines)
- `addons/pos_mollie/i18n/fa.po` (115 lines)
- `addons/pos_mollie/i18n/fi.po` (118 lines)
- `addons/pos_mollie/i18n/fr.po` (122 lines)
- `addons/pos_mollie/i18n/he.po` (116 lines)
- `addons/pos_mollie/i18n/hi.po` (115 lines)
- `addons/pos_mollie/i18n/hr.po` (116 lines)
- `addons/pos_mollie/i18n/hu.po` (115 lines)
- `addons/pos_mollie/i18n/id.po` (116 lines)
- `addons/pos_mollie/i18n/it.po` (120 lines)
- `addons/pos_mollie/i18n/ja.po` (117 lines)
- `addons/pos_mollie/i18n/kab.po` (115 lines)
- `addons/pos_mollie/i18n/ko.po` (116 lines)
- `addons/pos_mollie/i18n/ku.po` (115 lines)
- `addons/pos_mollie/i18n/lo.po` (115 lines)
- `addons/pos_mollie/i18n/lt.po` (117 lines)
- `addons/pos_mollie/i18n/lv.po` (116 lines)
- `addons/pos_mollie/i18n/mn.po` (115 lines)
- `addons/pos_mollie/i18n/my.po` (115 lines)
- `addons/pos_mollie/i18n/nb.po` (115 lines)
- `addons/pos_mollie/i18n/nl.po` (119 lines)
- `addons/pos_mollie/i18n/pl.po` (118 lines)
- `addons/pos_mollie/i18n/pos_mollie.pot` (112 lines)
- `addons/pos_mollie/i18n/pt.po` (115 lines)
- `addons/pos_mollie/i18n/pt_BR.po` (122 lines)
- `addons/pos_mollie/i18n/ro.po` (116 lines)
- `addons/pos_mollie/i18n/ru.po` (119 lines)
- `addons/pos_mollie/i18n/sk.po` (115 lines)
- `addons/pos_mollie/i18n/sl.po` (116 lines)
- `addons/pos_mollie/i18n/sr@latin.po` (116 lines)
- `addons/pos_mollie/i18n/sv.po` (120 lines)
- `addons/pos_mollie/i18n/th.po` (116 lines)
- `addons/pos_mollie/i18n/tr.po` (115 lines)
- `addons/pos_mollie/i18n/uk.po` (116 lines)
- `addons/pos_mollie/i18n/uz.po` (115 lines)
- `addons/pos_mollie/i18n/vi.po` (115 lines)
- `addons/pos_mollie/i18n/zh_CN.po` (116 lines)
- `addons/pos_mollie/i18n/zh_TW.po` (116 lines)
- `addons/pos_mollie/models/__init__.py` (1 lines)
- `addons/pos_mollie/models/pos_payment_method.py` (75 lines)
- `addons/pos_mollie/static/description/icon.png` (11 lines)
- `addons/pos_mollie/static/description/icon.svg` (1 lines)
- `addons/pos_mollie/static/src/payment_mollie.js` (235 lines)
- `addons/pos_mollie/static/tests/unit/data/pos_config.data.js` (6 lines)
- `addons/pos_mollie/static/tests/unit/data/pos_payment_method.data.js` (15 lines)
- `addons/pos_mollie/static/tests/unit/payment_mollie.test.js` (98 lines)
- `addons/pos_mollie/tests/__init__.py` (1 lines)
- `addons/pos_mollie/tests/test_mollie_payment_method.py` (79 lines)
- `addons/pos_mollie/views/pos_payment_method_views.xml` (20 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
