# Module: sale_service

- **Module ID:** MOD-531
- **Path:** `addons/sale_service`
- **Manifest:** `addons/sale_service/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Interaction between Sales and services apps (project and planning)


Allows to display sale information in the SOL services apps
===========================================================
Additional information is displayed in the name of the SOL when it is used in services apps (project and planning).


Declared dependencies: `sale_management`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sale_management"
  ],
  "assets": {
    "web.assets_backend": [
      "sale_service/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/sale_service/__init__.py` (4 lines)
- `addons/sale_service/__manifest__.py` (19 lines)
- `addons/sale_service/i18n/ar.po` (63 lines)
- `addons/sale_service/i18n/az.po` (64 lines)
- `addons/sale_service/i18n/bg.po` (64 lines)
- `addons/sale_service/i18n/bs.po` (66 lines)
- `addons/sale_service/i18n/ca.po` (64 lines)
- `addons/sale_service/i18n/cs.po` (64 lines)
- `addons/sale_service/i18n/da.po` (63 lines)
- `addons/sale_service/i18n/de.po` (70 lines)
- `addons/sale_service/i18n/el.po` (64 lines)
- `addons/sale_service/i18n/es.po` (65 lines)
- `addons/sale_service/i18n/es_419.po` (62 lines)
- `addons/sale_service/i18n/et.po` (64 lines)
- `addons/sale_service/i18n/fa.po` (64 lines)
- `addons/sale_service/i18n/fi.po` (68 lines)
- `addons/sale_service/i18n/fr.po` (63 lines)
- `addons/sale_service/i18n/he.po` (65 lines)
- `addons/sale_service/i18n/hi.po` (64 lines)
- `addons/sale_service/i18n/hr.po` (65 lines)
- `addons/sale_service/i18n/hu.po` (64 lines)
- `addons/sale_service/i18n/id.po` (62 lines)
- `addons/sale_service/i18n/it.po` (68 lines)
- `addons/sale_service/i18n/ja.po` (62 lines)
- `addons/sale_service/i18n/kab.po` (65 lines)
- `addons/sale_service/i18n/ko.po` (62 lines)
- `addons/sale_service/i18n/ku.po` (62 lines)
- `addons/sale_service/i18n/lo.po` (64 lines)
- `addons/sale_service/i18n/lt.po` (66 lines)
- `addons/sale_service/i18n/lv.po` (65 lines)
- `addons/sale_service/i18n/mn.po` (64 lines)
- `addons/sale_service/i18n/my.po` (64 lines)
- `addons/sale_service/i18n/nb.po` (64 lines)
- `addons/sale_service/i18n/nl.po` (69 lines)
- `addons/sale_service/i18n/pl.po` (63 lines)
- `addons/sale_service/i18n/pt.po` (64 lines)
- `addons/sale_service/i18n/pt_BR.po` (70 lines)
- `addons/sale_service/i18n/ro.po` (62 lines)
- `addons/sale_service/i18n/ru.po` (65 lines)
- `addons/sale_service/i18n/sale_service.pot` (56 lines)
- `addons/sale_service/i18n/sk.po` (64 lines)
- `addons/sale_service/i18n/sl.po` (65 lines)
- `addons/sale_service/i18n/sr@latin.po` (65 lines)
- `addons/sale_service/i18n/sv.po` (62 lines)
- `addons/sale_service/i18n/th.po` (62 lines)
- `addons/sale_service/i18n/tr.po` (68 lines)
- `addons/sale_service/i18n/uk.po` (65 lines)
- `addons/sale_service/i18n/uz.po` (71 lines)
- `addons/sale_service/i18n/vi.po` (64 lines)
- `addons/sale_service/i18n/zh_CN.po` (67 lines)
- `addons/sale_service/i18n/zh_TW.po` (64 lines)
- `addons/sale_service/models/__init__.py` (4 lines)
- `addons/sale_service/models/sale_order_line.py` (89 lines)
- `addons/sale_service/static/src/components/so_line_create_button/so_line_create_button.js` (52 lines)
- `addons/sale_service/static/src/components/so_line_create_button/so_line_create_button.scss` (8 lines)
- `addons/sale_service/static/src/components/so_line_create_button/so_line_create_button.xml` (20 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
