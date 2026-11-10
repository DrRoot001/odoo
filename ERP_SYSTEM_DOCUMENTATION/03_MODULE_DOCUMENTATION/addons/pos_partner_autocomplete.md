# Module: pos_partner_autocomplete

- **Module ID:** MOD-442
- **Path:** `addons/pos_partner_autocomplete`
- **Manifest:** `addons/pos_partner_autocomplete/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Link module between Partner Autocomplete and Point of Sale


This module links Partner Autocomplete with the Point of Sale, allowing partner data to be auto-completed from the POS frontend.
This module ensures that the Point of Sale remains independent of Partner Autocomplete.
    

Declared dependencies: `partner_autocomplete`, `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 2 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
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
    "partner_autocomplete",
    "point_of_sale"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "partner_autocomplete/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_partner_autocomplete/__init__.py` (0 lines)
- `addons/pos_partner_autocomplete/__manifest__.py` (20 lines)
- `addons/pos_partner_autocomplete/i18n/ar.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/az.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/bg.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/bs.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/ca.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/cs.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/da.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/de.po` (46 lines)
- `addons/pos_partner_autocomplete/i18n/el.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/es.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/es_419.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/et.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/fa.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/fi.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/fr.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/he.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/hi.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/hr.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/hu.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/id.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/it.po` (44 lines)
- `addons/pos_partner_autocomplete/i18n/ja.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/kab.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/ko.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/ku.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/lo.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/lt.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/lv.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/mn.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/my.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/nb.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/nl.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/pl.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/pos_partner_autocomplete.pot` (34 lines)
- `addons/pos_partner_autocomplete/i18n/pt.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/pt_BR.po` (46 lines)
- `addons/pos_partner_autocomplete/i18n/ro.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/ru.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/sk.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/sl.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/sr@latin.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/sv.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/th.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/tr.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/uk.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/uz.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/vi.po` (34 lines)
- `addons/pos_partner_autocomplete/i18n/zh_CN.po` (38 lines)
- `addons/pos_partner_autocomplete/i18n/zh_TW.po` (34 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
