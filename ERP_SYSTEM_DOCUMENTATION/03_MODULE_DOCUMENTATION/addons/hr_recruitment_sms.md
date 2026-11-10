# Module: hr_recruitment_sms

- **Module ID:** MOD-096
- **Path:** `addons/hr_recruitment_sms`
- **Manifest:** `addons/hr_recruitment_sms/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Mass mailing sms to job applicants

Mass mailing sms to job applicants

Declared dependencies: `hr_recruitment`, `sms`.

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
    "hr_recruitment",
    "sms"
  ],
  "data": [
    "views/hr_applicant_views.xml",
    "views/res_config_settings_views.xml"
  ]
}
```

### Representative source files

- `addons/hr_recruitment_sms/__init__.py` (3 lines)
- `addons/hr_recruitment_sms/__manifest__.py` (15 lines)
- `addons/hr_recruitment_sms/i18n/ar.po` (58 lines)
- `addons/hr_recruitment_sms/i18n/az.po` (60 lines)
- `addons/hr_recruitment_sms/i18n/bg.po` (60 lines)
- `addons/hr_recruitment_sms/i18n/bs.po` (60 lines)
- `addons/hr_recruitment_sms/i18n/ca.po` (61 lines)
- `addons/hr_recruitment_sms/i18n/cs.po` (61 lines)
- `addons/hr_recruitment_sms/i18n/da.po` (60 lines)
- `addons/hr_recruitment_sms/i18n/de.po` (56 lines)
- `addons/hr_recruitment_sms/i18n/el.po` (60 lines)
- `addons/hr_recruitment_sms/i18n/es.po` (56 lines)
- `addons/hr_recruitment_sms/i18n/es_419.po` (57 lines)
- `addons/hr_recruitment_sms/i18n/et.po` (61 lines)
- `addons/hr_recruitment_sms/i18n/fa.po` (60 lines)
- `addons/hr_recruitment_sms/i18n/fi.po` (56 lines)
- `addons/hr_recruitment_sms/i18n/fr.po` (56 lines)
- `addons/hr_recruitment_sms/i18n/he.po` (61 lines)
- `addons/hr_recruitment_sms/i18n/hi.po` (61 lines)
- `addons/hr_recruitment_sms/i18n/hr.po` (61 lines)
- `addons/hr_recruitment_sms/i18n/hr_recruitment_sms.pot` (52 lines)
- `addons/hr_recruitment_sms/i18n/hu.po` (60 lines)
- `addons/hr_recruitment_sms/i18n/id.po` (56 lines)
- `addons/hr_recruitment_sms/i18n/it.po` (56 lines)
- `addons/hr_recruitment_sms/i18n/ja.po` (56 lines)
- `addons/hr_recruitment_sms/i18n/kab.po` (60 lines)
- `addons/hr_recruitment_sms/i18n/ko.po` (56 lines)
- `addons/hr_recruitment_sms/i18n/ku.po` (57 lines)
- `addons/hr_recruitment_sms/i18n/lo.po` (61 lines)
- `addons/hr_recruitment_sms/i18n/lt.po` (62 lines)
- `addons/hr_recruitment_sms/i18n/lv.po` (61 lines)
- `addons/hr_recruitment_sms/i18n/mn.po` (60 lines)
- `addons/hr_recruitment_sms/i18n/my.po` (60 lines)
- `addons/hr_recruitment_sms/i18n/nb.po` (60 lines)
- `addons/hr_recruitment_sms/i18n/nl.po` (57 lines)
- `addons/hr_recruitment_sms/i18n/pl.po` (57 lines)
- `addons/hr_recruitment_sms/i18n/pt.po` (61 lines)
- `addons/hr_recruitment_sms/i18n/pt_BR.po` (57 lines)
- `addons/hr_recruitment_sms/i18n/ro.po` (58 lines)
- `addons/hr_recruitment_sms/i18n/ru.po` (58 lines)
- `addons/hr_recruitment_sms/i18n/sk.po` (60 lines)
- `addons/hr_recruitment_sms/i18n/sl.po` (62 lines)
- `addons/hr_recruitment_sms/i18n/sr@latin.po` (61 lines)
- `addons/hr_recruitment_sms/i18n/sv.po` (56 lines)
- `addons/hr_recruitment_sms/i18n/th.po` (59 lines)
- `addons/hr_recruitment_sms/i18n/tr.po` (56 lines)
- `addons/hr_recruitment_sms/i18n/uk.po` (61 lines)
- `addons/hr_recruitment_sms/i18n/uz.po` (68 lines)
- `addons/hr_recruitment_sms/i18n/vi.po` (60 lines)
- `addons/hr_recruitment_sms/i18n/zh_CN.po` (56 lines)
- `addons/hr_recruitment_sms/i18n/zh_TW.po` (59 lines)
- `addons/hr_recruitment_sms/models/__init__.py` (3 lines)
- `addons/hr_recruitment_sms/models/hr_applicant.py` (16 lines)
- `addons/hr_recruitment_sms/views/hr_applicant_views.xml` (12 lines)
- `addons/hr_recruitment_sms/views/res_config_settings_views.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
