# Module: data_recycle

- **Module ID:** MOD-061
- **Path:** `addons/data_recycle`
- **Manifest:** `addons/data_recycle/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Find old records and archive/delete them

Find old records and archive/delete them

Declared dependencies: `mail`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 3 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mail"
  ],
  "data": [
    "data/ir_cron_data.xml",
    "views/data_recycle_model_views.xml",
    "views/data_recycle_record_views.xml",
    "views/data_cleaning_menu.xml",
    "views/data_recycle_templates.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "data_recycle/static/src/cog_menu/data_refresh_cog_menu.js",
      "data_recycle/static/src/cog_menu/data_refresh_cog_menu.xml",
      "data_recycle/static/src/views/*.js"
    ]
  }
}
```

### Representative source files

- `addons/data_recycle/__init__.py` (4 lines)
- `addons/data_recycle/__manifest__.py` (28 lines)
- `addons/data_recycle/data/ir_cron_data.xml` (13 lines)
- `addons/data_recycle/i18n/ar.po` (411 lines)
- `addons/data_recycle/i18n/az.po` (403 lines)
- `addons/data_recycle/i18n/bg.po` (403 lines)
- `addons/data_recycle/i18n/bs.po` (405 lines)
- `addons/data_recycle/i18n/ca.po` (409 lines)
- `addons/data_recycle/i18n/cs.po` (406 lines)
- `addons/data_recycle/i18n/da.po` (410 lines)
- `addons/data_recycle/i18n/data_recycle.pot` (396 lines)
- `addons/data_recycle/i18n/de.po` (415 lines)
- `addons/data_recycle/i18n/el.po` (403 lines)
- `addons/data_recycle/i18n/es.po` (411 lines)
- `addons/data_recycle/i18n/es_419.po` (410 lines)
- `addons/data_recycle/i18n/et.po` (410 lines)
- `addons/data_recycle/i18n/fa.po` (407 lines)
- `addons/data_recycle/i18n/fi.po` (413 lines)
- `addons/data_recycle/i18n/fr.po` (414 lines)
- `addons/data_recycle/i18n/he.po` (409 lines)
- `addons/data_recycle/i18n/hi.po` (408 lines)
- `addons/data_recycle/i18n/hr.po` (407 lines)
- `addons/data_recycle/i18n/hu.po` (403 lines)
- `addons/data_recycle/i18n/id.po` (413 lines)
- `addons/data_recycle/i18n/it.po` (413 lines)
- `addons/data_recycle/i18n/ja.po` (409 lines)
- `addons/data_recycle/i18n/kab.po` (404 lines)
- `addons/data_recycle/i18n/ko.po` (409 lines)
- `addons/data_recycle/i18n/ku.po` (403 lines)
- `addons/data_recycle/i18n/lo.po` (402 lines)
- `addons/data_recycle/i18n/lt.po` (408 lines)
- `addons/data_recycle/i18n/lv.po` (405 lines)
- `addons/data_recycle/i18n/mn.po` (406 lines)
- `addons/data_recycle/i18n/my.po` (404 lines)
- `addons/data_recycle/i18n/nb.po` (403 lines)
- `addons/data_recycle/i18n/nl.po` (416 lines)
- `addons/data_recycle/i18n/pl.po` (412 lines)
- `addons/data_recycle/i18n/pt.po` (411 lines)
- `addons/data_recycle/i18n/pt_BR.po` (414 lines)
- `addons/data_recycle/i18n/ro.po` (411 lines)
- `addons/data_recycle/i18n/ru.po` (413 lines)
- `addons/data_recycle/i18n/sk.po` (404 lines)
- `addons/data_recycle/i18n/sl.po` (413 lines)
- `addons/data_recycle/i18n/sr@latin.po` (405 lines)
- `addons/data_recycle/i18n/sv.po` (412 lines)
- `addons/data_recycle/i18n/th.po` (408 lines)
- `addons/data_recycle/i18n/tr.po` (413 lines)
- `addons/data_recycle/i18n/uk.po` (410 lines)
- `addons/data_recycle/i18n/uz.po` (482 lines)
- `addons/data_recycle/i18n/vi.po` (408 lines)
- `addons/data_recycle/i18n/zh_CN.po` (409 lines)
- `addons/data_recycle/i18n/zh_TW.po` (411 lines)
- `addons/data_recycle/models/__init__.py` (5 lines)
- `addons/data_recycle/models/data_recycle_model.py` (260 lines)
- `addons/data_recycle/models/data_recycle_record.py` (90 lines)
- `addons/data_recycle/security/ir.access.csv` (3 lines)
- `addons/data_recycle/static/description/icon.png` (17 lines)
- `addons/data_recycle/static/description/icon.svg` (1 lines)
- `addons/data_recycle/static/description/icon_hi.png` (35 lines)
- `addons/data_recycle/static/src/cog_menu/data_refresh_cog_menu.js` (46 lines)
- `addons/data_recycle/static/src/cog_menu/data_refresh_cog_menu.xml` (9 lines)
- `addons/data_recycle/static/src/views/data_cleaning_common_list.js` (37 lines)
- `addons/data_recycle/static/src/views/data_recycle_list_view.js` (35 lines)
- `addons/data_recycle/tests/__init__.py` (4 lines)
- `addons/data_recycle/tests/test_data_recycle.py` (97 lines)
- `addons/data_recycle/views/data_cleaning_menu.xml` (34 lines)
- `addons/data_recycle/views/data_recycle_model_views.xml` (86 lines)
- `addons/data_recycle/views/data_recycle_record_views.xml` (72 lines)
- `addons/data_recycle/views/data_recycle_templates.xml` (7 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
