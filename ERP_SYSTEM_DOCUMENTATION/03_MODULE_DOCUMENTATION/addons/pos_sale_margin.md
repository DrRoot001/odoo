# Module: pos_sale_margin

- **Module ID:** MOD-453
- **Path:** `addons/pos_sale_margin`
- **Manifest:** `addons/pos_sale_margin/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Link module between Point of Sale and Sales Margin



This module adds enable you to view the margin of your Point of Sale orders in the Sales Margin report.


Declared dependencies: `pos_sale`, `sale_margin`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
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
    "sale_margin"
  ]
}
```

### Representative source files

- `addons/pos_sale_margin/__init__.py` (4 lines)
- `addons/pos_sale_margin/__manifest__.py` (17 lines)
- `addons/pos_sale_margin/i18n/ar.po` (56 lines)
- `addons/pos_sale_margin/i18n/az.po` (53 lines)
- `addons/pos_sale_margin/i18n/bg.po` (53 lines)
- `addons/pos_sale_margin/i18n/bs.po` (55 lines)
- `addons/pos_sale_margin/i18n/ca.po` (54 lines)
- `addons/pos_sale_margin/i18n/cs.po` (55 lines)
- `addons/pos_sale_margin/i18n/da.po` (54 lines)
- `addons/pos_sale_margin/i18n/de.po` (59 lines)
- `addons/pos_sale_margin/i18n/el.po` (54 lines)
- `addons/pos_sale_margin/i18n/es.po` (60 lines)
- `addons/pos_sale_margin/i18n/es_419.po` (55 lines)
- `addons/pos_sale_margin/i18n/et.po` (53 lines)
- `addons/pos_sale_margin/i18n/fa.po` (53 lines)
- `addons/pos_sale_margin/i18n/fi.po` (55 lines)
- `addons/pos_sale_margin/i18n/fr.po` (55 lines)
- `addons/pos_sale_margin/i18n/he.po` (54 lines)
- `addons/pos_sale_margin/i18n/hi.po` (53 lines)
- `addons/pos_sale_margin/i18n/hr.po` (54 lines)
- `addons/pos_sale_margin/i18n/hu.po` (54 lines)
- `addons/pos_sale_margin/i18n/id.po` (55 lines)
- `addons/pos_sale_margin/i18n/it.po` (59 lines)
- `addons/pos_sale_margin/i18n/ja.po` (55 lines)
- `addons/pos_sale_margin/i18n/kab.po` (54 lines)
- `addons/pos_sale_margin/i18n/ko.po` (55 lines)
- `addons/pos_sale_margin/i18n/ku.po` (53 lines)
- `addons/pos_sale_margin/i18n/lo.po` (53 lines)
- `addons/pos_sale_margin/i18n/lt.po` (55 lines)
- `addons/pos_sale_margin/i18n/lv.po` (54 lines)
- `addons/pos_sale_margin/i18n/mn.po` (53 lines)
- `addons/pos_sale_margin/i18n/my.po` (53 lines)
- `addons/pos_sale_margin/i18n/nb.po` (54 lines)
- `addons/pos_sale_margin/i18n/nl.po` (55 lines)
- `addons/pos_sale_margin/i18n/pl.po` (56 lines)
- `addons/pos_sale_margin/i18n/pos_sale_margin.pot` (49 lines)
- `addons/pos_sale_margin/i18n/pt.po` (54 lines)
- `addons/pos_sale_margin/i18n/pt_BR.po` (61 lines)
- `addons/pos_sale_margin/i18n/ro.po` (55 lines)
- `addons/pos_sale_margin/i18n/ru.po` (57 lines)
- `addons/pos_sale_margin/i18n/sk.po` (53 lines)
- `addons/pos_sale_margin/i18n/sl.po` (55 lines)
- `addons/pos_sale_margin/i18n/sr@latin.po` (54 lines)
- `addons/pos_sale_margin/i18n/sv.po` (55 lines)
- `addons/pos_sale_margin/i18n/th.po` (55 lines)
- `addons/pos_sale_margin/i18n/tr.po` (55 lines)
- `addons/pos_sale_margin/i18n/uk.po` (54 lines)
- `addons/pos_sale_margin/i18n/uz.po` (64 lines)
- `addons/pos_sale_margin/i18n/vi.po` (55 lines)
- `addons/pos_sale_margin/i18n/zh_CN.po` (55 lines)
- `addons/pos_sale_margin/i18n/zh_TW.po` (57 lines)
- `addons/pos_sale_margin/report/__init__.py` (4 lines)
- `addons/pos_sale_margin/report/sale_report.py` (17 lines)
- `addons/pos_sale_margin/tests/__init__.py` (4 lines)
- `addons/pos_sale_margin/tests/test_pos_sale_margin_report.py` (72 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
