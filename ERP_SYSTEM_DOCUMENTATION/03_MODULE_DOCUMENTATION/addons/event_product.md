# Module: event_product

- **Module ID:** MOD-069
- **Path:** `addons/event_product`
- **Manifest:** `addons/event_product/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

No manifest description declared.

Declared dependencies: `event`, `product`, `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 7 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "event",
    "product",
    "account"
  ],
  "data": [
    "views/event_ticket_views.xml",
    "views/event_registration_views.xml",
    "data/event_product_data.xml"
  ],
  "demo": [
    "data/event_product_demo.xml",
    "data/event_demo.xml"
  ],
  "assets": {}
}
```

### Representative source files

- `addons/event_product/__init__.py` (1 lines)
- `addons/event_product/__manifest__.py` (18 lines)
- `addons/event_product/data/event_demo.xml` (38 lines)
- `addons/event_product/data/event_product_data.xml` (20 lines)
- `addons/event_product/data/event_product_demo.xml` (25 lines)
- `addons/event_product/i18n/ar.po` (226 lines)
- `addons/event_product/i18n/az.po` (224 lines)
- `addons/event_product/i18n/bg.po` (224 lines)
- `addons/event_product/i18n/bs.po` (221 lines)
- `addons/event_product/i18n/ca.po` (225 lines)
- `addons/event_product/i18n/cs.po` (225 lines)
- `addons/event_product/i18n/da.po` (226 lines)
- `addons/event_product/i18n/de.po` (230 lines)
- `addons/event_product/i18n/el.po` (225 lines)
- `addons/event_product/i18n/es.po` (227 lines)
- `addons/event_product/i18n/es_419.po` (231 lines)
- `addons/event_product/i18n/et.po` (224 lines)
- `addons/event_product/i18n/event_product.pot` (216 lines)
- `addons/event_product/i18n/fa.po` (224 lines)
- `addons/event_product/i18n/fi.po` (227 lines)
- `addons/event_product/i18n/fr.po` (232 lines)
- `addons/event_product/i18n/he.po` (225 lines)
- `addons/event_product/i18n/hi.po` (224 lines)
- `addons/event_product/i18n/hr.po` (225 lines)
- `addons/event_product/i18n/hu.po` (225 lines)
- `addons/event_product/i18n/id.po` (233 lines)
- `addons/event_product/i18n/it.po` (230 lines)
- `addons/event_product/i18n/ja.po` (230 lines)
- `addons/event_product/i18n/kab.po` (220 lines)
- `addons/event_product/i18n/ko.po` (224 lines)
- `addons/event_product/i18n/ku.po` (221 lines)
- `addons/event_product/i18n/lo.po` (223 lines)
- `addons/event_product/i18n/lt.po` (226 lines)
- `addons/event_product/i18n/lv.po` (220 lines)
- `addons/event_product/i18n/mn.po` (224 lines)
- `addons/event_product/i18n/my.po` (221 lines)
- `addons/event_product/i18n/nb.po` (225 lines)
- `addons/event_product/i18n/nl.po` (231 lines)
- `addons/event_product/i18n/pl.po` (228 lines)
- `addons/event_product/i18n/pt.po` (226 lines)
- `addons/event_product/i18n/pt_BR.po` (231 lines)
- `addons/event_product/i18n/ro.po` (225 lines)
- `addons/event_product/i18n/ru.po` (228 lines)
- `addons/event_product/i18n/sk.po` (219 lines)
- `addons/event_product/i18n/sl.po` (226 lines)
- `addons/event_product/i18n/sr@latin.po` (225 lines)
- `addons/event_product/i18n/sv.po` (227 lines)
- `addons/event_product/i18n/th.po` (226 lines)
- `addons/event_product/i18n/tr.po` (228 lines)
- `addons/event_product/i18n/uk.po` (225 lines)
- `addons/event_product/i18n/uz.po` (253 lines)
- `addons/event_product/i18n/vi.po` (226 lines)
- `addons/event_product/i18n/zh_CN.po` (226 lines)
- `addons/event_product/i18n/zh_TW.po` (227 lines)
- `addons/event_product/models/__init__.py` (6 lines)
- `addons/event_product/models/event_event.py` (9 lines)
- `addons/event_product/models/event_event_ticket.py` (50 lines)
- `addons/event_product/models/event_registration.py` (24 lines)
- `addons/event_product/models/event_type_ticket.py` (104 lines)
- `addons/event_product/models/product_product.py` (18 lines)
- `addons/event_product/models/product_template.py` (12 lines)
- `addons/event_product/tests/__init__.py` (2 lines)
- `addons/event_product/tests/common.py` (33 lines)
- `addons/event_product/tests/test_event_product.py` (24 lines)
- `addons/event_product/views/event_registration_views.xml` (43 lines)
- `addons/event_product/views/event_ticket_views.xml` (119 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
