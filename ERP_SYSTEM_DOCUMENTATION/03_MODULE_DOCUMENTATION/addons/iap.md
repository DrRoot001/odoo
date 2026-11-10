# Module: iap

- **Module ID:** MOD-108
- **Path:** `addons/iap`
- **Manifest:** `addons/iap/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Basic models and helpers to support In-App Purchase.


This module provides standard tools (account model, context manager and helpers)
to support In-App Purchase inside Odoo. 

Declared dependencies: `web`, `base_setup`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 13 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "web",
    "base_setup"
  ],
  "data": [
    "data/services.xml",
    "views/iap_views.xml",
    "views/res_config_settings.xml",
    "views/res_users_views.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "iap/static/src/**/*.js",
      "iap/static/src/**/*.xml"
    ]
  }
}
```

### Representative source files

- `addons/iap/__init__.py` (9 lines)
- `addons/iap/__manifest__.py` (32 lines)
- `addons/iap/data/neutralize.sql` (9 lines)
- `addons/iap/data/services.xml` (13 lines)
- `addons/iap/i18n/af.po` (379 lines)
- `addons/iap/i18n/am.po` (375 lines)
- `addons/iap/i18n/ar.po` (438 lines)
- `addons/iap/i18n/az.po` (417 lines)
- `addons/iap/i18n/bg.po` (418 lines)
- `addons/iap/i18n/bs.po` (418 lines)
- `addons/iap/i18n/ca.po` (422 lines)
- `addons/iap/i18n/cs.po` (422 lines)
- `addons/iap/i18n/da.po` (419 lines)
- `addons/iap/i18n/de.po` (497 lines)
- `addons/iap/i18n/el.po` (417 lines)
- `addons/iap/i18n/es.po` (435 lines)
- `addons/iap/i18n/es_419.po` (489 lines)
- `addons/iap/i18n/es_CL.po` (69 lines)
- `addons/iap/i18n/et.po` (422 lines)
- `addons/iap/i18n/eu.po` (378 lines)
- `addons/iap/i18n/fa.po` (422 lines)
- `addons/iap/i18n/fi.po` (439 lines)
- `addons/iap/i18n/fo.po` (378 lines)
- `addons/iap/i18n/fr.po` (486 lines)
- `addons/iap/i18n/fr_CA.po` (64 lines)
- `addons/iap/i18n/gl.po` (378 lines)
- `addons/iap/i18n/gu.po` (379 lines)
- `addons/iap/i18n/he.po` (422 lines)
- `addons/iap/i18n/hi.po` (413 lines)
- `addons/iap/i18n/hr.po` (419 lines)
- `addons/iap/i18n/hu.po` (421 lines)
- `addons/iap/i18n/iap.pot` (410 lines)
- `addons/iap/i18n/id.po` (468 lines)
- `addons/iap/i18n/is.po` (375 lines)
- `addons/iap/i18n/it.po` (490 lines)
- `addons/iap/i18n/ja.po` (475 lines)
- `addons/iap/i18n/ka.po` (378 lines)
- `addons/iap/i18n/kab.po` (415 lines)
- `addons/iap/i18n/km.po` (378 lines)
- `addons/iap/i18n/ko.po` (449 lines)
- `addons/iap/i18n/ku.po` (413 lines)
- `addons/iap/i18n/lo.po` (424 lines)
- `addons/iap/i18n/lt.po` (423 lines)
- `addons/iap/i18n/lv.po` (419 lines)
- `addons/iap/i18n/mk.po` (378 lines)
- `addons/iap/i18n/mn.po` (419 lines)
- `addons/iap/i18n/my.po` (414 lines)
- `addons/iap/i18n/nb.po` (419 lines)
- `addons/iap/i18n/nl.po` (490 lines)
- `addons/iap/i18n/pl.po` (444 lines)
- `addons/iap/i18n/pt.po` (424 lines)
- `addons/iap/i18n/pt_BR.po` (496 lines)
- `addons/iap/i18n/ro.po` (436 lines)
- `addons/iap/i18n/ru.po` (435 lines)
- `addons/iap/i18n/sk.po` (418 lines)
- `addons/iap/i18n/sl.po` (442 lines)
- `addons/iap/i18n/sq.po` (378 lines)
- `addons/iap/i18n/sr@latin.po` (419 lines)
- `addons/iap/i18n/sv.po` (432 lines)
- `addons/iap/i18n/th.po` (427 lines)
- `addons/iap/i18n/tr.po` (455 lines)
- `addons/iap/i18n/uk.po` (420 lines)
- `addons/iap/i18n/uz.po` (477 lines)
- `addons/iap/i18n/vi.po` (445 lines)
- `addons/iap/i18n/zh_CN.po` (431 lines)
- `addons/iap/i18n/zh_TW.po` (425 lines)
- `addons/iap/models/__init__.py` (7 lines)
- `addons/iap/models/iap_account.py` (384 lines)
- `addons/iap/models/iap_enrich_api.py` (39 lines)
- `addons/iap/models/iap_service.py` (21 lines)
- `addons/iap/models/iap_service_pack.py` (23 lines)
- `addons/iap/models/res_config_settings.py` (8 lines)
- `addons/iap/security/ir.access.csv` (6 lines)
- `addons/iap/static/description/icon.png` (6 lines)
- `addons/iap/static/description/icon.svg` (1 lines)
- `addons/iap/static/description/icon_hi.png` (19 lines)
- `addons/iap/static/src/action_buttons_widget/action_buttons_widget.js` (46 lines)
- `addons/iap/static/src/action_buttons_widget/action_buttons_widget.xml` (13 lines)
- `addons/iap/tests/__init__.py` (5 lines)
- `addons/iap/tests/common.py` (176 lines)
- `addons/iap/tests/test_iap.py` (33 lines)
- `addons/iap/tools/__init__.py` (4 lines)
- `addons/iap/tools/iap_tools.py` (164 lines)
- `addons/iap/views/iap_views.xml` (104 lines)
- `addons/iap/views/res_config_settings.xml` (19 lines)
- `addons/iap/views/res_users_views.xml` (16 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
