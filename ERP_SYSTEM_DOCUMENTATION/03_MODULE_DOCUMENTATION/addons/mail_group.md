# Module: mail_group

- **Module ID:** MOD-354
- **Path:** `addons/mail_group`
- **Manifest:** `addons/mail_group/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Manage your mailing lists


Manage your mailing lists from Odoo.
    

Declared dependencies: `mail`, `portal`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 18 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 14 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 7 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 9 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mail",
    "portal"
  ],
  "data": [
    "data/ir_cron_data.xml",
    "data/mail_templates.xml",
    "data/mail_template_data.xml",
    "data/mail_template_email_layouts.xml",
    "data/res_groups.xml",
    "wizard/mail_group_message_reject_views.xml",
    "views/mail_compose_message_views.xml",
    "views/mail_group_member_views.xml",
    "views/mail_group_message_views.xml",
    "views/mail_group_moderation_views.xml",
    "views/mail_group_views.xml",
    "views/mail_group_menus.xml",
    "views/portal_templates.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/mail_group_demo.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "mail_group/static/src/css/mail_group.scss",
      "mail_group/static/src/interactions/*"
    ],
    "web.assets_backend": [
      "mail_group/static/src/css/mail_group_backend.scss"
    ]
  }
}
```

### Representative source files

- `addons/mail_group/__init__.py` (6 lines)
- `addons/mail_group/__manifest__.py` (44 lines)
- `addons/mail_group/controllers/__init__.py` (4 lines)
- `addons/mail_group/controllers/portal.py` (391 lines)
- `addons/mail_group/data/ir_cron_data.xml` (14 lines)
- `addons/mail_group/data/mail_group_demo.xml` (164 lines)
- `addons/mail_group/data/mail_template_data.xml` (62 lines)
- `addons/mail_group/data/mail_template_email_layouts.xml` (14 lines)
- `addons/mail_group/data/mail_templates.xml` (22 lines)
- `addons/mail_group/data/res_groups.xml` (10 lines)
- `addons/mail_group/i18n/ar.po` (1,714 lines)
- `addons/mail_group/i18n/az.po` (1,557 lines)
- `addons/mail_group/i18n/bg.po` (1,558 lines)
- `addons/mail_group/i18n/bs.po` (1,559 lines)
- `addons/mail_group/i18n/ca.po` (1,701 lines)
- `addons/mail_group/i18n/cs.po` (1,720 lines)
- `addons/mail_group/i18n/da.po` (1,607 lines)
- `addons/mail_group/i18n/de.po` (1,738 lines)
- `addons/mail_group/i18n/el.po` (1,589 lines)
- `addons/mail_group/i18n/es.po` (1,740 lines)
- `addons/mail_group/i18n/es_419.po` (1,737 lines)
- `addons/mail_group/i18n/et.po` (1,557 lines)
- `addons/mail_group/i18n/fa.po` (1,557 lines)
- `addons/mail_group/i18n/fi.po` (1,726 lines)
- `addons/mail_group/i18n/fr.po` (1,734 lines)
- `addons/mail_group/i18n/he.po` (1,558 lines)
- `addons/mail_group/i18n/hi.po` (1,557 lines)
- `addons/mail_group/i18n/hr.po` (1,558 lines)
- `addons/mail_group/i18n/hu.po` (1,588 lines)
- `addons/mail_group/i18n/id.po` (1,721 lines)
- `addons/mail_group/i18n/it.po` (1,731 lines)
- `addons/mail_group/i18n/ja.po` (1,720 lines)
- `addons/mail_group/i18n/kab.po` (1,558 lines)
- `addons/mail_group/i18n/ko.po` (1,677 lines)
- `addons/mail_group/i18n/ku.po` (1,557 lines)
- `addons/mail_group/i18n/lo.po` (1,690 lines)
- `addons/mail_group/i18n/lt.po` (1,559 lines)
- `addons/mail_group/i18n/lv.po` (1,558 lines)
- `addons/mail_group/i18n/mail_group.pot` (1,537 lines)
- `addons/mail_group/i18n/mn.po` (1,557 lines)
- `addons/mail_group/i18n/my.po` (1,559 lines)
- `addons/mail_group/i18n/nb.po` (1,568 lines)
- `addons/mail_group/i18n/nl.po` (1,730 lines)
- `addons/mail_group/i18n/pl.po` (1,726 lines)
- `addons/mail_group/i18n/pt.po` (1,719 lines)
- `addons/mail_group/i18n/pt_BR.po` (1,727 lines)
- `addons/mail_group/i18n/ro.po` (1,692 lines)
- `addons/mail_group/i18n/ru.po` (1,736 lines)
- `addons/mail_group/i18n/sk.po` (1,557 lines)
- `addons/mail_group/i18n/sl.po` (1,629 lines)
- `addons/mail_group/i18n/sr@latin.po` (1,558 lines)
- `addons/mail_group/i18n/sv.po` (1,639 lines)
- `addons/mail_group/i18n/th.po` (1,602 lines)
- `addons/mail_group/i18n/tr.po` (1,725 lines)
- `addons/mail_group/i18n/uk.po` (1,558 lines)
- `addons/mail_group/i18n/uz.po` (1,934 lines)
- `addons/mail_group/i18n/vi.po` (1,717 lines)
- `addons/mail_group/i18n/zh_CN.po` (1,696 lines)
- `addons/mail_group/i18n/zh_TW.po` (1,692 lines)
- `addons/mail_group/models/__init__.py` (7 lines)
- `addons/mail_group/models/mail_group.py` (755 lines)
- `addons/mail_group/models/mail_group_member.py` (41 lines)
- `addons/mail_group/models/mail_group_message.py` (249 lines)
- `addons/mail_group/models/mail_group_moderation.py` (39 lines)
- `addons/mail_group/security/ir.access.csv` (39 lines)
- `addons/mail_group/static/src/css/mail_group.scss` (49 lines)
- `addons/mail_group/static/src/css/mail_group_backend.scss` (5 lines)
- `addons/mail_group/static/src/img/fa_envelope_square.svg` (4 lines)
- `addons/mail_group/static/src/img/mail_group_portal.jpg` (450 lines)
- `addons/mail_group/static/src/interactions/mail_group.js` (89 lines)
- `addons/mail_group/static/src/interactions/mail_group_message.js` (62 lines)
- `addons/mail_group/tests/__init__.py` (7 lines)
- `addons/mail_group/tests/common.py` (78 lines)
- `addons/mail_group/tests/data.py` (44 lines)
- `addons/mail_group/tests/test_mail_group.py` (252 lines)
- `addons/mail_group/tests/test_mail_group_mailing.py` (35 lines)
- `addons/mail_group/tests/test_mail_group_message.py` (185 lines)
- `addons/mail_group/tests/test_mail_group_moderation.py` (417 lines)
- `addons/mail_group/views/mail_compose_message_views.xml` (16 lines)
- `addons/mail_group/views/mail_group_member_views.xml` (41 lines)
- `addons/mail_group/views/mail_group_menus.xml` (13 lines)
- `addons/mail_group/views/mail_group_message_views.xml` (117 lines)
- `addons/mail_group/views/mail_group_moderation_views.xml` (42 lines)
- `addons/mail_group/views/mail_group_views.xml` (201 lines)
- `addons/mail_group/views/portal_templates.xml` (332 lines)
- `addons/mail_group/wizard/__init__.py` (4 lines)
- `addons/mail_group/wizard/mail_group_message_reject.py` (42 lines)
- `addons/mail_group/wizard/mail_group_message_reject_views.xml` (42 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
