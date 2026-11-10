# Module: sale_stock_margin

- **Module ID:** MOD-534
- **Path:** `addons/sale_stock_margin`
- **Manifest:** `addons/sale_stock_margin/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Once the delivery is validated, update the cost on the SO to have an exact margin computation.

Declared dependencies: `sale_stock`, `sale_margin`.

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
    "sale_stock",
    "sale_margin"
  ]
}
```

### Representative source files

- `addons/sale_stock_margin/__init__.py` (4 lines)
- `addons/sale_stock_margin/__manifest__.py` (9 lines)
- `addons/sale_stock_margin/i18n/ar.po` (49 lines)
- `addons/sale_stock_margin/i18n/az.po` (46 lines)
- `addons/sale_stock_margin/i18n/bg.po` (46 lines)
- `addons/sale_stock_margin/i18n/bs.po` (48 lines)
- `addons/sale_stock_margin/i18n/ca.po` (47 lines)
- `addons/sale_stock_margin/i18n/cs.po` (48 lines)
- `addons/sale_stock_margin/i18n/da.po` (47 lines)
- `addons/sale_stock_margin/i18n/de.po` (50 lines)
- `addons/sale_stock_margin/i18n/el.po` (47 lines)
- `addons/sale_stock_margin/i18n/es.po` (51 lines)
- `addons/sale_stock_margin/i18n/es_419.po` (48 lines)
- `addons/sale_stock_margin/i18n/et.po` (46 lines)
- `addons/sale_stock_margin/i18n/fa.po` (46 lines)
- `addons/sale_stock_margin/i18n/fi.po` (50 lines)
- `addons/sale_stock_margin/i18n/fr.po` (48 lines)
- `addons/sale_stock_margin/i18n/he.po` (47 lines)
- `addons/sale_stock_margin/i18n/hi.po` (46 lines)
- `addons/sale_stock_margin/i18n/hr.po` (47 lines)
- `addons/sale_stock_margin/i18n/hu.po` (47 lines)
- `addons/sale_stock_margin/i18n/id.po` (48 lines)
- `addons/sale_stock_margin/i18n/it.po` (48 lines)
- `addons/sale_stock_margin/i18n/ja.po` (48 lines)
- `addons/sale_stock_margin/i18n/kab.po` (47 lines)
- `addons/sale_stock_margin/i18n/ko.po` (48 lines)
- `addons/sale_stock_margin/i18n/ku.po` (46 lines)
- `addons/sale_stock_margin/i18n/lo.po` (46 lines)
- `addons/sale_stock_margin/i18n/lt.po` (48 lines)
- `addons/sale_stock_margin/i18n/lv.po` (47 lines)
- `addons/sale_stock_margin/i18n/mn.po` (46 lines)
- `addons/sale_stock_margin/i18n/my.po` (46 lines)
- `addons/sale_stock_margin/i18n/nb.po` (47 lines)
- `addons/sale_stock_margin/i18n/nl.po` (48 lines)
- `addons/sale_stock_margin/i18n/pl.po` (49 lines)
- `addons/sale_stock_margin/i18n/pt.po` (47 lines)
- `addons/sale_stock_margin/i18n/pt_BR.po` (52 lines)
- `addons/sale_stock_margin/i18n/ro.po` (48 lines)
- `addons/sale_stock_margin/i18n/ru.po` (50 lines)
- `addons/sale_stock_margin/i18n/sale_stock_margin.pot` (43 lines)
- `addons/sale_stock_margin/i18n/sk.po` (46 lines)
- `addons/sale_stock_margin/i18n/sl.po` (48 lines)
- `addons/sale_stock_margin/i18n/sr@latin.po` (47 lines)
- `addons/sale_stock_margin/i18n/sv.po` (49 lines)
- `addons/sale_stock_margin/i18n/th.po` (48 lines)
- `addons/sale_stock_margin/i18n/tr.po` (48 lines)
- `addons/sale_stock_margin/i18n/uk.po` (47 lines)
- `addons/sale_stock_margin/i18n/uz.po` (57 lines)
- `addons/sale_stock_margin/i18n/vi.po` (48 lines)
- `addons/sale_stock_margin/i18n/zh_CN.po` (48 lines)
- `addons/sale_stock_margin/i18n/zh_TW.po` (50 lines)
- `addons/sale_stock_margin/models/__init__.py` (4 lines)
- `addons/sale_stock_margin/models/sale_order_line.py` (36 lines)
- `addons/sale_stock_margin/tests/__init__.py` (3 lines)
- `addons/sale_stock_margin/tests/test_sale_stock_margin.py` (716 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
