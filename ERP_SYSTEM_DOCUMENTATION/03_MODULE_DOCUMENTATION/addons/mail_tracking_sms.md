# Module: mail_tracking_sms

- **Module ID:** MOD-358
- **Path:** `addons/mail_tracking_sms`
- **Manifest:** `addons/mail_tracking_sms/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Track source of messages by sms

No manifest description declared.

Declared dependencies: `mail_tracking`, `sms`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mail_tracking",
    "sms"
  ],
  "data": [
    "views/mail_message_views.xml"
  ]
}
```

### Representative source files

- `addons/mail_tracking_sms/__init__.py` (2 lines)
- `addons/mail_tracking_sms/__manifest__.py` (15 lines)
- `addons/mail_tracking_sms/i18n/ar.po` (72 lines)
- `addons/mail_tracking_sms/i18n/az.po` (72 lines)
- `addons/mail_tracking_sms/i18n/bg.po` (72 lines)
- `addons/mail_tracking_sms/i18n/bs.po` (72 lines)
- `addons/mail_tracking_sms/i18n/ca.po` (72 lines)
- `addons/mail_tracking_sms/i18n/cs.po` (72 lines)
- `addons/mail_tracking_sms/i18n/da.po` (72 lines)
- `addons/mail_tracking_sms/i18n/de.po` (76 lines)
- `addons/mail_tracking_sms/i18n/el.po` (72 lines)
- `addons/mail_tracking_sms/i18n/es.po` (76 lines)
- `addons/mail_tracking_sms/i18n/es_419.po` (72 lines)
- `addons/mail_tracking_sms/i18n/et.po` (72 lines)
- `addons/mail_tracking_sms/i18n/fa.po` (72 lines)
- `addons/mail_tracking_sms/i18n/fi.po` (76 lines)
- `addons/mail_tracking_sms/i18n/fr.po` (72 lines)
- `addons/mail_tracking_sms/i18n/he.po` (72 lines)
- `addons/mail_tracking_sms/i18n/hi.po` (72 lines)
- `addons/mail_tracking_sms/i18n/hr.po` (72 lines)
- `addons/mail_tracking_sms/i18n/hu.po` (72 lines)
- `addons/mail_tracking_sms/i18n/id.po` (72 lines)
- `addons/mail_tracking_sms/i18n/it.po` (76 lines)
- `addons/mail_tracking_sms/i18n/ja.po` (72 lines)
- `addons/mail_tracking_sms/i18n/kab.po` (72 lines)
- `addons/mail_tracking_sms/i18n/ko.po` (72 lines)
- `addons/mail_tracking_sms/i18n/ku.po` (72 lines)
- `addons/mail_tracking_sms/i18n/lo.po` (72 lines)
- `addons/mail_tracking_sms/i18n/lt.po` (72 lines)
- `addons/mail_tracking_sms/i18n/lv.po` (72 lines)
- `addons/mail_tracking_sms/i18n/mail_tracking_sms.pot` (72 lines)
- `addons/mail_tracking_sms/i18n/mn.po` (72 lines)
- `addons/mail_tracking_sms/i18n/my.po` (72 lines)
- `addons/mail_tracking_sms/i18n/nb.po` (72 lines)
- `addons/mail_tracking_sms/i18n/nl.po` (76 lines)
- `addons/mail_tracking_sms/i18n/pl.po` (72 lines)
- `addons/mail_tracking_sms/i18n/pt.po` (72 lines)
- `addons/mail_tracking_sms/i18n/pt_BR.po` (77 lines)
- `addons/mail_tracking_sms/i18n/ro.po` (72 lines)
- `addons/mail_tracking_sms/i18n/ru.po` (77 lines)
- `addons/mail_tracking_sms/i18n/sk.po` (72 lines)
- `addons/mail_tracking_sms/i18n/sl.po` (72 lines)
- `addons/mail_tracking_sms/i18n/sr@latin.po` (72 lines)
- `addons/mail_tracking_sms/i18n/sv.po` (76 lines)
- `addons/mail_tracking_sms/i18n/th.po` (72 lines)
- `addons/mail_tracking_sms/i18n/tr.po` (72 lines)
- `addons/mail_tracking_sms/i18n/uk.po` (72 lines)
- `addons/mail_tracking_sms/i18n/uz.po` (72 lines)
- `addons/mail_tracking_sms/i18n/vi.po` (72 lines)
- `addons/mail_tracking_sms/i18n/zh_CN.po` (72 lines)
- `addons/mail_tracking_sms/i18n/zh_TW.po` (72 lines)
- `addons/mail_tracking_sms/models/__init__.py` (2 lines)
- `addons/mail_tracking_sms/models/mail_message.py` (11 lines)
- `addons/mail_tracking_sms/models/mail_thread.py` (15 lines)
- `addons/mail_tracking_sms/views/mail_message_views.xml` (37 lines)
- `addons/mail_tracking_sms/wizard/__init__.py` (1 lines)
- `addons/mail_tracking_sms/wizard/sms_composer.py` (15 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
