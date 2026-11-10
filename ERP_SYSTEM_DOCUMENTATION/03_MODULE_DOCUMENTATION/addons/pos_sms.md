# Module: pos_sms

- **Module ID:** MOD-463
- **Path:** `addons/pos_sms`
- **Manifest:** `addons/pos_sms/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

This module integrates the Point of Sale with SMS

Declared dependencies: `point_of_sale`, `sms`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 3 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "point_of_sale",
    "sms"
  ],
  "data": [
    "data/sms_data.xml",
    "views/res_config_settings_views.xml",
    "data/point_of_sale_data.xml"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "pos_sms/static/src/**/*"
    ],
    "web.assets_tests": [
      "pos_sms/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_sms/__init__.py` (5 lines)
- `addons/pos_sms/__manifest__.py` (22 lines)
- `addons/pos_sms/data/point_of_sale_data.xml` (6 lines)
- `addons/pos_sms/data/sms_data.xml` (12 lines)
- `addons/pos_sms/i18n/ar.po` (100 lines)
- `addons/pos_sms/i18n/az.po` (92 lines)
- `addons/pos_sms/i18n/bg.po` (92 lines)
- `addons/pos_sms/i18n/bs.po` (93 lines)
- `addons/pos_sms/i18n/ca.po` (99 lines)
- `addons/pos_sms/i18n/cs.po` (99 lines)
- `addons/pos_sms/i18n/da.po` (100 lines)
- `addons/pos_sms/i18n/de.po` (100 lines)
- `addons/pos_sms/i18n/el.po` (93 lines)
- `addons/pos_sms/i18n/es.po` (100 lines)
- `addons/pos_sms/i18n/es_419.po` (101 lines)
- `addons/pos_sms/i18n/et.po` (92 lines)
- `addons/pos_sms/i18n/fa.po` (92 lines)
- `addons/pos_sms/i18n/fi.po` (99 lines)
- `addons/pos_sms/i18n/fr.po` (99 lines)
- `addons/pos_sms/i18n/he.po` (93 lines)
- `addons/pos_sms/i18n/hi.po` (92 lines)
- `addons/pos_sms/i18n/hr.po` (93 lines)
- `addons/pos_sms/i18n/hu.po` (93 lines)
- `addons/pos_sms/i18n/id.po` (99 lines)
- `addons/pos_sms/i18n/it.po` (99 lines)
- `addons/pos_sms/i18n/ja.po` (99 lines)
- `addons/pos_sms/i18n/kab.po` (92 lines)
- `addons/pos_sms/i18n/ko.po` (99 lines)
- `addons/pos_sms/i18n/ku.po` (92 lines)
- `addons/pos_sms/i18n/lo.po` (91 lines)
- `addons/pos_sms/i18n/lt.po` (94 lines)
- `addons/pos_sms/i18n/lv.po` (92 lines)
- `addons/pos_sms/i18n/mn.po` (92 lines)
- `addons/pos_sms/i18n/my.po` (92 lines)
- `addons/pos_sms/i18n/nb.po` (93 lines)
- `addons/pos_sms/i18n/nl.po` (99 lines)
- `addons/pos_sms/i18n/pl.po` (101 lines)
- `addons/pos_sms/i18n/pos_sms.pot` (85 lines)
- `addons/pos_sms/i18n/pt.po` (100 lines)
- `addons/pos_sms/i18n/pt_BR.po` (100 lines)
- `addons/pos_sms/i18n/ro.po` (99 lines)
- `addons/pos_sms/i18n/ru.po` (100 lines)
- `addons/pos_sms/i18n/sk.po` (91 lines)
- `addons/pos_sms/i18n/sl.po` (94 lines)
- `addons/pos_sms/i18n/sr@latin.po` (93 lines)
- `addons/pos_sms/i18n/sv.po` (100 lines)
- `addons/pos_sms/i18n/th.po` (99 lines)
- `addons/pos_sms/i18n/tr.po` (100 lines)
- `addons/pos_sms/i18n/uk.po` (93 lines)
- `addons/pos_sms/i18n/uz.po` (112 lines)
- `addons/pos_sms/i18n/vi.po` (100 lines)
- `addons/pos_sms/i18n/zh_CN.po` (100 lines)
- `addons/pos_sms/i18n/zh_TW.po` (101 lines)
- `addons/pos_sms/models/__init__.py` (3 lines)
- `addons/pos_sms/models/pos_config.py` (7 lines)
- `addons/pos_sms/models/pos_order.py` (27 lines)
- `addons/pos_sms/models/res_config_settings.py` (7 lines)
- `addons/pos_sms/static/src/app/components/popups/send_receipt_popup/send_receipt_popup.js` (28 lines)
- `addons/pos_sms/static/tests/tours/test_pos_sms_tour.js` (35 lines)
- `addons/pos_sms/static/tests/tours/utils/test_pos_sms_util.js` (11 lines)
- `addons/pos_sms/tests/__init__.py` (1 lines)
- `addons/pos_sms/tests/test_frontend.py` (17 lines)
- `addons/pos_sms/views/res_config_settings_views.xml` (17 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
