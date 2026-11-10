# Module: iap_mail

- **Module ID:** MOD-110
- **Path:** `addons/iap_mail`
- **Manifest:** `addons/iap_mail/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Bridge between IAP and mail

Bridge between IAP and mail

Declared dependencies: `iap`, `mail`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "iap",
    "mail"
  ],
  "data": [
    "data/mail_templates.xml",
    "views/iap_views.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "iap_mail/static/src/js/**/*",
      "iap_mail/static/src/scss/iap_mail.scss"
    ],
    "web.dark_mode_assets_backend": [
      "iap_mail/static/src/scss/iap_mail.dark.scss"
    ]
  }
}
```

### Representative source files

- `addons/iap_mail/__init__.py` (3 lines)
- `addons/iap_mail/__manifest__.py` (29 lines)
- `addons/iap_mail/data/mail_templates.xml` (201 lines)
- `addons/iap_mail/i18n/ar.po` (316 lines)
- `addons/iap_mail/i18n/az.po` (285 lines)
- `addons/iap_mail/i18n/bg.po` (285 lines)
- `addons/iap_mail/i18n/bs.po` (287 lines)
- `addons/iap_mail/i18n/ca.po` (311 lines)
- `addons/iap_mail/i18n/cs.po` (293 lines)
- `addons/iap_mail/i18n/da.po` (288 lines)
- `addons/iap_mail/i18n/de.po` (337 lines)
- `addons/iap_mail/i18n/el.po` (286 lines)
- `addons/iap_mail/i18n/es.po` (316 lines)
- `addons/iap_mail/i18n/es_419.po` (339 lines)
- `addons/iap_mail/i18n/et.po` (285 lines)
- `addons/iap_mail/i18n/fa.po` (285 lines)
- `addons/iap_mail/i18n/fi.po` (311 lines)
- `addons/iap_mail/i18n/fr.po` (338 lines)
- `addons/iap_mail/i18n/he.po` (286 lines)
- `addons/iap_mail/i18n/hi.po` (285 lines)
- `addons/iap_mail/i18n/hr.po` (286 lines)
- `addons/iap_mail/i18n/hu.po` (286 lines)
- `addons/iap_mail/i18n/iap_mail.pot` (277 lines)
- `addons/iap_mail/i18n/id.po` (321 lines)
- `addons/iap_mail/i18n/it.po` (338 lines)
- `addons/iap_mail/i18n/ja.po` (334 lines)
- `addons/iap_mail/i18n/kab.po` (286 lines)
- `addons/iap_mail/i18n/ko.po` (314 lines)
- `addons/iap_mail/i18n/ku.po` (285 lines)
- `addons/iap_mail/i18n/lo.po` (328 lines)
- `addons/iap_mail/i18n/lt.po` (287 lines)
- `addons/iap_mail/i18n/lv.po` (286 lines)
- `addons/iap_mail/i18n/mn.po` (285 lines)
- `addons/iap_mail/i18n/my.po` (285 lines)
- `addons/iap_mail/i18n/nb.po` (289 lines)
- `addons/iap_mail/i18n/nl.po` (335 lines)
- `addons/iap_mail/i18n/pl.po` (338 lines)
- `addons/iap_mail/i18n/pt.po` (310 lines)
- `addons/iap_mail/i18n/pt_BR.po` (343 lines)
- `addons/iap_mail/i18n/ro.po` (288 lines)
- `addons/iap_mail/i18n/ru.po` (315 lines)
- `addons/iap_mail/i18n/sk.po` (285 lines)
- `addons/iap_mail/i18n/sl.po` (311 lines)
- `addons/iap_mail/i18n/sr@latin.po` (286 lines)
- `addons/iap_mail/i18n/sv.po` (313 lines)
- `addons/iap_mail/i18n/th.po` (311 lines)
- `addons/iap_mail/i18n/tr.po` (317 lines)
- `addons/iap_mail/i18n/uk.po` (286 lines)
- `addons/iap_mail/i18n/uz.po` (316 lines)
- `addons/iap_mail/i18n/vi.po` (314 lines)
- `addons/iap_mail/i18n/zh_CN.po` (335 lines)
- `addons/iap_mail/i18n/zh_TW.po` (313 lines)
- `addons/iap_mail/models/__init__.py` (4 lines)
- `addons/iap_mail/models/iap_account.py` (40 lines)
- `addons/iap_mail/static/src/js/services/iap_notification_service.js` (40 lines)
- `addons/iap_mail/static/src/scss/iap_mail.dark.scss` (3 lines)
- `addons/iap_mail/static/src/scss/iap_mail.scss` (4 lines)
- `addons/iap_mail/views/iap_views.xml` (15 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
