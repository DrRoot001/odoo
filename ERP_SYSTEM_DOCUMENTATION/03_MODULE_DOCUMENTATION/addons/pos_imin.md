# Module: pos_imin

- **Module ID:** MOD-435
- **Path:** `addons/pos_imin`
- **Manifest:** `addons/pos_imin/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

iMin ePOS Printers in PoS



Use iMin ePOS Printers without the IoT Box in the Point of Sale


Declared dependencies: `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
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
    "views/pos_printer_views.xml"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "pos_imin/static/lib/**/*",
      "pos_imin/static/src/**/*",
      [
        "remove",
        "pos_imin/static/src/backend/**/*"
      ]
    ],
    "web.assets_backend": [
      "pos_imin/static/lib/**/*",
      "pos_imin/static/src/backend/test_imin/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_imin/__init__.py` (2 lines)
- `addons/pos_imin/__manifest__.py` (28 lines)
- `addons/pos_imin/i18n/ar.po` (113 lines)
- `addons/pos_imin/i18n/az.po` (111 lines)
- `addons/pos_imin/i18n/bg.po` (111 lines)
- `addons/pos_imin/i18n/bs.po` (112 lines)
- `addons/pos_imin/i18n/ca.po` (111 lines)
- `addons/pos_imin/i18n/cs.po` (112 lines)
- `addons/pos_imin/i18n/da.po` (111 lines)
- `addons/pos_imin/i18n/de.po` (115 lines)
- `addons/pos_imin/i18n/el.po` (111 lines)
- `addons/pos_imin/i18n/es.po` (117 lines)
- `addons/pos_imin/i18n/es_419.po` (112 lines)
- `addons/pos_imin/i18n/et.po` (111 lines)
- `addons/pos_imin/i18n/fa.po` (111 lines)
- `addons/pos_imin/i18n/fi.po` (112 lines)
- `addons/pos_imin/i18n/fr.po` (115 lines)
- `addons/pos_imin/i18n/he.po` (112 lines)
- `addons/pos_imin/i18n/hi.po` (111 lines)
- `addons/pos_imin/i18n/hr.po` (112 lines)
- `addons/pos_imin/i18n/hu.po` (111 lines)
- `addons/pos_imin/i18n/id.po` (112 lines)
- `addons/pos_imin/i18n/it.po` (116 lines)
- `addons/pos_imin/i18n/ja.po` (112 lines)
- `addons/pos_imin/i18n/kab.po` (111 lines)
- `addons/pos_imin/i18n/ko.po` (112 lines)
- `addons/pos_imin/i18n/ku.po` (111 lines)
- `addons/pos_imin/i18n/lo.po` (110 lines)
- `addons/pos_imin/i18n/lt.po` (113 lines)
- `addons/pos_imin/i18n/lv.po` (111 lines)
- `addons/pos_imin/i18n/mn.po` (111 lines)
- `addons/pos_imin/i18n/my.po` (111 lines)
- `addons/pos_imin/i18n/nb.po` (111 lines)
- `addons/pos_imin/i18n/nl.po` (112 lines)
- `addons/pos_imin/i18n/pl.po` (113 lines)
- `addons/pos_imin/i18n/pos_imin.pot` (107 lines)
- `addons/pos_imin/i18n/pt.po` (111 lines)
- `addons/pos_imin/i18n/pt_BR.po` (116 lines)
- `addons/pos_imin/i18n/ro.po` (113 lines)
- `addons/pos_imin/i18n/ru.po` (113 lines)
- `addons/pos_imin/i18n/sk.po` (110 lines)
- `addons/pos_imin/i18n/sl.po` (112 lines)
- `addons/pos_imin/i18n/sr@latin.po` (112 lines)
- `addons/pos_imin/i18n/sv.po` (112 lines)
- `addons/pos_imin/i18n/th.po` (112 lines)
- `addons/pos_imin/i18n/tr.po` (114 lines)
- `addons/pos_imin/i18n/uk.po` (112 lines)
- `addons/pos_imin/i18n/uz.po` (126 lines)
- `addons/pos_imin/i18n/vi.po` (112 lines)
- `addons/pos_imin/i18n/zh_CN.po` (116 lines)
- `addons/pos_imin/i18n/zh_TW.po` (111 lines)
- `addons/pos_imin/models/__init__.py` (2 lines)
- `addons/pos_imin/models/pos_printer.py` (18 lines)
- `addons/pos_imin/static/lib/imin-printer/imin-printer.js` (982 lines)
- `addons/pos_imin/static/src/app/plugins/pos_ticket_printer_plugin.js` (34 lines)
- `addons/pos_imin/static/src/app/utils/imin_printer.js` (155 lines)
- `addons/pos_imin/static/src/backend/test_imin/test_imin.js` (48 lines)
- `addons/pos_imin/views/pos_printer_views.xml` (30 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
