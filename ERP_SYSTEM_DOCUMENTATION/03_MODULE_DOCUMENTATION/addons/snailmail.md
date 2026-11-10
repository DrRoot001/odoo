# Module: snailmail

- **Module ID:** MOD-541
- **Path:** `addons/snailmail`
- **Manifest:** `addons/snailmail/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Allows users to send documents by post
=====================================================
        

Declared dependencies: `iap_mail`, `mail`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 19 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 9 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 10 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "iap_mail",
    "mail"
  ],
  "data": [
    "data/iap_service_data.xml",
    "data/snailmail_data.xml",
    "views/report_assets.xml",
    "views/snailmail_views.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "snailmail/static/src/**/*"
    ],
    "snailmail.report_assets_snailmail": [
      [
        "include",
        "web._assets_helpers"
      ],
      "web/static/src/scss/pre_variables.scss",
      "web/static/lib/bootstrap/scss/_variables.scss",
      "web/static/lib/bootstrap/scss/_variables-dark.scss",
      "web/static/lib/bootstrap/scss/_maps.scss"
    ],
    "web.assets_unit_tests": [
      "snailmail/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/snailmail/__init__.py` (5 lines)
- `addons/snailmail/__manifest__.py` (38 lines)
- `addons/snailmail/controller/__init__.py` (1 lines)
- `addons/snailmail/controller/snailmail_webhook.py` (94 lines)
- `addons/snailmail/country_utils.py` (256 lines)
- `addons/snailmail/data/iap_service_data.xml` (12 lines)
- `addons/snailmail/data/snailmail_data.xml` (13 lines)
- `addons/snailmail/i18n/ar.po` (702 lines)
- `addons/snailmail/i18n/az.po` (667 lines)
- `addons/snailmail/i18n/bg.po` (664 lines)
- `addons/snailmail/i18n/bs.po` (669 lines)
- `addons/snailmail/i18n/ca.po` (706 lines)
- `addons/snailmail/i18n/cs.po` (702 lines)
- `addons/snailmail/i18n/da.po` (698 lines)
- `addons/snailmail/i18n/de.po` (720 lines)
- `addons/snailmail/i18n/el.po` (669 lines)
- `addons/snailmail/i18n/es.po` (711 lines)
- `addons/snailmail/i18n/es_419.po` (711 lines)
- `addons/snailmail/i18n/et.po` (677 lines)
- `addons/snailmail/i18n/fa.po` (704 lines)
- `addons/snailmail/i18n/fi.po` (706 lines)
- `addons/snailmail/i18n/fr.po` (710 lines)
- `addons/snailmail/i18n/gu.po` (610 lines)
- `addons/snailmail/i18n/he.po` (680 lines)
- `addons/snailmail/i18n/hi.po` (664 lines)
- `addons/snailmail/i18n/hr.po` (676 lines)
- `addons/snailmail/i18n/hu.po` (675 lines)
- `addons/snailmail/i18n/id.po` (697 lines)
- `addons/snailmail/i18n/is.po` (606 lines)
- `addons/snailmail/i18n/it.po` (707 lines)
- `addons/snailmail/i18n/ja.po` (700 lines)
- `addons/snailmail/i18n/kab.po` (664 lines)
- `addons/snailmail/i18n/km.po` (612 lines)
- `addons/snailmail/i18n/ko.po` (696 lines)
- `addons/snailmail/i18n/ku.po` (664 lines)
- `addons/snailmail/i18n/lo.po` (687 lines)
- `addons/snailmail/i18n/lt.po` (679 lines)
- `addons/snailmail/i18n/lv.po` (664 lines)
- `addons/snailmail/i18n/mn.po` (676 lines)
- `addons/snailmail/i18n/my.po` (665 lines)
- `addons/snailmail/i18n/nb.po` (669 lines)
- `addons/snailmail/i18n/nl.po` (720 lines)
- `addons/snailmail/i18n/pl.po` (719 lines)
- `addons/snailmail/i18n/pt.po` (710 lines)
- `addons/snailmail/i18n/pt_BR.po` (719 lines)
- `addons/snailmail/i18n/ro.po` (708 lines)
- `addons/snailmail/i18n/ru.po` (708 lines)
- `addons/snailmail/i18n/sk.po` (672 lines)
- `addons/snailmail/i18n/sl.po` (676 lines)
- `addons/snailmail/i18n/snailmail.pot` (657 lines)
- `addons/snailmail/i18n/sr@latin.po` (669 lines)
- `addons/snailmail/i18n/sv.po` (697 lines)
- `addons/snailmail/i18n/th.po` (695 lines)
- `addons/snailmail/i18n/tr.po` (711 lines)
- `addons/snailmail/i18n/uk.po` (699 lines)
- `addons/snailmail/i18n/uz.po` (801 lines)
- `addons/snailmail/i18n/vi.po` (699 lines)
- `addons/snailmail/i18n/zh_CN.po` (702 lines)
- `addons/snailmail/i18n/zh_TW.po` (693 lines)
- `addons/snailmail/models/__init__.py` (10 lines)
- `addons/snailmail/models/ir_actions_report.py` (21 lines)
- `addons/snailmail/models/mail_message.py` (31 lines)
- `addons/snailmail/models/mail_notification.py` (19 lines)
- `addons/snailmail/models/mail_thread.py` (25 lines)
- `addons/snailmail/models/res_company.py` (12 lines)
- `addons/snailmail/models/res_config_settings.py` (11 lines)
- `addons/snailmail/models/res_partner.py` (51 lines)
- `addons/snailmail/models/snailmail_letter.py` (596 lines)
- `addons/snailmail/security/ir.access.csv` (3 lines)
- `addons/snailmail/static/description/icon.png` (12 lines)
- `addons/snailmail/static/description/icon.svg` (1 lines)
- `addons/snailmail/static/description/icon_hi.png` (41 lines)
- `addons/snailmail/static/img/snailmail_failure.png` (62 lines)
- `addons/snailmail/static/src/core/failure_model_patch.js` (24 lines)
- `addons/snailmail/static/src/core/notification_model_patch.js` (77 lines)
- `addons/snailmail/static/src/core_ui/message_patch.js` (8 lines)
- `addons/snailmail/static/src/core_ui/snailmail_notification_popover.js` (5 lines)
- `addons/snailmail/static/src/core_ui/snailmail_notification_popover.xml` (17 lines)
- `addons/snailmail/static/src/messaging_menu/messaging_menu_patch.js` (36 lines)
- `addons/snailmail/static/tests/message/message_patch.test.js` (218 lines)
- `addons/snailmail/static/tests/messaging_menu/messaging_menu_patch.test.js` (152 lines)
- `addons/snailmail/static/tests/mock_server/mock_model/iap_account.js` (9 lines)
- `addons/snailmail/static/tests/mock_server/mock_model/snailmail_letter.js` (5 lines)
- `addons/snailmail/static/tests/snailmail_test_helpers.js` (10 lines)
- `addons/snailmail/tests/__init__.py` (7 lines)
- `addons/snailmail/tests/common.py` (77 lines)
- `addons/snailmail/tests/test_attachment_access.py` (132 lines)
- `addons/snailmail/tests/test_snailmail_letter.py` (39 lines)
- `addons/snailmail/tests/test_snailmail_webhook.py` (127 lines)
- `addons/snailmail/views/report_assets.xml` (13 lines)
- `addons/snailmail/views/snailmail_views.xml` (62 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
