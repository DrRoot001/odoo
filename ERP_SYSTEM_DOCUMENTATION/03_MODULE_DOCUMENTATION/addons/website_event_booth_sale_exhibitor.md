# Module: website_event_booth_sale_exhibitor

- **Module ID:** MOD-610
- **Path:** `addons/website_event_booth_sale_exhibitor`
- **Manifest:** `addons/website_event_booth_sale_exhibitor/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Bridge module between website_event_booth_exhibitor and website_event_booth_sale.

No manifest description declared.

Declared dependencies: `website_event_exhibitor`, `website_event_booth_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website_event_exhibitor",
    "website_event_booth_sale"
  ],
  "assets": {
    "web.assets_tests": [
      "website_event_booth_sale_exhibitor/static/tests/tours/website_event_booth_sale_exhibitor.js"
    ]
  }
}
```

### Representative source files

- `addons/website_event_booth_sale_exhibitor/__init__.py` (4 lines)
- `addons/website_event_booth_sale_exhibitor/__manifest__.py` (15 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/ar.po` (78 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/az.po` (76 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/bg.po` (76 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/bs.po` (78 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/ca.po` (77 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/cs.po` (77 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/da.po` (78 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/de.po` (80 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/el.po` (76 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/es.po` (80 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/es_419.po` (77 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/et.po` (76 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/fa.po` (76 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/fi.po` (77 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/fr.po` (77 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/he.po` (77 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/hi.po` (76 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/hr.po` (77 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/hu.po` (77 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/id.po` (77 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/it.po` (80 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/ja.po` (77 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/kab.po` (77 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/ko.po` (77 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/ku.po` (76 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/lo.po` (76 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/lt.po` (78 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/lv.po` (77 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/mn.po` (76 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/my.po` (76 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/nb.po` (77 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/nl.po` (77 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/pl.po` (78 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/pt.po` (78 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/pt_BR.po` (81 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/ro.po` (78 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/ru.po` (80 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/sk.po` (76 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/sl.po` (78 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/sr@latin.po` (77 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/sv.po` (80 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/th.po` (77 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/tr.po` (77 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/uk.po` (77 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/uz.po` (93 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/vi.po` (77 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/website_event_booth_sale_exhibitor.pot` (73 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/zh_CN.po` (77 lines)
- `addons/website_event_booth_sale_exhibitor/i18n/zh_TW.po` (80 lines)
- `addons/website_event_booth_sale_exhibitor/models/__init__.py` (4 lines)
- `addons/website_event_booth_sale_exhibitor/models/event_booth_registration.py` (20 lines)
- `addons/website_event_booth_sale_exhibitor/static/tests/tours/website_event_booth_sale_exhibitor.js` (20 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
