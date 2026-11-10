# Module: mass_mailing_crm_sms

- **Module ID:** MOD-364
- **Path:** `addons/mass_mailing_crm_sms`
- **Manifest:** `addons/mass_mailing_crm_sms/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Add lead / opportunities info on mass mailing sms

Mass mailing sms on lead / opportunities

Declared dependencies: `mass_mailing_crm`, `mass_mailing_sms`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
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
    "mass_mailing_crm",
    "mass_mailing_sms"
  ]
}
```

### Representative source files

- `addons/mass_mailing_crm_sms/__init__.py` (4 lines)
- `addons/mass_mailing_crm_sms/__manifest__.py` (12 lines)
- `addons/mass_mailing_crm_sms/i18n/ar.po` (58 lines)
- `addons/mass_mailing_crm_sms/i18n/az.po` (55 lines)
- `addons/mass_mailing_crm_sms/i18n/bg.po` (55 lines)
- `addons/mass_mailing_crm_sms/i18n/bs.po` (57 lines)
- `addons/mass_mailing_crm_sms/i18n/ca.po` (56 lines)
- `addons/mass_mailing_crm_sms/i18n/cs.po` (57 lines)
- `addons/mass_mailing_crm_sms/i18n/da.po` (57 lines)
- `addons/mass_mailing_crm_sms/i18n/de.po` (58 lines)
- `addons/mass_mailing_crm_sms/i18n/el.po` (56 lines)
- `addons/mass_mailing_crm_sms/i18n/es.po` (58 lines)
- `addons/mass_mailing_crm_sms/i18n/es_419.po` (57 lines)
- `addons/mass_mailing_crm_sms/i18n/et.po` (55 lines)
- `addons/mass_mailing_crm_sms/i18n/fa.po` (55 lines)
- `addons/mass_mailing_crm_sms/i18n/fi.po` (57 lines)
- `addons/mass_mailing_crm_sms/i18n/fr.po` (57 lines)
- `addons/mass_mailing_crm_sms/i18n/he.po` (56 lines)
- `addons/mass_mailing_crm_sms/i18n/hi.po` (55 lines)
- `addons/mass_mailing_crm_sms/i18n/hr.po` (56 lines)
- `addons/mass_mailing_crm_sms/i18n/hu.po` (56 lines)
- `addons/mass_mailing_crm_sms/i18n/id.po` (57 lines)
- `addons/mass_mailing_crm_sms/i18n/it.po` (57 lines)
- `addons/mass_mailing_crm_sms/i18n/ja.po` (57 lines)
- `addons/mass_mailing_crm_sms/i18n/kab.po` (56 lines)
- `addons/mass_mailing_crm_sms/i18n/ko.po` (57 lines)
- `addons/mass_mailing_crm_sms/i18n/ku.po` (55 lines)
- `addons/mass_mailing_crm_sms/i18n/lo.po` (55 lines)
- `addons/mass_mailing_crm_sms/i18n/lt.po` (57 lines)
- `addons/mass_mailing_crm_sms/i18n/lv.po` (56 lines)
- `addons/mass_mailing_crm_sms/i18n/mass_mailing_crm_sms.pot` (52 lines)
- `addons/mass_mailing_crm_sms/i18n/mn.po` (55 lines)
- `addons/mass_mailing_crm_sms/i18n/my.po` (55 lines)
- `addons/mass_mailing_crm_sms/i18n/nb.po` (56 lines)
- `addons/mass_mailing_crm_sms/i18n/nl.po` (57 lines)
- `addons/mass_mailing_crm_sms/i18n/pl.po` (58 lines)
- `addons/mass_mailing_crm_sms/i18n/pt.po` (56 lines)
- `addons/mass_mailing_crm_sms/i18n/pt_BR.po` (59 lines)
- `addons/mass_mailing_crm_sms/i18n/ro.po` (57 lines)
- `addons/mass_mailing_crm_sms/i18n/ru.po` (59 lines)
- `addons/mass_mailing_crm_sms/i18n/sk.po` (55 lines)
- `addons/mass_mailing_crm_sms/i18n/sl.po` (57 lines)
- `addons/mass_mailing_crm_sms/i18n/sr@latin.po` (56 lines)
- `addons/mass_mailing_crm_sms/i18n/sv.po` (57 lines)
- `addons/mass_mailing_crm_sms/i18n/th.po` (57 lines)
- `addons/mass_mailing_crm_sms/i18n/tr.po` (57 lines)
- `addons/mass_mailing_crm_sms/i18n/uk.po` (56 lines)
- `addons/mass_mailing_crm_sms/i18n/uz.po` (68 lines)
- `addons/mass_mailing_crm_sms/i18n/vi.po` (57 lines)
- `addons/mass_mailing_crm_sms/i18n/zh_CN.po` (57 lines)
- `addons/mass_mailing_crm_sms/i18n/zh_TW.po` (59 lines)
- `addons/mass_mailing_crm_sms/models/__init__.py` (4 lines)
- `addons/mass_mailing_crm_sms/models/utm.py` (10 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
