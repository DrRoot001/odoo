# Module: pos_self_order_sale

- **Module ID:** MOD-461
- **Path:** `addons/pos_self_order_sale`
- **Manifest:** `addons/pos_self_order_sale/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

No manifest description declared.

Declared dependencies: `pos_sale`, `pos_self_order`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "pos_sale",
    "pos_self_order"
  ],
  "data": [
    "views/res_config_settings_views.xml",
    "data/kiosk_sale_team.xml"
  ]
}
```

### Representative source files

- `addons/pos_self_order_sale/__init__.py` (3 lines)
- `addons/pos_self_order_sale/__manifest__.py` (12 lines)
- `addons/pos_self_order_sale/data/kiosk_sale_team.xml` (8 lines)
- `addons/pos_self_order_sale/i18n/ar.po` (47 lines)
- `addons/pos_self_order_sale/i18n/az.po` (45 lines)
- `addons/pos_self_order_sale/i18n/bg.po` (45 lines)
- `addons/pos_self_order_sale/i18n/bs.po` (46 lines)
- `addons/pos_self_order_sale/i18n/ca.po` (46 lines)
- `addons/pos_self_order_sale/i18n/cs.po` (46 lines)
- `addons/pos_self_order_sale/i18n/da.po` (47 lines)
- `addons/pos_self_order_sale/i18n/de.po` (46 lines)
- `addons/pos_self_order_sale/i18n/el.po` (46 lines)
- `addons/pos_self_order_sale/i18n/es.po` (47 lines)
- `addons/pos_self_order_sale/i18n/es_419.po` (46 lines)
- `addons/pos_self_order_sale/i18n/et.po` (45 lines)
- `addons/pos_self_order_sale/i18n/fa.po` (45 lines)
- `addons/pos_self_order_sale/i18n/fi.po` (46 lines)
- `addons/pos_self_order_sale/i18n/fr.po` (46 lines)
- `addons/pos_self_order_sale/i18n/he.po` (46 lines)
- `addons/pos_self_order_sale/i18n/hi.po` (45 lines)
- `addons/pos_self_order_sale/i18n/hr.po` (46 lines)
- `addons/pos_self_order_sale/i18n/hu.po` (46 lines)
- `addons/pos_self_order_sale/i18n/id.po` (46 lines)
- `addons/pos_self_order_sale/i18n/it.po` (46 lines)
- `addons/pos_self_order_sale/i18n/ja.po` (46 lines)
- `addons/pos_self_order_sale/i18n/kab.po` (45 lines)
- `addons/pos_self_order_sale/i18n/ko.po` (47 lines)
- `addons/pos_self_order_sale/i18n/ku.po` (45 lines)
- `addons/pos_self_order_sale/i18n/lo.po` (44 lines)
- `addons/pos_self_order_sale/i18n/lt.po` (47 lines)
- `addons/pos_self_order_sale/i18n/lv.po` (45 lines)
- `addons/pos_self_order_sale/i18n/mn.po` (45 lines)
- `addons/pos_self_order_sale/i18n/my.po` (45 lines)
- `addons/pos_self_order_sale/i18n/nb.po` (46 lines)
- `addons/pos_self_order_sale/i18n/nl.po` (46 lines)
- `addons/pos_self_order_sale/i18n/pl.po` (47 lines)
- `addons/pos_self_order_sale/i18n/pos_self_order_sale.pot` (41 lines)
- `addons/pos_self_order_sale/i18n/pt.po` (47 lines)
- `addons/pos_self_order_sale/i18n/pt_BR.po` (47 lines)
- `addons/pos_self_order_sale/i18n/ro.po` (47 lines)
- `addons/pos_self_order_sale/i18n/ru.po` (49 lines)
- `addons/pos_self_order_sale/i18n/sk.po` (44 lines)
- `addons/pos_self_order_sale/i18n/sl.po` (47 lines)
- `addons/pos_self_order_sale/i18n/sr@latin.po` (46 lines)
- `addons/pos_self_order_sale/i18n/sv.po` (47 lines)
- `addons/pos_self_order_sale/i18n/th.po` (46 lines)
- `addons/pos_self_order_sale/i18n/tr.po` (45 lines)
- `addons/pos_self_order_sale/i18n/uk.po` (46 lines)
- `addons/pos_self_order_sale/i18n/uz.po` (56 lines)
- `addons/pos_self_order_sale/i18n/vi.po` (47 lines)
- `addons/pos_self_order_sale/i18n/zh_CN.po` (46 lines)
- `addons/pos_self_order_sale/i18n/zh_TW.po` (48 lines)
- `addons/pos_self_order_sale/models/__init__.py` (3 lines)
- `addons/pos_self_order_sale/models/res_config_settings.py` (16 lines)
- `addons/pos_self_order_sale/views/res_config_settings_views.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
