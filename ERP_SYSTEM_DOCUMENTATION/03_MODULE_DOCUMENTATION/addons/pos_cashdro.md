# Module: pos_cashdro

- **Module ID:** MOD-425
- **Path:** `addons/pos_cashdro`
- **Manifest:** `addons/pos_cashdro/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Integrate your POS with a Cashdro automatic cash payment device

No manifest description declared.

Declared dependencies: `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 5 | Client behavior/assets. |
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
    "web.assets_backend": [
      "pos_cashdro/static/src/cashdro_service.js",
      "pos_cashdro/static/src/backend/**/*"
    ],
    "point_of_sale._assets_pos": [
      "pos_cashdro/static/src/app/**/*"
    ],
    "point_of_sale.payment_terminals": [
      "pos_cashdro/static/src/cashdro_service.js",
      "pos_cashdro/static/src/app/payment_cashdro.js"
    ],
    "web.assets_unit_tests": [
      "pos_cashdro/static/tests/**/*",
      "pos_cashdro/static/src/cashdro_service.js"
    ]
  }
}
```

### Representative source files

- `addons/pos_cashdro/__init__.py` (1 lines)
- `addons/pos_cashdro/__manifest__.py` (28 lines)
- `addons/pos_cashdro/data/neutralize.sql` (2 lines)
- `addons/pos_cashdro/i18n/ar.po` (160 lines)
- `addons/pos_cashdro/i18n/az.po` (158 lines)
- `addons/pos_cashdro/i18n/bg.po` (158 lines)
- `addons/pos_cashdro/i18n/bs.po` (159 lines)
- `addons/pos_cashdro/i18n/ca.po` (158 lines)
- `addons/pos_cashdro/i18n/cs.po` (158 lines)
- `addons/pos_cashdro/i18n/da.po` (158 lines)
- `addons/pos_cashdro/i18n/de.po` (166 lines)
- `addons/pos_cashdro/i18n/el.po` (158 lines)
- `addons/pos_cashdro/i18n/es.po` (165 lines)
- `addons/pos_cashdro/i18n/es_419.po` (164 lines)
- `addons/pos_cashdro/i18n/et.po` (158 lines)
- `addons/pos_cashdro/i18n/fa.po` (158 lines)
- `addons/pos_cashdro/i18n/fi.po` (163 lines)
- `addons/pos_cashdro/i18n/fr.po` (163 lines)
- `addons/pos_cashdro/i18n/he.po` (159 lines)
- `addons/pos_cashdro/i18n/hi.po` (158 lines)
- `addons/pos_cashdro/i18n/hr.po` (159 lines)
- `addons/pos_cashdro/i18n/hu.po` (158 lines)
- `addons/pos_cashdro/i18n/id.po` (159 lines)
- `addons/pos_cashdro/i18n/it.po` (162 lines)
- `addons/pos_cashdro/i18n/ja.po` (162 lines)
- `addons/pos_cashdro/i18n/kab.po` (158 lines)
- `addons/pos_cashdro/i18n/ko.po` (158 lines)
- `addons/pos_cashdro/i18n/ku.po` (158 lines)
- `addons/pos_cashdro/i18n/lo.po` (160 lines)
- `addons/pos_cashdro/i18n/lt.po` (160 lines)
- `addons/pos_cashdro/i18n/lv.po` (159 lines)
- `addons/pos_cashdro/i18n/mn.po` (158 lines)
- `addons/pos_cashdro/i18n/my.po` (158 lines)
- `addons/pos_cashdro/i18n/nb.po` (158 lines)
- `addons/pos_cashdro/i18n/nl.po` (163 lines)
- `addons/pos_cashdro/i18n/pl.po` (163 lines)
- `addons/pos_cashdro/i18n/pos_cashdro.pot` (155 lines)
- `addons/pos_cashdro/i18n/pt.po` (158 lines)
- `addons/pos_cashdro/i18n/pt_BR.po` (166 lines)
- `addons/pos_cashdro/i18n/ro.po` (159 lines)
- `addons/pos_cashdro/i18n/ru.po` (164 lines)
- `addons/pos_cashdro/i18n/sk.po` (158 lines)
- `addons/pos_cashdro/i18n/sl.po` (159 lines)
- `addons/pos_cashdro/i18n/sr@latin.po` (159 lines)
- `addons/pos_cashdro/i18n/sv.po` (159 lines)
- `addons/pos_cashdro/i18n/th.po` (159 lines)
- `addons/pos_cashdro/i18n/tr.po` (158 lines)
- `addons/pos_cashdro/i18n/uk.po` (159 lines)
- `addons/pos_cashdro/i18n/uz.po` (158 lines)
- `addons/pos_cashdro/i18n/vi.po` (158 lines)
- `addons/pos_cashdro/i18n/zh_CN.po` (159 lines)
- `addons/pos_cashdro/i18n/zh_TW.po` (158 lines)
- `addons/pos_cashdro/models/__init__.py` (1 lines)
- `addons/pos_cashdro/models/pos_payment_method.py` (16 lines)
- `addons/pos_cashdro/static/description/icon.png` (41 lines)
- `addons/pos_cashdro/static/src/app/payment_cashdro.js` (181 lines)
- `addons/pos_cashdro/static/src/app/screens/payment_screen/payment_screen.js` (16 lines)
- `addons/pos_cashdro/static/src/backend/cashdro_admin_buttons/cashdro_admin_buttons.js` (61 lines)
- `addons/pos_cashdro/static/src/backend/cashdro_admin_buttons/cashdro_admin_buttons.xml` (21 lines)
- `addons/pos_cashdro/static/src/cashdro_service.js` (177 lines)
- `addons/pos_cashdro/static/tests/cashdro_service.test.js` (195 lines)
- `addons/pos_cashdro/views/pos_payment_method_views.xml` (25 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
