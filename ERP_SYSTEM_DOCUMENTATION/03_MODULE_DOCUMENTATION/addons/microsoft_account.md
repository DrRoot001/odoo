# Module: microsoft_account

- **Module ID:** MOD-374
- **Path:** `addons/microsoft_account`
- **Manifest:** `addons/microsoft_account/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


The module adds Microsoft user in res user.
===========================================


Declared dependencies: `base_setup`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base_setup"
  ],
  "data": [
    "data/microsoft_account_data.xml"
  ]
}
```

### Representative source files

- `addons/microsoft_account/__init__.py` (5 lines)
- `addons/microsoft_account/__manifest__.py` (16 lines)
- `addons/microsoft_account/controllers/__init__.py` (4 lines)
- `addons/microsoft_account/controllers/main.py` (58 lines)
- `addons/microsoft_account/data/microsoft_account_data.xml` (9 lines)
- `addons/microsoft_account/i18n/ar.po` (91 lines)
- `addons/microsoft_account/i18n/az.po` (84 lines)
- `addons/microsoft_account/i18n/bg.po` (88 lines)
- `addons/microsoft_account/i18n/bs.po` (85 lines)
- `addons/microsoft_account/i18n/ca.po` (87 lines)
- `addons/microsoft_account/i18n/cs.po` (88 lines)
- `addons/microsoft_account/i18n/da.po` (89 lines)
- `addons/microsoft_account/i18n/de.po` (91 lines)
- `addons/microsoft_account/i18n/el.po` (85 lines)
- `addons/microsoft_account/i18n/es.po` (92 lines)
- `addons/microsoft_account/i18n/es_419.po` (89 lines)
- `addons/microsoft_account/i18n/et.po` (86 lines)
- `addons/microsoft_account/i18n/fa.po` (84 lines)
- `addons/microsoft_account/i18n/fi.po` (92 lines)
- `addons/microsoft_account/i18n/fr.po` (89 lines)
- `addons/microsoft_account/i18n/he.po` (86 lines)
- `addons/microsoft_account/i18n/hi.po` (84 lines)
- `addons/microsoft_account/i18n/hr.po` (87 lines)
- `addons/microsoft_account/i18n/hu.po` (88 lines)
- `addons/microsoft_account/i18n/id.po` (89 lines)
- `addons/microsoft_account/i18n/it.po` (91 lines)
- `addons/microsoft_account/i18n/ja.po` (89 lines)
- `addons/microsoft_account/i18n/kab.po` (84 lines)
- `addons/microsoft_account/i18n/ko.po` (86 lines)
- `addons/microsoft_account/i18n/ku.po` (84 lines)
- `addons/microsoft_account/i18n/lo.po` (83 lines)
- `addons/microsoft_account/i18n/lt.po` (88 lines)
- `addons/microsoft_account/i18n/lv.po` (84 lines)
- `addons/microsoft_account/i18n/microsoft_account.pot` (80 lines)
- `addons/microsoft_account/i18n/mn.po` (87 lines)
- `addons/microsoft_account/i18n/my.po` (84 lines)
- `addons/microsoft_account/i18n/nb.po` (85 lines)
- `addons/microsoft_account/i18n/nl.po` (92 lines)
- `addons/microsoft_account/i18n/pl.po` (88 lines)
- `addons/microsoft_account/i18n/pt.po` (89 lines)
- `addons/microsoft_account/i18n/pt_BR.po` (93 lines)
- `addons/microsoft_account/i18n/ro.po` (88 lines)
- `addons/microsoft_account/i18n/ru.po` (90 lines)
- `addons/microsoft_account/i18n/sk.po` (83 lines)
- `addons/microsoft_account/i18n/sl.po` (86 lines)
- `addons/microsoft_account/i18n/sr@latin.po` (85 lines)
- `addons/microsoft_account/i18n/sv.po` (88 lines)
- `addons/microsoft_account/i18n/th.po` (85 lines)
- `addons/microsoft_account/i18n/tr.po` (92 lines)
- `addons/microsoft_account/i18n/uk.po` (87 lines)
- `addons/microsoft_account/i18n/uz.po` (104 lines)
- `addons/microsoft_account/i18n/vi.po` (90 lines)
- `addons/microsoft_account/i18n/zh_CN.po` (88 lines)
- `addons/microsoft_account/i18n/zh_TW.po` (87 lines)
- `addons/microsoft_account/models/__init__.py` (5 lines)
- `addons/microsoft_account/models/microsoft_service.py` (183 lines)
- `addons/microsoft_account/models/res_users.py` (22 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
