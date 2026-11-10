# Module: pos_sale_delivery

- **Module ID:** MOD-451
- **Path:** `addons/pos_sale_delivery`
- **Manifest:** `addons/pos_sale_delivery/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Link module between Point of Sale and Delivery

Declared dependencies: `pos_sale`, `stock_delivery`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "pos_sale",
    "stock_delivery"
  ]
}
```

### Representative source files

- `addons/pos_sale_delivery/__init__.py` (3 lines)
- `addons/pos_sale_delivery/__manifest__.py` (11 lines)
- `addons/pos_sale_delivery/i18n/ar.po` (47 lines)
- `addons/pos_sale_delivery/i18n/az.po` (47 lines)
- `addons/pos_sale_delivery/i18n/bg.po` (47 lines)
- `addons/pos_sale_delivery/i18n/bs.po` (47 lines)
- `addons/pos_sale_delivery/i18n/ca.po` (47 lines)
- `addons/pos_sale_delivery/i18n/cs.po` (47 lines)
- `addons/pos_sale_delivery/i18n/da.po` (47 lines)
- `addons/pos_sale_delivery/i18n/de.po` (51 lines)
- `addons/pos_sale_delivery/i18n/el.po` (47 lines)
- `addons/pos_sale_delivery/i18n/es.po` (51 lines)
- `addons/pos_sale_delivery/i18n/es_419.po` (51 lines)
- `addons/pos_sale_delivery/i18n/et.po` (47 lines)
- `addons/pos_sale_delivery/i18n/fa.po` (47 lines)
- `addons/pos_sale_delivery/i18n/fi.po` (51 lines)
- `addons/pos_sale_delivery/i18n/fr.po` (47 lines)
- `addons/pos_sale_delivery/i18n/he.po` (47 lines)
- `addons/pos_sale_delivery/i18n/hi.po` (47 lines)
- `addons/pos_sale_delivery/i18n/hr.po` (47 lines)
- `addons/pos_sale_delivery/i18n/hu.po` (47 lines)
- `addons/pos_sale_delivery/i18n/id.po` (47 lines)
- `addons/pos_sale_delivery/i18n/it.po` (51 lines)
- `addons/pos_sale_delivery/i18n/ja.po` (47 lines)
- `addons/pos_sale_delivery/i18n/kab.po` (47 lines)
- `addons/pos_sale_delivery/i18n/ko.po` (47 lines)
- `addons/pos_sale_delivery/i18n/ku.po` (47 lines)
- `addons/pos_sale_delivery/i18n/lo.po` (47 lines)
- `addons/pos_sale_delivery/i18n/lt.po` (47 lines)
- `addons/pos_sale_delivery/i18n/lv.po` (47 lines)
- `addons/pos_sale_delivery/i18n/mn.po` (47 lines)
- `addons/pos_sale_delivery/i18n/my.po` (47 lines)
- `addons/pos_sale_delivery/i18n/nb.po` (47 lines)
- `addons/pos_sale_delivery/i18n/nl.po` (51 lines)
- `addons/pos_sale_delivery/i18n/pl.po` (47 lines)
- `addons/pos_sale_delivery/i18n/pos_sale_delivery.pot` (47 lines)
- `addons/pos_sale_delivery/i18n/pt.po` (47 lines)
- `addons/pos_sale_delivery/i18n/pt_BR.po` (52 lines)
- `addons/pos_sale_delivery/i18n/ro.po` (47 lines)
- `addons/pos_sale_delivery/i18n/ru.po` (47 lines)
- `addons/pos_sale_delivery/i18n/sk.po` (47 lines)
- `addons/pos_sale_delivery/i18n/sl.po` (47 lines)
- `addons/pos_sale_delivery/i18n/sr@latin.po` (47 lines)
- `addons/pos_sale_delivery/i18n/sv.po` (51 lines)
- `addons/pos_sale_delivery/i18n/th.po` (47 lines)
- `addons/pos_sale_delivery/i18n/tr.po` (47 lines)
- `addons/pos_sale_delivery/i18n/uk.po` (47 lines)
- `addons/pos_sale_delivery/i18n/uz.po` (47 lines)
- `addons/pos_sale_delivery/i18n/vi.po` (47 lines)
- `addons/pos_sale_delivery/i18n/zh_CN.po` (51 lines)
- `addons/pos_sale_delivery/i18n/zh_TW.po` (47 lines)
- `addons/pos_sale_delivery/models/__init__.py` (3 lines)
- `addons/pos_sale_delivery/models/pos_order.py` (25 lines)
- `addons/pos_sale_delivery/tests/__init__.py` (3 lines)
- `addons/pos_sale_delivery/tests/test_pos_sale_delivery.py` (40 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
