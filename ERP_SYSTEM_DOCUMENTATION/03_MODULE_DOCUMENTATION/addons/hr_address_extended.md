# Module: hr_address_extended

- **Module ID:** MOD-082
- **Path:** `addons/hr_address_extended`
- **Manifest:** `addons/hr_address_extended/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Centralize employee information

No manifest description declared.

Declared dependencies: `hr`, `base_address_extended`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "hr",
    "base_address_extended"
  ],
  "data": [
    "views/hr_employee_views.xml"
  ]
}
```

### Representative source files

- `addons/hr_address_extended/__init__.py` (2 lines)
- `addons/hr_address_extended/__manifest__.py` (18 lines)
- `addons/hr_address_extended/i18n/ar.po` (77 lines)
- `addons/hr_address_extended/i18n/az.po` (76 lines)
- `addons/hr_address_extended/i18n/bg.po` (76 lines)
- `addons/hr_address_extended/i18n/bs.po` (77 lines)
- `addons/hr_address_extended/i18n/ca.po` (76 lines)
- `addons/hr_address_extended/i18n/cs.po` (76 lines)
- `addons/hr_address_extended/i18n/da.po` (76 lines)
- `addons/hr_address_extended/i18n/de.po` (80 lines)
- `addons/hr_address_extended/i18n/el.po` (76 lines)
- `addons/hr_address_extended/i18n/es.po` (77 lines)
- `addons/hr_address_extended/i18n/es_419.po` (79 lines)
- `addons/hr_address_extended/i18n/et.po` (76 lines)
- `addons/hr_address_extended/i18n/fa.po` (76 lines)
- `addons/hr_address_extended/i18n/fi.po` (77 lines)
- `addons/hr_address_extended/i18n/fr.po` (80 lines)
- `addons/hr_address_extended/i18n/he.po` (77 lines)
- `addons/hr_address_extended/i18n/hi.po` (76 lines)
- `addons/hr_address_extended/i18n/hr.po` (77 lines)
- `addons/hr_address_extended/i18n/hr_address_extended.pot` (73 lines)
- `addons/hr_address_extended/i18n/hu.po` (76 lines)
- `addons/hr_address_extended/i18n/id.po` (76 lines)
- `addons/hr_address_extended/i18n/it.po` (79 lines)
- `addons/hr_address_extended/i18n/ja.po` (79 lines)
- `addons/hr_address_extended/i18n/kab.po` (76 lines)
- `addons/hr_address_extended/i18n/ko.po` (76 lines)
- `addons/hr_address_extended/i18n/ku.po` (76 lines)
- `addons/hr_address_extended/i18n/lo.po` (76 lines)
- `addons/hr_address_extended/i18n/lt.po` (78 lines)
- `addons/hr_address_extended/i18n/lv.po` (77 lines)
- `addons/hr_address_extended/i18n/mn.po` (80 lines)
- `addons/hr_address_extended/i18n/my.po` (76 lines)
- `addons/hr_address_extended/i18n/nb.po` (76 lines)
- `addons/hr_address_extended/i18n/nl.po` (79 lines)
- `addons/hr_address_extended/i18n/pl.po` (77 lines)
- `addons/hr_address_extended/i18n/pt.po` (76 lines)
- `addons/hr_address_extended/i18n/pt_BR.po` (81 lines)
- `addons/hr_address_extended/i18n/ro.po` (77 lines)
- `addons/hr_address_extended/i18n/ru.po` (77 lines)
- `addons/hr_address_extended/i18n/sk.po` (76 lines)
- `addons/hr_address_extended/i18n/sl.po` (77 lines)
- `addons/hr_address_extended/i18n/sr@latin.po` (78 lines)
- `addons/hr_address_extended/i18n/sv.po` (77 lines)
- `addons/hr_address_extended/i18n/th.po` (79 lines)
- `addons/hr_address_extended/i18n/tr.po` (79 lines)
- `addons/hr_address_extended/i18n/uk.po` (77 lines)
- `addons/hr_address_extended/i18n/uz.po` (76 lines)
- `addons/hr_address_extended/i18n/vi.po` (76 lines)
- `addons/hr_address_extended/i18n/zh_CN.po` (78 lines)
- `addons/hr_address_extended/i18n/zh_TW.po` (76 lines)
- `addons/hr_address_extended/models/__init__.py` (2 lines)
- `addons/hr_address_extended/models/hr_employee.py` (9 lines)
- `addons/hr_address_extended/models/hr_version.py` (28 lines)
- `addons/hr_address_extended/tests/__init__.py` (1 lines)
- `addons/hr_address_extended/tests/test_hr_version.py` (52 lines)
- `addons/hr_address_extended/views/hr_employee_views.xml` (25 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
