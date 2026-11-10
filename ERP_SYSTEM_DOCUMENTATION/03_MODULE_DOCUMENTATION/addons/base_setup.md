# Module: base_setup

- **Module ID:** MOD-042
- **Path:** `addons/base_setup`
- **Manifest:** `addons/base_setup/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This module helps to configure the system at the installation of a new database.
================================================================================

Shows you a list of applications features to install from.

    

Declared dependencies: `base`, `web`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 15 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 3 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base",
    "web"
  ],
  "data": [
    "data/base_setup_data.xml",
    "views/res_config_settings_views.xml",
    "views/res_partner_views.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "base_setup/static/src/views/**/*"
    ]
  }
}
```

### Representative source files

- `addons/base_setup/__init__.py` (4 lines)
- `addons/base_setup/__manifest__.py` (26 lines)
- `addons/base_setup/controllers/__init__.py` (3 lines)
- `addons/base_setup/controllers/kpi.py` (177 lines)
- `addons/base_setup/controllers/main.py` (59 lines)
- `addons/base_setup/data/base_setup_data.xml` (9 lines)
- `addons/base_setup/i18n/af.po` (598 lines)
- `addons/base_setup/i18n/am.po` (594 lines)
- `addons/base_setup/i18n/ar.po` (645 lines)
- `addons/base_setup/i18n/az.po` (625 lines)
- `addons/base_setup/i18n/base_setup.pot` (589 lines)
- `addons/base_setup/i18n/bg.po` (632 lines)
- `addons/base_setup/i18n/bs.po` (600 lines)
- `addons/base_setup/i18n/ca.po` (664 lines)
- `addons/base_setup/i18n/cs.po` (651 lines)
- `addons/base_setup/i18n/da.po` (655 lines)
- `addons/base_setup/i18n/de.po` (667 lines)
- `addons/base_setup/i18n/el.po` (617 lines)
- `addons/base_setup/i18n/es.po` (666 lines)
- `addons/base_setup/i18n/es_419.po` (662 lines)
- `addons/base_setup/i18n/es_CL.po` (30 lines)
- `addons/base_setup/i18n/et.po` (640 lines)
- `addons/base_setup/i18n/eu.po` (597 lines)
- `addons/base_setup/i18n/fa.po` (649 lines)
- `addons/base_setup/i18n/fi.po` (677 lines)
- `addons/base_setup/i18n/fo.po` (597 lines)
- `addons/base_setup/i18n/fr.po` (677 lines)
- `addons/base_setup/i18n/fr_CA.po` (25 lines)
- `addons/base_setup/i18n/gl.po` (597 lines)
- `addons/base_setup/i18n/gu.po` (597 lines)
- `addons/base_setup/i18n/he.po` (638 lines)
- `addons/base_setup/i18n/hi.po` (598 lines)
- `addons/base_setup/i18n/hr.po` (635 lines)
- `addons/base_setup/i18n/hu.po` (625 lines)
- `addons/base_setup/i18n/hy.po` (596 lines)
- `addons/base_setup/i18n/id.po` (658 lines)
- `addons/base_setup/i18n/is.po` (594 lines)
- `addons/base_setup/i18n/it.po` (663 lines)
- `addons/base_setup/i18n/ja.po` (662 lines)
- `addons/base_setup/i18n/ka.po` (597 lines)
- `addons/base_setup/i18n/kab.po` (598 lines)
- `addons/base_setup/i18n/km.po` (597 lines)
- `addons/base_setup/i18n/ko.po` (648 lines)
- `addons/base_setup/i18n/ku.po` (596 lines)
- `addons/base_setup/i18n/lo.po` (640 lines)
- `addons/base_setup/i18n/lt.po` (625 lines)
- `addons/base_setup/i18n/lv.po` (605 lines)
- `addons/base_setup/i18n/mk.po` (597 lines)
- `addons/base_setup/i18n/mn.po` (611 lines)
- `addons/base_setup/i18n/my.po` (596 lines)
- `addons/base_setup/i18n/nb.po` (613 lines)
- `addons/base_setup/i18n/nl.po` (664 lines)
- `addons/base_setup/i18n/pl.po` (671 lines)
- `addons/base_setup/i18n/pt.po` (663 lines)
- `addons/base_setup/i18n/pt_BR.po` (666 lines)
- `addons/base_setup/i18n/ro.po` (659 lines)
- `addons/base_setup/i18n/ru.po` (660 lines)
- `addons/base_setup/i18n/sk.po` (622 lines)
- `addons/base_setup/i18n/sl.po` (657 lines)
- `addons/base_setup/i18n/sq.po` (597 lines)
- `addons/base_setup/i18n/sr@latin.po` (603 lines)
- `addons/base_setup/i18n/sv.po` (664 lines)
- `addons/base_setup/i18n/th.po` (643 lines)
- `addons/base_setup/i18n/tr.po` (667 lines)
- `addons/base_setup/i18n/uk.po` (658 lines)
- `addons/base_setup/i18n/uz.po` (744 lines)
- `addons/base_setup/i18n/vi.po` (650 lines)
- `addons/base_setup/i18n/zh_CN.po` (644 lines)
- `addons/base_setup/i18n/zh_TW.po` (638 lines)
- `addons/base_setup/models/__init__.py` (7 lines)
- `addons/base_setup/models/ir_http.py` (13 lines)
- `addons/base_setup/models/kpi_provider.py` (25 lines)
- `addons/base_setup/models/res_config_settings.py` (133 lines)
- `addons/base_setup/models/res_users.py` (37 lines)
- `addons/base_setup/static/src/img/logo_apple_store.png` (29 lines)
- `addons/base_setup/static/src/img/logo_google_play.png` (52 lines)
- `addons/base_setup/static/src/views/module_views.js` (23 lines)
- `addons/base_setup/static/src/views/module_views.xml` (9 lines)
- `addons/base_setup/tests/__init__.py` (7 lines)
- `addons/base_setup/tests/test_default_group.py` (46 lines)
- `addons/base_setup/tests/test_kpi_controller.py` (225 lines)
- `addons/base_setup/tests/test_res_config.py` (97 lines)
- `addons/base_setup/tests/test_res_config_doc_links.py` (75 lines)
- `addons/base_setup/views/res_config_settings_views.xml` (222 lines)
- `addons/base_setup/views/res_partner_views.xml` (14 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
