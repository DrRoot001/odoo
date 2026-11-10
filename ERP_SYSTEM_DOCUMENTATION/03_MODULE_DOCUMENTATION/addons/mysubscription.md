# Module: mysubscription

- **Module ID:** MOD-388
- **Path:** `addons/mysubscription`
- **Manifest:** `addons/mysubscription/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Backend Subscription App

No manifest description declared.

Declared dependencies: `base`, `web`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 11 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 11 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base",
    "web"
  ],
  "data": [
    "data/ir_config_parameter_data.xml",
    "views/menus.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "mysubscription/static/src/**/*.js",
      "mysubscription/static/src/**/*.xml",
      "mysubscription/static/src/**/*.scss"
    ],
    "web.assets_unit_tests": [
      "mysubscription/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/mysubscription/__init__.py` (1 lines)
- `addons/mysubscription/__manifest__.py` (23 lines)
- `addons/mysubscription/data/ir_config_parameter_data.xml` (7 lines)
- `addons/mysubscription/i18n/ar.po` (394 lines)
- `addons/mysubscription/i18n/az.po` (394 lines)
- `addons/mysubscription/i18n/bg.po` (394 lines)
- `addons/mysubscription/i18n/bs.po` (394 lines)
- `addons/mysubscription/i18n/ca.po` (394 lines)
- `addons/mysubscription/i18n/cs.po` (394 lines)
- `addons/mysubscription/i18n/da.po` (394 lines)
- `addons/mysubscription/i18n/de.po` (408 lines)
- `addons/mysubscription/i18n/el.po` (394 lines)
- `addons/mysubscription/i18n/es.po` (398 lines)
- `addons/mysubscription/i18n/es_419.po` (398 lines)
- `addons/mysubscription/i18n/et.po` (394 lines)
- `addons/mysubscription/i18n/fa.po` (394 lines)
- `addons/mysubscription/i18n/fi.po` (398 lines)
- `addons/mysubscription/i18n/fr.po` (394 lines)
- `addons/mysubscription/i18n/he.po` (394 lines)
- `addons/mysubscription/i18n/hi.po` (394 lines)
- `addons/mysubscription/i18n/hr.po` (394 lines)
- `addons/mysubscription/i18n/hu.po` (394 lines)
- `addons/mysubscription/i18n/id.po` (394 lines)
- `addons/mysubscription/i18n/it.po` (398 lines)
- `addons/mysubscription/i18n/ja.po` (398 lines)
- `addons/mysubscription/i18n/kab.po` (394 lines)
- `addons/mysubscription/i18n/ko.po` (394 lines)
- `addons/mysubscription/i18n/ku.po` (394 lines)
- `addons/mysubscription/i18n/lo.po` (401 lines)
- `addons/mysubscription/i18n/lt.po` (394 lines)
- `addons/mysubscription/i18n/lv.po` (394 lines)
- `addons/mysubscription/i18n/mn.po` (394 lines)
- `addons/mysubscription/i18n/my.po` (394 lines)
- `addons/mysubscription/i18n/mysubscription.pot` (394 lines)
- `addons/mysubscription/i18n/nb.po` (394 lines)
- `addons/mysubscription/i18n/nl.po` (405 lines)
- `addons/mysubscription/i18n/pl.po` (394 lines)
- `addons/mysubscription/i18n/pt.po` (394 lines)
- `addons/mysubscription/i18n/pt_BR.po` (408 lines)
- `addons/mysubscription/i18n/ro.po` (394 lines)
- `addons/mysubscription/i18n/ru.po` (394 lines)
- `addons/mysubscription/i18n/sk.po` (394 lines)
- `addons/mysubscription/i18n/sl.po` (394 lines)
- `addons/mysubscription/i18n/sr@latin.po` (394 lines)
- `addons/mysubscription/i18n/sv.po` (398 lines)
- `addons/mysubscription/i18n/th.po` (394 lines)
- `addons/mysubscription/i18n/tr.po` (394 lines)
- `addons/mysubscription/i18n/uk.po` (394 lines)
- `addons/mysubscription/i18n/uz.po` (394 lines)
- `addons/mysubscription/i18n/vi.po` (394 lines)
- `addons/mysubscription/i18n/zh_CN.po` (399 lines)
- `addons/mysubscription/i18n/zh_TW.po` (394 lines)
- `addons/mysubscription/models/__init__.py` (1 lines)
- `addons/mysubscription/models/mysubscription.py` (56 lines)
- `addons/mysubscription/static/src/components/dashboard_block.js` (9 lines)
- `addons/mysubscription/static/src/components/dashboard_block.xml` (18 lines)
- `addons/mysubscription/static/src/components/database_dialog.js` (140 lines)
- `addons/mysubscription/static/src/components/database_dialog.xml` (70 lines)
- `addons/mysubscription/static/src/components/navbar.js` (37 lines)
- `addons/mysubscription/static/src/components/navbar.xml` (32 lines)
- `addons/mysubscription/static/src/components/plan_box.js` (41 lines)
- `addons/mysubscription/static/src/components/plan_box.xml` (58 lines)
- `addons/mysubscription/static/src/components/subscription_dialog.js` (36 lines)
- `addons/mysubscription/static/src/components/subscription_dialog.xml` (16 lines)
- `addons/mysubscription/static/src/dashboard.js` (53 lines)
- `addons/mysubscription/static/src/dashboard.scss` (32 lines)
- `addons/mysubscription/static/src/dashboard.xml` (24 lines)
- `addons/mysubscription/static/src/database_section.js` (74 lines)
- `addons/mysubscription/static/src/database_section.xml` (101 lines)
- `addons/mysubscription/static/src/iap_section.js` (76 lines)
- `addons/mysubscription/static/src/iap_section.xml` (56 lines)
- `addons/mysubscription/static/src/img/default_iap_icon.png` (10 lines)
- `addons/mysubscription/static/src/img/invoice_ocr_icon.png` (20 lines)
- `addons/mysubscription/static/src/img/odoo_o.svg` (3 lines)
- `addons/mysubscription/static/src/img/partner_autocomplete_icon.png` (18 lines)
- `addons/mysubscription/static/src/img/phone_service_icon.png` (31 lines)
- `addons/mysubscription/static/src/img/reveal_icon.png` (11 lines)
- `addons/mysubscription/static/src/img/sms_icon.png` (12 lines)
- `addons/mysubscription/static/src/img/snailmail_icon.png` (16 lines)
- `addons/mysubscription/static/src/plan_section.js` (98 lines)
- `addons/mysubscription/static/src/plan_section.xml` (33 lines)
- `addons/mysubscription/static/src/user_menu.js` (19 lines)
- `addons/mysubscription/static/tests/mysubscription.test.js` (144 lines)
- `addons/mysubscription/tests/__init__.py` (1 lines)
- `addons/mysubscription/tests/test_mysubscription.py` (17 lines)
- `addons/mysubscription/views/menus.xml` (7 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
