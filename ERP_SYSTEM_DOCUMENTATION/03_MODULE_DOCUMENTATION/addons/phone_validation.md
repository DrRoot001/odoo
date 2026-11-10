# Module: phone_validation

- **Module ID:** MOD-416
- **Path:** `addons/phone_validation`
- **Manifest:** `addons/phone_validation/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Validate and format phone numbers


Phone Numbers Validation
========================

This module adds the feature of validation and formatting phone numbers
according to a destination country.

It also adds phone blacklist management through a specific model storing
blacklisted phone numbers.

It adds mail.thread.phone mixin that handles sanitation and blacklist of
records numbers. 

Declared dependencies: `base`, `mail`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 32 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 8 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base",
    "mail"
  ],
  "data": [
    "views/phone_blacklist_views.xml",
    "views/res_partner_views.xml",
    "wizard/mail_activity_schedule_views.xml",
    "wizard/phone_blacklist_remove_view.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/phone_validation/__init__.py` (7 lines)
- `addons/phone_validation/__manifest__.py` (35 lines)
- `addons/phone_validation/i18n/ar.po` (495 lines)
- `addons/phone_validation/i18n/az.po` (489 lines)
- `addons/phone_validation/i18n/bg.po` (486 lines)
- `addons/phone_validation/i18n/bs.po` (482 lines)
- `addons/phone_validation/i18n/ca.po` (500 lines)
- `addons/phone_validation/i18n/cs.po` (495 lines)
- `addons/phone_validation/i18n/da.po` (488 lines)
- `addons/phone_validation/i18n/de.po` (521 lines)
- `addons/phone_validation/i18n/el.po` (482 lines)
- `addons/phone_validation/i18n/es.po` (513 lines)
- `addons/phone_validation/i18n/es_419.po` (507 lines)
- `addons/phone_validation/i18n/et.po` (499 lines)
- `addons/phone_validation/i18n/fa.po` (495 lines)
- `addons/phone_validation/i18n/fi.po` (507 lines)
- `addons/phone_validation/i18n/fr.po` (503 lines)
- `addons/phone_validation/i18n/gu.po` (452 lines)
- `addons/phone_validation/i18n/he.po` (499 lines)
- `addons/phone_validation/i18n/hi.po` (478 lines)
- `addons/phone_validation/i18n/hr.po` (488 lines)
- `addons/phone_validation/i18n/hu.po` (486 lines)
- `addons/phone_validation/i18n/id.po` (498 lines)
- `addons/phone_validation/i18n/is.po` (448 lines)
- `addons/phone_validation/i18n/it.po` (513 lines)
- `addons/phone_validation/i18n/ja.po` (495 lines)
- `addons/phone_validation/i18n/kab.po` (478 lines)
- `addons/phone_validation/i18n/km.po` (451 lines)
- `addons/phone_validation/i18n/ko.po` (492 lines)
- `addons/phone_validation/i18n/ku.po` (478 lines)
- `addons/phone_validation/i18n/lo.po` (498 lines)
- `addons/phone_validation/i18n/lt.po` (492 lines)
- `addons/phone_validation/i18n/lv.po` (483 lines)
- `addons/phone_validation/i18n/mn.po` (486 lines)
- `addons/phone_validation/i18n/my.po` (479 lines)
- `addons/phone_validation/i18n/nb.po` (486 lines)
- `addons/phone_validation/i18n/nl.po` (497 lines)
- `addons/phone_validation/i18n/phone_validation.pot` (474 lines)
- `addons/phone_validation/i18n/pl.po` (511 lines)
- `addons/phone_validation/i18n/pt.po` (503 lines)
- `addons/phone_validation/i18n/pt_BR.po` (519 lines)
- `addons/phone_validation/i18n/ro.po` (497 lines)
- `addons/phone_validation/i18n/ru.po` (499 lines)
- `addons/phone_validation/i18n/sk.po` (490 lines)
- `addons/phone_validation/i18n/sl.po` (495 lines)
- `addons/phone_validation/i18n/sr@latin.po` (490 lines)
- `addons/phone_validation/i18n/sv.po` (501 lines)
- `addons/phone_validation/i18n/th.po` (487 lines)
- `addons/phone_validation/i18n/tr.po` (513 lines)
- `addons/phone_validation/i18n/uk.po` (493 lines)
- `addons/phone_validation/i18n/uz.po` (563 lines)
- `addons/phone_validation/i18n/vi.po` (493 lines)
- `addons/phone_validation/i18n/zh_CN.po` (496 lines)
- `addons/phone_validation/i18n/zh_TW.po` (488 lines)
- `addons/phone_validation/lib/__init__.py` (4 lines)
- `addons/phone_validation/lib/phonemetadata.py` (8 lines)
- `addons/phone_validation/lib/phonenumbers_patch/__init__.py` (110 lines)
- `addons/phone_validation/lib/phonenumbers_patch/region_BR.py` (26 lines)
- `addons/phone_validation/lib/phonenumbers_patch/region_CI.py` (9 lines)
- `addons/phone_validation/lib/phonenumbers_patch/region_CO.py` (18 lines)
- `addons/phone_validation/lib/phonenumbers_patch/region_IL.py` (25 lines)
- `addons/phone_validation/lib/phonenumbers_patch/region_KE.py` (15 lines)
- `addons/phone_validation/lib/phonenumbers_patch/region_MA.py` (18 lines)
- `addons/phone_validation/lib/phonenumbers_patch/region_MU.py` (14 lines)
- `addons/phone_validation/lib/phonenumbers_patch/region_PA.py` (13 lines)
- `addons/phone_validation/lib/phonenumbers_patch/region_SN.py` (13 lines)
- `addons/phone_validation/models/__init__.py` (10 lines)
- `addons/phone_validation/models/mail_activity.py` (15 lines)
- `addons/phone_validation/models/mail_activity_mixin.py` (26 lines)
- `addons/phone_validation/models/mail_thread_phone.py` (241 lines)
- `addons/phone_validation/models/models.py` (251 lines)
- `addons/phone_validation/models/phone_blacklist.py` (140 lines)
- `addons/phone_validation/models/res_partner.py` (8 lines)
- `addons/phone_validation/models/res_users.py` (32 lines)
- `addons/phone_validation/security/ir.access.csv` (3 lines)
- `addons/phone_validation/tests/__init__.py` (7 lines)
- `addons/phone_validation/tests/test_mail_activity_schedule.py` (165 lines)
- `addons/phone_validation/tests/test_phonenumbers.py` (84 lines)
- `addons/phone_validation/tests/test_phonenumbers_blacklist.py` (33 lines)
- `addons/phone_validation/tests/test_phonenumbers_patch.py` (193 lines)
- `addons/phone_validation/tools/__init__.py` (4 lines)
- `addons/phone_validation/tools/phone_validation.py` (135 lines)
- `addons/phone_validation/views/phone_blacklist_views.xml` (75 lines)
- `addons/phone_validation/views/res_partner_views.xml` (74 lines)
- `addons/phone_validation/wizard/__init__.py` (5 lines)
- `addons/phone_validation/wizard/mail_activity_schedule.py` (30 lines)
- `addons/phone_validation/wizard/mail_activity_schedule_views.xml` (19 lines)
- `addons/phone_validation/wizard/phone_blacklist_remove.py` (22 lines)
- `addons/phone_validation/wizard/phone_blacklist_remove_view.xml` (19 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
