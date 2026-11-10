# Module: mass_mailing_sale_sms

- **Module ID:** MOD-370
- **Path:** `addons/mass_mailing_sale_sms`
- **Manifest:** `addons/mass_mailing_sale_sms/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Add sale order info on mass mailing sms

Mass mailing sms on sale orders

Declared dependencies: `mass_mailing_sale`, `mass_mailing_sms`.

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
    "mass_mailing_sale",
    "mass_mailing_sms"
  ]
}
```

### Representative source files

- `addons/mass_mailing_sale_sms/__init__.py` (4 lines)
- `addons/mass_mailing_sale_sms/__manifest__.py` (12 lines)
- `addons/mass_mailing_sale_sms/i18n/ar.po` (63 lines)
- `addons/mass_mailing_sale_sms/i18n/az.po` (61 lines)
- `addons/mass_mailing_sale_sms/i18n/bg.po` (61 lines)
- `addons/mass_mailing_sale_sms/i18n/bs.po` (62 lines)
- `addons/mass_mailing_sale_sms/i18n/ca.po` (62 lines)
- `addons/mass_mailing_sale_sms/i18n/cs.po` (62 lines)
- `addons/mass_mailing_sale_sms/i18n/da.po` (63 lines)
- `addons/mass_mailing_sale_sms/i18n/de.po` (62 lines)
- `addons/mass_mailing_sale_sms/i18n/el.po` (62 lines)
- `addons/mass_mailing_sale_sms/i18n/es.po` (63 lines)
- `addons/mass_mailing_sale_sms/i18n/es_419.po` (62 lines)
- `addons/mass_mailing_sale_sms/i18n/et.po` (61 lines)
- `addons/mass_mailing_sale_sms/i18n/fa.po` (61 lines)
- `addons/mass_mailing_sale_sms/i18n/fi.po` (63 lines)
- `addons/mass_mailing_sale_sms/i18n/fr.po` (62 lines)
- `addons/mass_mailing_sale_sms/i18n/he.po` (62 lines)
- `addons/mass_mailing_sale_sms/i18n/hi.po` (61 lines)
- `addons/mass_mailing_sale_sms/i18n/hr.po` (62 lines)
- `addons/mass_mailing_sale_sms/i18n/hu.po` (62 lines)
- `addons/mass_mailing_sale_sms/i18n/id.po` (62 lines)
- `addons/mass_mailing_sale_sms/i18n/it.po` (63 lines)
- `addons/mass_mailing_sale_sms/i18n/ja.po` (62 lines)
- `addons/mass_mailing_sale_sms/i18n/kab.po` (61 lines)
- `addons/mass_mailing_sale_sms/i18n/ko.po` (62 lines)
- `addons/mass_mailing_sale_sms/i18n/ku.po` (61 lines)
- `addons/mass_mailing_sale_sms/i18n/lo.po` (60 lines)
- `addons/mass_mailing_sale_sms/i18n/lt.po` (63 lines)
- `addons/mass_mailing_sale_sms/i18n/lv.po` (61 lines)
- `addons/mass_mailing_sale_sms/i18n/mass_mailing_sale_sms.pot` (57 lines)
- `addons/mass_mailing_sale_sms/i18n/mn.po` (61 lines)
- `addons/mass_mailing_sale_sms/i18n/my.po` (61 lines)
- `addons/mass_mailing_sale_sms/i18n/nb.po` (62 lines)
- `addons/mass_mailing_sale_sms/i18n/nl.po` (62 lines)
- `addons/mass_mailing_sale_sms/i18n/pl.po` (63 lines)
- `addons/mass_mailing_sale_sms/i18n/pt.po` (63 lines)
- `addons/mass_mailing_sale_sms/i18n/pt_BR.po` (64 lines)
- `addons/mass_mailing_sale_sms/i18n/ro.po` (62 lines)
- `addons/mass_mailing_sale_sms/i18n/ru.po` (66 lines)
- `addons/mass_mailing_sale_sms/i18n/sk.po` (60 lines)
- `addons/mass_mailing_sale_sms/i18n/sl.po` (63 lines)
- `addons/mass_mailing_sale_sms/i18n/sr@latin.po` (62 lines)
- `addons/mass_mailing_sale_sms/i18n/sv.po` (63 lines)
- `addons/mass_mailing_sale_sms/i18n/th.po` (62 lines)
- `addons/mass_mailing_sale_sms/i18n/tr.po` (61 lines)
- `addons/mass_mailing_sale_sms/i18n/uk.po` (62 lines)
- `addons/mass_mailing_sale_sms/i18n/uz.po` (74 lines)
- `addons/mass_mailing_sale_sms/i18n/vi.po` (63 lines)
- `addons/mass_mailing_sale_sms/i18n/zh_CN.po` (62 lines)
- `addons/mass_mailing_sale_sms/i18n/zh_TW.po` (64 lines)
- `addons/mass_mailing_sale_sms/models/__init__.py` (4 lines)
- `addons/mass_mailing_sale_sms/models/utm.py` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
