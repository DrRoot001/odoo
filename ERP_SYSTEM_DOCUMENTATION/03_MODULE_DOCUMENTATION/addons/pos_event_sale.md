# Module: pos_event_sale

- **Module ID:** MOD-431
- **Path:** `addons/pos_event_sale`
- **Manifest:** `addons/pos_event_sale/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Link module between pos_sale and pos_event

No manifest description declared.

Declared dependencies: `pos_event`, `pos_sale`, `event_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "pos_event",
    "pos_sale",
    "event_sale"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "pos_event_sale/static/src/**/*"
    ],
    "web.assets_tests": [
      "pos_event_sale/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_event_sale/__init__.py` (3 lines)
- `addons/pos_event_sale/__manifest__.py` (19 lines)
- `addons/pos_event_sale/i18n/ar.po` (67 lines)
- `addons/pos_event_sale/i18n/az.po` (68 lines)
- `addons/pos_event_sale/i18n/bg.po` (69 lines)
- `addons/pos_event_sale/i18n/bs.po` (70 lines)
- `addons/pos_event_sale/i18n/ca.po` (69 lines)
- `addons/pos_event_sale/i18n/cs.po` (67 lines)
- `addons/pos_event_sale/i18n/da.po` (68 lines)
- `addons/pos_event_sale/i18n/de.po` (66 lines)
- `addons/pos_event_sale/i18n/el.po` (68 lines)
- `addons/pos_event_sale/i18n/es.po` (67 lines)
- `addons/pos_event_sale/i18n/es_419.po` (66 lines)
- `addons/pos_event_sale/i18n/et.po` (69 lines)
- `addons/pos_event_sale/i18n/fa.po` (69 lines)
- `addons/pos_event_sale/i18n/fi.po` (65 lines)
- `addons/pos_event_sale/i18n/fr.po` (66 lines)
- `addons/pos_event_sale/i18n/he.po` (70 lines)
- `addons/pos_event_sale/i18n/hi.po` (69 lines)
- `addons/pos_event_sale/i18n/hr.po` (69 lines)
- `addons/pos_event_sale/i18n/hu.po` (69 lines)
- `addons/pos_event_sale/i18n/id.po` (66 lines)
- `addons/pos_event_sale/i18n/it.po` (65 lines)
- `addons/pos_event_sale/i18n/ja.po` (65 lines)
- `addons/pos_event_sale/i18n/kab.po` (68 lines)
- `addons/pos_event_sale/i18n/ko.po` (67 lines)
- `addons/pos_event_sale/i18n/ku.po` (66 lines)
- `addons/pos_event_sale/i18n/lo.po` (69 lines)
- `addons/pos_event_sale/i18n/lt.po` (71 lines)
- `addons/pos_event_sale/i18n/lv.po` (70 lines)
- `addons/pos_event_sale/i18n/mn.po` (68 lines)
- `addons/pos_event_sale/i18n/my.po` (67 lines)
- `addons/pos_event_sale/i18n/nb.po` (68 lines)
- `addons/pos_event_sale/i18n/nl.po` (67 lines)
- `addons/pos_event_sale/i18n/pl.po` (68 lines)
- `addons/pos_event_sale/i18n/pos_event_sale.pot` (61 lines)
- `addons/pos_event_sale/i18n/pt.po` (69 lines)
- `addons/pos_event_sale/i18n/pt_BR.po` (71 lines)
- `addons/pos_event_sale/i18n/ro.po` (68 lines)
- `addons/pos_event_sale/i18n/ru.po` (68 lines)
- `addons/pos_event_sale/i18n/sk.po` (68 lines)
- `addons/pos_event_sale/i18n/sl.po` (70 lines)
- `addons/pos_event_sale/i18n/sr@latin.po` (70 lines)
- `addons/pos_event_sale/i18n/sv.po` (67 lines)
- `addons/pos_event_sale/i18n/th.po` (67 lines)
- `addons/pos_event_sale/i18n/tr.po` (66 lines)
- `addons/pos_event_sale/i18n/uk.po` (70 lines)
- `addons/pos_event_sale/i18n/uz.po` (75 lines)
- `addons/pos_event_sale/i18n/vi.po` (69 lines)
- `addons/pos_event_sale/i18n/zh_CN.po` (66 lines)
- `addons/pos_event_sale/i18n/zh_TW.po` (65 lines)
- `addons/pos_event_sale/models/__init__.py` (3 lines)
- `addons/pos_event_sale/models/event_registration.py` (26 lines)
- `addons/pos_event_sale/models/sale_order_line.py` (10 lines)
- `addons/pos_event_sale/report/__init__.py` (3 lines)
- `addons/pos_event_sale/report/event_sale_report.py` (83 lines)
- `addons/pos_event_sale/static/src/app/services/pos_store.js` (87 lines)
- `addons/pos_event_sale/static/tests/tours/pos_event_sale_tour.js` (50 lines)
- `addons/pos_event_sale/tests/__init__.py` (3 lines)
- `addons/pos_event_sale/tests/test_frontend.py` (179 lines)
- `addons/pos_event_sale/tests/test_sale_report.py` (72 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
