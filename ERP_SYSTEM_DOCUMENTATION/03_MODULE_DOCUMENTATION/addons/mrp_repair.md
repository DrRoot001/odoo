# Module: mrp_repair

- **Module ID:** MOD-382
- **Path:** `addons/mrp_repair`
- **Manifest:** `addons/mrp_repair/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

No manifest description declared.

Declared dependencies: `repair`, `mrp`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "repair",
    "mrp"
  ],
  "data": [
    "views/production_views.xml",
    "views/repair_views.xml"
  ]
}
```

### Representative source files

- `addons/mrp_repair/__init__.py` (4 lines)
- `addons/mrp_repair/__manifest__.py` (15 lines)
- `addons/mrp_repair/i18n/ar.po` (88 lines)
- `addons/mrp_repair/i18n/az.po` (92 lines)
- `addons/mrp_repair/i18n/bg.po` (94 lines)
- `addons/mrp_repair/i18n/bs.po` (95 lines)
- `addons/mrp_repair/i18n/ca.po` (90 lines)
- `addons/mrp_repair/i18n/cs.po` (87 lines)
- `addons/mrp_repair/i18n/da.po` (90 lines)
- `addons/mrp_repair/i18n/de.po` (87 lines)
- `addons/mrp_repair/i18n/el.po` (89 lines)
- `addons/mrp_repair/i18n/es.po` (88 lines)
- `addons/mrp_repair/i18n/es_419.po` (87 lines)
- `addons/mrp_repair/i18n/et.po` (86 lines)
- `addons/mrp_repair/i18n/fa.po` (93 lines)
- `addons/mrp_repair/i18n/fi.po` (87 lines)
- `addons/mrp_repair/i18n/fr.po` (87 lines)
- `addons/mrp_repair/i18n/he.po` (98 lines)
- `addons/mrp_repair/i18n/hi.po` (93 lines)
- `addons/mrp_repair/i18n/hr.po` (94 lines)
- `addons/mrp_repair/i18n/hu.po` (89 lines)
- `addons/mrp_repair/i18n/id.po` (88 lines)
- `addons/mrp_repair/i18n/it.po` (87 lines)
- `addons/mrp_repair/i18n/ja.po` (87 lines)
- `addons/mrp_repair/i18n/kab.po` (90 lines)
- `addons/mrp_repair/i18n/ko.po` (87 lines)
- `addons/mrp_repair/i18n/ku.po` (87 lines)
- `addons/mrp_repair/i18n/lo.po` (97 lines)
- `addons/mrp_repair/i18n/lt.po` (95 lines)
- `addons/mrp_repair/i18n/lv.po` (94 lines)
- `addons/mrp_repair/i18n/mn.po` (93 lines)
- `addons/mrp_repair/i18n/mrp_repair.pot` (82 lines)
- `addons/mrp_repair/i18n/my.po` (93 lines)
- `addons/mrp_repair/i18n/nb.po` (89 lines)
- `addons/mrp_repair/i18n/nl.po` (87 lines)
- `addons/mrp_repair/i18n/pl.po` (88 lines)
- `addons/mrp_repair/i18n/pt.po` (89 lines)
- `addons/mrp_repair/i18n/pt_BR.po` (88 lines)
- `addons/mrp_repair/i18n/ro.po` (88 lines)
- `addons/mrp_repair/i18n/ru.po` (91 lines)
- `addons/mrp_repair/i18n/sk.po` (95 lines)
- `addons/mrp_repair/i18n/sl.po` (90 lines)
- `addons/mrp_repair/i18n/sr@latin.po` (94 lines)
- `addons/mrp_repair/i18n/sv.po` (87 lines)
- `addons/mrp_repair/i18n/th.po` (89 lines)
- `addons/mrp_repair/i18n/tr.po` (88 lines)
- `addons/mrp_repair/i18n/uk.po` (98 lines)
- `addons/mrp_repair/i18n/uz.po` (104 lines)
- `addons/mrp_repair/i18n/vi.po` (89 lines)
- `addons/mrp_repair/i18n/zh_CN.po` (87 lines)
- `addons/mrp_repair/i18n/zh_TW.po` (89 lines)
- `addons/mrp_repair/models/__init__.py` (6 lines)
- `addons/mrp_repair/models/production.py` (38 lines)
- `addons/mrp_repair/models/repair.py` (93 lines)
- `addons/mrp_repair/models/stock_move.py` (11 lines)
- `addons/mrp_repair/tests/__init__.py` (5 lines)
- `addons/mrp_repair/tests/test_mrp_repair_flow.py` (116 lines)
- `addons/mrp_repair/tests/test_tracability.py` (359 lines)
- `addons/mrp_repair/views/production_views.xml` (22 lines)
- `addons/mrp_repair/views/repair_views.xml` (22 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
