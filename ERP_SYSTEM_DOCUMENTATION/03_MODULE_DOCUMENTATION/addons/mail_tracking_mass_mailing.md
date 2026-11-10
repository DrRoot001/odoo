# Module: mail_tracking_mass_mailing

- **Module ID:** MOD-357
- **Path:** `addons/mail_tracking_mass_mailing`
- **Manifest:** `addons/mail_tracking_mass_mailing/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Track source of messages by mass mailing

No manifest description declared.

Declared dependencies: `mail_tracking`, `mass_mailing`.

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
    "mass_mailing"
  ],
  "data": [
    "views/mail_message_views.xml"
  ]
}
```

### Representative source files

- `addons/mail_tracking_mass_mailing/__init__.py` (2 lines)
- `addons/mail_tracking_mass_mailing/__manifest__.py` (15 lines)
- `addons/mail_tracking_mass_mailing/i18n/ar.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/az.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/bg.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/bs.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/ca.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/cs.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/da.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/de.po` (80 lines)
- `addons/mail_tracking_mass_mailing/i18n/el.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/es.po` (80 lines)
- `addons/mail_tracking_mass_mailing/i18n/es_419.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/et.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/fa.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/fi.po` (80 lines)
- `addons/mail_tracking_mass_mailing/i18n/fr.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/he.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/hi.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/hr.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/hu.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/id.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/it.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/ja.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/kab.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/ko.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/ku.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/lo.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/lt.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/lv.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/mail_tracking_mass_mailing.pot` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/mn.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/my.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/nb.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/nl.po` (80 lines)
- `addons/mail_tracking_mass_mailing/i18n/pl.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/pt.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/pt_BR.po` (81 lines)
- `addons/mail_tracking_mass_mailing/i18n/ro.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/ru.po` (81 lines)
- `addons/mail_tracking_mass_mailing/i18n/sk.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/sl.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/sr@latin.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/sv.po` (80 lines)
- `addons/mail_tracking_mass_mailing/i18n/th.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/tr.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/uk.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/uz.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/vi.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/zh_CN.po` (76 lines)
- `addons/mail_tracking_mass_mailing/i18n/zh_TW.po` (76 lines)
- `addons/mail_tracking_mass_mailing/models/__init__.py` (2 lines)
- `addons/mail_tracking_mass_mailing/models/mail_message.py` (11 lines)
- `addons/mail_tracking_mass_mailing/models/mail_thread.py` (15 lines)
- `addons/mail_tracking_mass_mailing/views/mail_message_views.xml` (37 lines)
- `addons/mail_tracking_mass_mailing/wizard/__init__.py` (1 lines)
- `addons/mail_tracking_mass_mailing/wizard/mail_compose_message.py` (12 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
