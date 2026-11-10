# Module: google_account

- **Module ID:** MOD-076
- **Path:** `addons/google_account`
- **Manifest:** `addons/google_account/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


The module adds google user in res user.
========================================


Declared dependencies: `base_setup`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
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
  ]
}
```

### Representative source files

- `addons/google_account/__init__.py` (7 lines)
- `addons/google_account/__manifest__.py` (13 lines)
- `addons/google_account/controllers/__init__.py` (1 lines)
- `addons/google_account/controllers/main.py` (62 lines)
- `addons/google_account/i18n/ar.po` (73 lines)
- `addons/google_account/i18n/az.po` (62 lines)
- `addons/google_account/i18n/bg.po` (68 lines)
- `addons/google_account/i18n/bs.po` (66 lines)
- `addons/google_account/i18n/ca.po` (68 lines)
- `addons/google_account/i18n/cs.po` (69 lines)
- `addons/google_account/i18n/da.po` (69 lines)
- `addons/google_account/i18n/de.po` (72 lines)
- `addons/google_account/i18n/el.po` (65 lines)
- `addons/google_account/i18n/es.po` (73 lines)
- `addons/google_account/i18n/es_419.po` (70 lines)
- `addons/google_account/i18n/et.po` (67 lines)
- `addons/google_account/i18n/fa.po` (66 lines)
- `addons/google_account/i18n/fi.po` (71 lines)
- `addons/google_account/i18n/fr.po` (74 lines)
- `addons/google_account/i18n/google_account.pot` (58 lines)
- `addons/google_account/i18n/he.po` (68 lines)
- `addons/google_account/i18n/hi.po` (62 lines)
- `addons/google_account/i18n/hr.po` (67 lines)
- `addons/google_account/i18n/hu.po` (68 lines)
- `addons/google_account/i18n/id.po` (65 lines)
- `addons/google_account/i18n/it.po` (73 lines)
- `addons/google_account/i18n/ja.po` (69 lines)
- `addons/google_account/i18n/kab.po` (63 lines)
- `addons/google_account/i18n/ko.po` (66 lines)
- `addons/google_account/i18n/ku.po` (62 lines)
- `addons/google_account/i18n/lo.po` (61 lines)
- `addons/google_account/i18n/lt.po` (68 lines)
- `addons/google_account/i18n/lv.po` (61 lines)
- `addons/google_account/i18n/mn.po` (68 lines)
- `addons/google_account/i18n/my.po` (62 lines)
- `addons/google_account/i18n/nb.po` (65 lines)
- `addons/google_account/i18n/nl.po` (72 lines)
- `addons/google_account/i18n/pl.po` (72 lines)
- `addons/google_account/i18n/pt.po` (70 lines)
- `addons/google_account/i18n/pt_BR.po` (73 lines)
- `addons/google_account/i18n/ro.po` (69 lines)
- `addons/google_account/i18n/ru.po` (68 lines)
- `addons/google_account/i18n/sk.po` (67 lines)
- `addons/google_account/i18n/sl.po` (65 lines)
- `addons/google_account/i18n/sr@latin.po` (63 lines)
- `addons/google_account/i18n/sv.po` (69 lines)
- `addons/google_account/i18n/th.po` (63 lines)
- `addons/google_account/i18n/tr.po` (74 lines)
- `addons/google_account/i18n/uk.po` (70 lines)
- `addons/google_account/i18n/uz.po` (78 lines)
- `addons/google_account/i18n/vi.po` (69 lines)
- `addons/google_account/i18n/zh_CN.po` (69 lines)
- `addons/google_account/i18n/zh_TW.po` (65 lines)
- `addons/google_account/models/__init__.py` (4 lines)
- `addons/google_account/models/google_service.py` (162 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
