# Module: uom

- **Module ID:** MOD-590
- **Path:** `addons/uom`
- **Manifest:** `addons/uom/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the base module for managing Units of measure.
========================================================================
    

Declared dependencies: `base`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base"
  ],
  "data": [
    "data/uom_data.xml",
    "security/uom_security.xml",
    "views/uom_uom_views.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "uom/static/src/components/**/*"
    ]
  }
}
```

### Representative source files

- `addons/uom/__init__.py` (4 lines)
- `addons/uom/__manifest__.py` (24 lines)
- `addons/uom/data/uom_data.xml` (192 lines)
- `addons/uom/i18n/ar.po` (388 lines)
- `addons/uom/i18n/az.po` (377 lines)
- `addons/uom/i18n/bg.po` (377 lines)
- `addons/uom/i18n/bs.po` (379 lines)
- `addons/uom/i18n/ca.po` (390 lines)
- `addons/uom/i18n/cs.po` (387 lines)
- `addons/uom/i18n/da.po` (380 lines)
- `addons/uom/i18n/de.po` (396 lines)
- `addons/uom/i18n/el.po` (382 lines)
- `addons/uom/i18n/es.po` (396 lines)
- `addons/uom/i18n/es_419.po` (389 lines)
- `addons/uom/i18n/et.po` (398 lines)
- `addons/uom/i18n/fa.po` (386 lines)
- `addons/uom/i18n/fi.po` (401 lines)
- `addons/uom/i18n/fr.po` (394 lines)
- `addons/uom/i18n/gu.po` (367 lines)
- `addons/uom/i18n/he.po` (386 lines)
- `addons/uom/i18n/hi.po` (375 lines)
- `addons/uom/i18n/hr.po` (387 lines)
- `addons/uom/i18n/hu.po` (386 lines)
- `addons/uom/i18n/id.po` (391 lines)
- `addons/uom/i18n/is.po` (363 lines)
- `addons/uom/i18n/it.po` (396 lines)
- `addons/uom/i18n/ja.po` (389 lines)
- `addons/uom/i18n/kab.po` (374 lines)
- `addons/uom/i18n/km.po` (367 lines)
- `addons/uom/i18n/ko.po` (388 lines)
- `addons/uom/i18n/ku.po` (374 lines)
- `addons/uom/i18n/lo.po` (385 lines)
- `addons/uom/i18n/lt.po` (389 lines)
- `addons/uom/i18n/lv.po` (374 lines)
- `addons/uom/i18n/mn.po` (398 lines)
- `addons/uom/i18n/my.po` (376 lines)
- `addons/uom/i18n/nb.po` (380 lines)
- `addons/uom/i18n/nl.po` (398 lines)
- `addons/uom/i18n/pl.po` (407 lines)
- `addons/uom/i18n/pt.po` (391 lines)
- `addons/uom/i18n/pt_BR.po` (397 lines)
- `addons/uom/i18n/ro.po` (396 lines)
- `addons/uom/i18n/ru.po` (394 lines)
- `addons/uom/i18n/sk.po` (385 lines)
- `addons/uom/i18n/sl.po` (379 lines)
- `addons/uom/i18n/sr@latin.po` (380 lines)
- `addons/uom/i18n/sv.po` (389 lines)
- `addons/uom/i18n/th.po` (393 lines)
- `addons/uom/i18n/tr.po` (400 lines)
- `addons/uom/i18n/uk.po` (386 lines)
- `addons/uom/i18n/uom.pot` (367 lines)
- `addons/uom/i18n/uz.po` (452 lines)
- `addons/uom/i18n/vi.po` (389 lines)
- `addons/uom/i18n/zh_CN.po` (390 lines)
- `addons/uom/i18n/zh_TW.po` (386 lines)
- `addons/uom/models/__init__.py` (6 lines)
- `addons/uom/models/res_groups.py` (13 lines)
- `addons/uom/models/uom_uom.py` (220 lines)
- `addons/uom/security/ir.access.csv` (3 lines)
- `addons/uom/security/uom_security.xml` (8 lines)
- `addons/uom/static/src/components/many2one_uom/many2one_uom_field.js` (118 lines)
- `addons/uom/static/src/components/many2one_uom/many2one_uom_field.scss` (5 lines)
- `addons/uom/static/src/components/many2one_uom/many2one_uom_field.xml` (20 lines)
- `addons/uom/static/src/components/many2x_uom_tags/many2x_uom_tags.js` (136 lines)
- `addons/uom/static/src/components/many2x_uom_tags/many2x_uom_tags.xml` (21 lines)
- `addons/uom/tests/__init__.py` (4 lines)
- `addons/uom/tests/common.py` (33 lines)
- `addons/uom/tests/test_uom.py` (59 lines)
- `addons/uom/views/uom_uom_views.xml` (62 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
