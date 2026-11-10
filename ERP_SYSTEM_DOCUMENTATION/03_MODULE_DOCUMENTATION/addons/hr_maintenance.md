# Module: hr_maintenance

- **Module ID:** MOD-092
- **Path:** `addons/hr_maintenance`
- **Manifest:** `addons/hr_maintenance/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Equipment, Assets, Internal Hardware, Allocation Tracking


Bridge between HR and Maintenance.

Declared dependencies: `hr`, `maintenance`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "hr",
    "maintenance"
  ],
  "data": [
    "security/equipment.xml",
    "views/maintenance_views.xml",
    "views/hr_views.xml"
  ]
}
```

### Representative source files

- `addons/hr_maintenance/__init__.py` (3 lines)
- `addons/hr_maintenance/__manifest__.py` (18 lines)
- `addons/hr_maintenance/i18n/af.po` (158 lines)
- `addons/hr_maintenance/i18n/ar.po` (163 lines)
- `addons/hr_maintenance/i18n/az.po` (161 lines)
- `addons/hr_maintenance/i18n/bg.po` (164 lines)
- `addons/hr_maintenance/i18n/bs.po` (161 lines)
- `addons/hr_maintenance/i18n/ca.po` (165 lines)
- `addons/hr_maintenance/i18n/cs.po` (167 lines)
- `addons/hr_maintenance/i18n/da.po` (162 lines)
- `addons/hr_maintenance/i18n/de.po` (167 lines)
- `addons/hr_maintenance/i18n/el.po` (161 lines)
- `addons/hr_maintenance/i18n/es.po` (165 lines)
- `addons/hr_maintenance/i18n/es_419.po` (161 lines)
- `addons/hr_maintenance/i18n/et.po` (166 lines)
- `addons/hr_maintenance/i18n/fa.po` (165 lines)
- `addons/hr_maintenance/i18n/fi.po` (167 lines)
- `addons/hr_maintenance/i18n/fr.po` (166 lines)
- `addons/hr_maintenance/i18n/gu.po` (158 lines)
- `addons/hr_maintenance/i18n/he.po` (165 lines)
- `addons/hr_maintenance/i18n/hi.po` (157 lines)
- `addons/hr_maintenance/i18n/hr.po` (165 lines)
- `addons/hr_maintenance/i18n/hr_maintenance.pot` (154 lines)
- `addons/hr_maintenance/i18n/hu.po` (165 lines)
- `addons/hr_maintenance/i18n/id.po` (164 lines)
- `addons/hr_maintenance/i18n/is.po` (158 lines)
- `addons/hr_maintenance/i18n/it.po` (169 lines)
- `addons/hr_maintenance/i18n/ja.po` (163 lines)
- `addons/hr_maintenance/i18n/kab.po` (157 lines)
- `addons/hr_maintenance/i18n/km.po` (158 lines)
- `addons/hr_maintenance/i18n/ko.po` (164 lines)
- `addons/hr_maintenance/i18n/ku.po` (157 lines)
- `addons/hr_maintenance/i18n/lo.po` (162 lines)
- `addons/hr_maintenance/i18n/lt.po` (166 lines)
- `addons/hr_maintenance/i18n/lv.po` (162 lines)
- `addons/hr_maintenance/i18n/mn.po` (162 lines)
- `addons/hr_maintenance/i18n/my.po` (159 lines)
- `addons/hr_maintenance/i18n/nb.po` (161 lines)
- `addons/hr_maintenance/i18n/nl.po` (164 lines)
- `addons/hr_maintenance/i18n/pl.po` (173 lines)
- `addons/hr_maintenance/i18n/pt.po` (168 lines)
- `addons/hr_maintenance/i18n/pt_BR.po` (171 lines)
- `addons/hr_maintenance/i18n/ro.po` (163 lines)
- `addons/hr_maintenance/i18n/ru.po` (162 lines)
- `addons/hr_maintenance/i18n/sk.po` (164 lines)
- `addons/hr_maintenance/i18n/sl.po` (162 lines)
- `addons/hr_maintenance/i18n/sr@latin.po` (162 lines)
- `addons/hr_maintenance/i18n/sv.po` (166 lines)
- `addons/hr_maintenance/i18n/th.po` (164 lines)
- `addons/hr_maintenance/i18n/tr.po` (166 lines)
- `addons/hr_maintenance/i18n/uk.po` (164 lines)
- `addons/hr_maintenance/i18n/uz.po` (180 lines)
- `addons/hr_maintenance/i18n/vi.po` (161 lines)
- `addons/hr_maintenance/i18n/zh_CN.po` (165 lines)
- `addons/hr_maintenance/i18n/zh_TW.po` (162 lines)
- `addons/hr_maintenance/models/__init__.py` (6 lines)
- `addons/hr_maintenance/models/equipment.py` (140 lines)
- `addons/hr_maintenance/models/hr_employee.py` (13 lines)
- `addons/hr_maintenance/models/hr_employee_departure.py` (30 lines)
- `addons/hr_maintenance/models/hr_employee_public.py` (9 lines)
- `addons/hr_maintenance/security/equipment.xml` (8 lines)
- `addons/hr_maintenance/tests/__init__.py` (3 lines)
- `addons/hr_maintenance/tests/test_employee_departure_maintenance.py` (29 lines)
- `addons/hr_maintenance/views/hr_views.xml` (47 lines)
- `addons/hr_maintenance/views/maintenance_views.xml` (129 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
