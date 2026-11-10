# Module: sale_gelato_stock

- **Module ID:** MOD-515
- **Path:** `addons/sale_gelato_stock`
- **Manifest:** `addons/sale_gelato_stock/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

No manifest description declared.

Declared dependencies: `sale_gelato`, `sale_stock`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sale_gelato",
    "sale_stock"
  ]
}
```

### Representative source files

- `addons/sale_gelato_stock/__init__.py` (3 lines)
- `addons/sale_gelato_stock/__manifest__.py` (10 lines)
- `addons/sale_gelato_stock/i18n/ar.po` (42 lines)
- `addons/sale_gelato_stock/i18n/az.po` (40 lines)
- `addons/sale_gelato_stock/i18n/bg.po` (40 lines)
- `addons/sale_gelato_stock/i18n/bs.po` (45 lines)
- `addons/sale_gelato_stock/i18n/ca.po` (41 lines)
- `addons/sale_gelato_stock/i18n/cs.po` (40 lines)
- `addons/sale_gelato_stock/i18n/da.po` (41 lines)
- `addons/sale_gelato_stock/i18n/de.po` (40 lines)
- `addons/sale_gelato_stock/i18n/el.po` (40 lines)
- `addons/sale_gelato_stock/i18n/es.po` (40 lines)
- `addons/sale_gelato_stock/i18n/es_419.po` (41 lines)
- `addons/sale_gelato_stock/i18n/et.po` (40 lines)
- `addons/sale_gelato_stock/i18n/fa.po` (40 lines)
- `addons/sale_gelato_stock/i18n/fi.po` (41 lines)
- `addons/sale_gelato_stock/i18n/fr.po` (40 lines)
- `addons/sale_gelato_stock/i18n/he.po` (41 lines)
- `addons/sale_gelato_stock/i18n/hi.po` (40 lines)
- `addons/sale_gelato_stock/i18n/hr.po` (41 lines)
- `addons/sale_gelato_stock/i18n/hu.po` (40 lines)
- `addons/sale_gelato_stock/i18n/id.po` (40 lines)
- `addons/sale_gelato_stock/i18n/it.po` (40 lines)
- `addons/sale_gelato_stock/i18n/ja.po` (40 lines)
- `addons/sale_gelato_stock/i18n/kab.po` (44 lines)
- `addons/sale_gelato_stock/i18n/ko.po` (40 lines)
- `addons/sale_gelato_stock/i18n/ku.po` (40 lines)
- `addons/sale_gelato_stock/i18n/lo.po` (43 lines)
- `addons/sale_gelato_stock/i18n/lt.po` (42 lines)
- `addons/sale_gelato_stock/i18n/lv.po` (44 lines)
- `addons/sale_gelato_stock/i18n/mn.po` (40 lines)
- `addons/sale_gelato_stock/i18n/my.po` (41 lines)
- `addons/sale_gelato_stock/i18n/nb.po` (40 lines)
- `addons/sale_gelato_stock/i18n/nl.po` (41 lines)
- `addons/sale_gelato_stock/i18n/pl.po` (41 lines)
- `addons/sale_gelato_stock/i18n/pt.po` (41 lines)
- `addons/sale_gelato_stock/i18n/pt_BR.po` (41 lines)
- `addons/sale_gelato_stock/i18n/ro.po` (42 lines)
- `addons/sale_gelato_stock/i18n/ru.po` (42 lines)
- `addons/sale_gelato_stock/i18n/sale_gelato_stock.pot` (36 lines)
- `addons/sale_gelato_stock/i18n/sk.po` (43 lines)
- `addons/sale_gelato_stock/i18n/sl.po` (41 lines)
- `addons/sale_gelato_stock/i18n/sr@latin.po` (41 lines)
- `addons/sale_gelato_stock/i18n/sv.po` (41 lines)
- `addons/sale_gelato_stock/i18n/th.po` (40 lines)
- `addons/sale_gelato_stock/i18n/tr.po` (40 lines)
- `addons/sale_gelato_stock/i18n/uk.po` (41 lines)
- `addons/sale_gelato_stock/i18n/uz.po` (50 lines)
- `addons/sale_gelato_stock/i18n/vi.po` (41 lines)
- `addons/sale_gelato_stock/i18n/zh_CN.po` (41 lines)
- `addons/sale_gelato_stock/i18n/zh_TW.po` (41 lines)
- `addons/sale_gelato_stock/models/__init__.py` (3 lines)
- `addons/sale_gelato_stock/models/sale_order_line.py` (14 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
