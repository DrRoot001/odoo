# Module: account_update_tax_tags

- **Module ID:** MOD-016
- **Path:** `addons/account_update_tax_tags`
- **Manifest:** `addons/account_update_tax_tags/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Allow updating tax grids on existing entries


    This module allows updating tax grids on existing accounting entries.
    In debug mode a button to update your entries' tax grids will be available
    in Accounting settings.
    This is typically useful after some legal changes were done on the tax report,
    requiring a new tax configuration.
    

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account"
  ],
  "data": [
    "views/res_config_settings_views.xml",
    "wizard/account_update_tax_tags_wizard.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/account_update_tax_tags/__init__.py` (1 lines)
- `addons/account_update_tax_tags/__manifest__.py` (20 lines)
- `addons/account_update_tax_tags/i18n/account_update_tax_tags.pot` (127 lines)
- `addons/account_update_tax_tags/i18n/ar.po` (154 lines)
- `addons/account_update_tax_tags/i18n/az.po` (136 lines)
- `addons/account_update_tax_tags/i18n/bg.po` (136 lines)
- `addons/account_update_tax_tags/i18n/bs.po` (138 lines)
- `addons/account_update_tax_tags/i18n/ca.po` (149 lines)
- `addons/account_update_tax_tags/i18n/cs.po` (136 lines)
- `addons/account_update_tax_tags/i18n/da.po` (149 lines)
- `addons/account_update_tax_tags/i18n/de.po` (159 lines)
- `addons/account_update_tax_tags/i18n/el.po` (136 lines)
- `addons/account_update_tax_tags/i18n/es.po` (159 lines)
- `addons/account_update_tax_tags/i18n/es_419.po` (159 lines)
- `addons/account_update_tax_tags/i18n/et.po` (145 lines)
- `addons/account_update_tax_tags/i18n/fa.po` (136 lines)
- `addons/account_update_tax_tags/i18n/fi.po` (155 lines)
- `addons/account_update_tax_tags/i18n/fr.po` (162 lines)
- `addons/account_update_tax_tags/i18n/he.po` (137 lines)
- `addons/account_update_tax_tags/i18n/hi.po` (137 lines)
- `addons/account_update_tax_tags/i18n/hr.po` (137 lines)
- `addons/account_update_tax_tags/i18n/hu.po` (136 lines)
- `addons/account_update_tax_tags/i18n/id.po` (150 lines)
- `addons/account_update_tax_tags/i18n/it.po` (159 lines)
- `addons/account_update_tax_tags/i18n/ja.po` (152 lines)
- `addons/account_update_tax_tags/i18n/kab.po` (137 lines)
- `addons/account_update_tax_tags/i18n/ko.po` (146 lines)
- `addons/account_update_tax_tags/i18n/ku.po` (138 lines)
- `addons/account_update_tax_tags/i18n/lo.po` (135 lines)
- `addons/account_update_tax_tags/i18n/lt.po` (138 lines)
- `addons/account_update_tax_tags/i18n/lv.po` (138 lines)
- `addons/account_update_tax_tags/i18n/mn.po` (136 lines)
- `addons/account_update_tax_tags/i18n/my.po` (137 lines)
- `addons/account_update_tax_tags/i18n/nb.po` (136 lines)
- `addons/account_update_tax_tags/i18n/nl.po` (150 lines)
- `addons/account_update_tax_tags/i18n/pl.po` (159 lines)
- `addons/account_update_tax_tags/i18n/pt.po` (150 lines)
- `addons/account_update_tax_tags/i18n/pt_BR.po` (159 lines)
- `addons/account_update_tax_tags/i18n/ro.po` (151 lines)
- `addons/account_update_tax_tags/i18n/ru.po` (151 lines)
- `addons/account_update_tax_tags/i18n/sk.po` (137 lines)
- `addons/account_update_tax_tags/i18n/sl.po` (147 lines)
- `addons/account_update_tax_tags/i18n/sr@latin.po` (137 lines)
- `addons/account_update_tax_tags/i18n/sv.po` (160 lines)
- `addons/account_update_tax_tags/i18n/th.po` (143 lines)
- `addons/account_update_tax_tags/i18n/tr.po` (157 lines)
- `addons/account_update_tax_tags/i18n/uk.po` (158 lines)
- `addons/account_update_tax_tags/i18n/uz.po` (169 lines)
- `addons/account_update_tax_tags/i18n/vi.po` (144 lines)
- `addons/account_update_tax_tags/i18n/zh_CN.po` (148 lines)
- `addons/account_update_tax_tags/i18n/zh_TW.po` (144 lines)
- `addons/account_update_tax_tags/security/ir.access.csv` (2 lines)
- `addons/account_update_tax_tags/tests/__init__.py` (1 lines)
- `addons/account_update_tax_tags/tests/test_account_update_tax_tags_wizard.py` (420 lines)
- `addons/account_update_tax_tags/views/res_config_settings_views.xml` (25 lines)
- `addons/account_update_tax_tags/wizard/__init__.py` (1 lines)
- `addons/account_update_tax_tags/wizard/account_update_tax_tags_wizard.py` (182 lines)
- `addons/account_update_tax_tags/wizard/account_update_tax_tags_wizard.xml` (29 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
