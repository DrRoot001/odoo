# Module: stock_sms

- **Module ID:** MOD-566
- **Path:** `addons/stock_sms`
- **Manifest:** `addons/stock_sms/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Send text messages when final stock move

Send text messages when final stock move

Declared dependencies: `stock`, `sms`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "stock",
    "sms"
  ],
  "data": [
    "data/sms_data.xml",
    "views/res_config_settings_views.xml",
    "wizard/confirm_stock_sms_views.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/stock_sms/__init__.py` (27 lines)
- `addons/stock_sms/__manifest__.py` (20 lines)
- `addons/stock_sms/data/sms_data.xml` (12 lines)
- `addons/stock_sms/i18n/ar.po` (176 lines)
- `addons/stock_sms/i18n/az.po` (156 lines)
- `addons/stock_sms/i18n/bg.po` (156 lines)
- `addons/stock_sms/i18n/bs.po` (157 lines)
- `addons/stock_sms/i18n/ca.po` (160 lines)
- `addons/stock_sms/i18n/cs.po` (165 lines)
- `addons/stock_sms/i18n/da.po` (164 lines)
- `addons/stock_sms/i18n/de.po` (176 lines)
- `addons/stock_sms/i18n/el.po` (156 lines)
- `addons/stock_sms/i18n/es.po` (177 lines)
- `addons/stock_sms/i18n/es_419.po` (174 lines)
- `addons/stock_sms/i18n/et.po` (159 lines)
- `addons/stock_sms/i18n/fa.po` (159 lines)
- `addons/stock_sms/i18n/fi.po` (172 lines)
- `addons/stock_sms/i18n/fr.po` (178 lines)
- `addons/stock_sms/i18n/he.po` (167 lines)
- `addons/stock_sms/i18n/hi.po` (156 lines)
- `addons/stock_sms/i18n/hr.po` (161 lines)
- `addons/stock_sms/i18n/hu.po` (164 lines)
- `addons/stock_sms/i18n/id.po` (173 lines)
- `addons/stock_sms/i18n/it.po` (178 lines)
- `addons/stock_sms/i18n/ja.po` (172 lines)
- `addons/stock_sms/i18n/kab.po` (156 lines)
- `addons/stock_sms/i18n/ko.po` (172 lines)
- `addons/stock_sms/i18n/ku.po` (156 lines)
- `addons/stock_sms/i18n/lo.po` (155 lines)
- `addons/stock_sms/i18n/lt.po` (165 lines)
- `addons/stock_sms/i18n/lv.po` (156 lines)
- `addons/stock_sms/i18n/mn.po` (163 lines)
- `addons/stock_sms/i18n/my.po` (157 lines)
- `addons/stock_sms/i18n/nb.po` (161 lines)
- `addons/stock_sms/i18n/nl.po` (175 lines)
- `addons/stock_sms/i18n/pl.po` (172 lines)
- `addons/stock_sms/i18n/pt.po` (169 lines)
- `addons/stock_sms/i18n/pt_BR.po` (178 lines)
- `addons/stock_sms/i18n/ro.po` (166 lines)
- `addons/stock_sms/i18n/ru.po` (162 lines)
- `addons/stock_sms/i18n/sk.po` (155 lines)
- `addons/stock_sms/i18n/sl.po` (157 lines)
- `addons/stock_sms/i18n/sr@latin.po` (157 lines)
- `addons/stock_sms/i18n/stock_sms.pot` (142 lines)
- `addons/stock_sms/i18n/sv.po` (160 lines)
- `addons/stock_sms/i18n/th.po` (172 lines)
- `addons/stock_sms/i18n/tr.po` (178 lines)
- `addons/stock_sms/i18n/uk.po` (166 lines)
- `addons/stock_sms/i18n/uz.po` (185 lines)
- `addons/stock_sms/i18n/vi.po` (164 lines)
- `addons/stock_sms/i18n/zh_CN.po` (175 lines)
- `addons/stock_sms/i18n/zh_TW.po` (160 lines)
- `addons/stock_sms/models/__init__.py` (6 lines)
- `addons/stock_sms/models/res_company.py` (21 lines)
- `addons/stock_sms/models/res_config_settings.py` (11 lines)
- `addons/stock_sms/models/stock_picking.py` (57 lines)
- `addons/stock_sms/security/ir.access.csv` (4 lines)
- `addons/stock_sms/views/res_config_settings_views.xml` (24 lines)
- `addons/stock_sms/wizard/__init__.py` (4 lines)
- `addons/stock_sms/wizard/confirm_stock_sms.py` (30 lines)
- `addons/stock_sms/wizard/confirm_stock_sms_views.xml` (20 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
