# Module: pos_cashmatic

- **Module ID:** MOD-426
- **Path:** `addons/pos_cashmatic`
- **Manifest:** `addons/pos_cashmatic/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Integrate your POS with a cash matic automatic cash payment device

No manifest description declared.

Declared dependencies: `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 4 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

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
    "point_of_sale._assets_pos": [
      "pos_cashmatic/static/src/**/*"
    ],
    "point_of_sale.payment_terminals": [
      "pos_cashmatic/static/src/cashmatic_service.js",
      "pos_cashmatic/static/src/app/payment_cashmatic.js"
    ],
    "web.assets_unit_tests": [
      "pos_cashmatic/static/tests/**/*",
      "pos_cashmatic/static/src/cashmatic_service.js"
    ]
  }
}
```

### Representative source files

- `addons/pos_cashmatic/__init__.py` (1 lines)
- `addons/pos_cashmatic/__manifest__.py` (24 lines)
- `addons/pos_cashmatic/data/neutralize.sql` (2 lines)
- `addons/pos_cashmatic/i18n/ar.po` (109 lines)
- `addons/pos_cashmatic/i18n/az.po` (107 lines)
- `addons/pos_cashmatic/i18n/bg.po` (107 lines)
- `addons/pos_cashmatic/i18n/bs.po` (108 lines)
- `addons/pos_cashmatic/i18n/ca.po` (107 lines)
- `addons/pos_cashmatic/i18n/cs.po` (107 lines)
- `addons/pos_cashmatic/i18n/da.po` (107 lines)
- `addons/pos_cashmatic/i18n/de.po` (112 lines)
- `addons/pos_cashmatic/i18n/el.po` (107 lines)
- `addons/pos_cashmatic/i18n/es.po` (112 lines)
- `addons/pos_cashmatic/i18n/es_419.po` (110 lines)
- `addons/pos_cashmatic/i18n/et.po` (107 lines)
- `addons/pos_cashmatic/i18n/fa.po` (107 lines)
- `addons/pos_cashmatic/i18n/fi.po` (110 lines)
- `addons/pos_cashmatic/i18n/fr.po` (110 lines)
- `addons/pos_cashmatic/i18n/he.po` (108 lines)
- `addons/pos_cashmatic/i18n/hi.po` (107 lines)
- `addons/pos_cashmatic/i18n/hr.po` (108 lines)
- `addons/pos_cashmatic/i18n/hu.po` (107 lines)
- `addons/pos_cashmatic/i18n/id.po` (107 lines)
- `addons/pos_cashmatic/i18n/it.po` (110 lines)
- `addons/pos_cashmatic/i18n/ja.po` (107 lines)
- `addons/pos_cashmatic/i18n/kab.po` (107 lines)
- `addons/pos_cashmatic/i18n/ko.po` (107 lines)
- `addons/pos_cashmatic/i18n/ku.po` (107 lines)
- `addons/pos_cashmatic/i18n/lo.po` (107 lines)
- `addons/pos_cashmatic/i18n/lt.po` (109 lines)
- `addons/pos_cashmatic/i18n/lv.po` (108 lines)
- `addons/pos_cashmatic/i18n/mn.po` (107 lines)
- `addons/pos_cashmatic/i18n/my.po` (107 lines)
- `addons/pos_cashmatic/i18n/nb.po` (107 lines)
- `addons/pos_cashmatic/i18n/nl.po` (111 lines)
- `addons/pos_cashmatic/i18n/pl.po` (108 lines)
- `addons/pos_cashmatic/i18n/pos_cashmatic.pot` (104 lines)
- `addons/pos_cashmatic/i18n/pt.po` (107 lines)
- `addons/pos_cashmatic/i18n/pt_BR.po` (114 lines)
- `addons/pos_cashmatic/i18n/ro.po` (111 lines)
- `addons/pos_cashmatic/i18n/ru.po` (111 lines)
- `addons/pos_cashmatic/i18n/sk.po` (107 lines)
- `addons/pos_cashmatic/i18n/sl.po` (108 lines)
- `addons/pos_cashmatic/i18n/sr@latin.po` (108 lines)
- `addons/pos_cashmatic/i18n/sv.po` (108 lines)
- `addons/pos_cashmatic/i18n/th.po` (107 lines)
- `addons/pos_cashmatic/i18n/tr.po` (107 lines)
- `addons/pos_cashmatic/i18n/uk.po` (108 lines)
- `addons/pos_cashmatic/i18n/uz.po` (107 lines)
- `addons/pos_cashmatic/i18n/vi.po` (107 lines)
- `addons/pos_cashmatic/i18n/zh_CN.po` (109 lines)
- `addons/pos_cashmatic/i18n/zh_TW.po` (107 lines)
- `addons/pos_cashmatic/models/__init__.py` (1 lines)
- `addons/pos_cashmatic/models/pos_payment_method.py` (16 lines)
- `addons/pos_cashmatic/static/description/icon.png` (37 lines)
- `addons/pos_cashmatic/static/src/app/payment_cashmatic.js` (121 lines)
- `addons/pos_cashmatic/static/src/app/screens/payment_screen/payment_lines/payment_lines.xml` (12 lines)
- `addons/pos_cashmatic/static/src/app/screens/payment_screen/payment_screen.js` (12 lines)
- `addons/pos_cashmatic/static/src/cashmatic_service.js` (131 lines)
- `addons/pos_cashmatic/static/tests/cashmatic_service.test.js` (155 lines)
- `addons/pos_cashmatic/views/pos_payment_method_views.xml` (24 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
