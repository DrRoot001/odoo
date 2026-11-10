# Module: base_automation

- **Module ID:** MOD-035
- **Path:** `addons/base_automation`
- **Manifest:** `addons/base_automation/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This module allows to implement automation rules for any object.
================================================================

Use automation rules to automatically trigger actions for various screens.

**Example:** A lead created by a specific user may be automatically set to a specific
Sales Team, or an opportunity which still has status pending after 14 days might
trigger an automatic reminder email.
    

Declared dependencies: `base`, `digest`, `resource`, `mail`, `sms`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 7 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 8 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base",
    "digest",
    "resource",
    "mail",
    "sms"
  ],
  "data": [
    "data/base_automation_data.xml",
    "data/digest_data.xml",
    "views/base_automation_views.xml",
    "views/ir_actions_server_views.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "base_automation/static/src/**/*"
    ],
    "web.assets_unit_tests": [
      "base_automation/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/base_automation/__init__.py` (5 lines)
- `addons/base_automation/__manifest__.py` (34 lines)
- `addons/base_automation/controllers/__init__.py` (1 lines)
- `addons/base_automation/controllers/main.py` (18 lines)
- `addons/base_automation/data/base_automation_data.xml` (14 lines)
- `addons/base_automation/data/digest_data.xml` (17 lines)
- `addons/base_automation/i18n/af.po` (988 lines)
- `addons/base_automation/i18n/ar.po` (1,049 lines)
- `addons/base_automation/i18n/az.po` (1,014 lines)
- `addons/base_automation/i18n/base_automation.pot` (979 lines)
- `addons/base_automation/i18n/bg.po` (1,013 lines)
- `addons/base_automation/i18n/bs.po` (1,056 lines)
- `addons/base_automation/i18n/ca.po` (1,038 lines)
- `addons/base_automation/i18n/cs.po` (1,062 lines)
- `addons/base_automation/i18n/da.po` (1,059 lines)
- `addons/base_automation/i18n/de.po` (1,090 lines)
- `addons/base_automation/i18n/el.po` (1,007 lines)
- `addons/base_automation/i18n/es.po` (1,084 lines)
- `addons/base_automation/i18n/es_419.po` (1,076 lines)
- `addons/base_automation/i18n/es_CL.po` (54 lines)
- `addons/base_automation/i18n/et.po` (1,051 lines)
- `addons/base_automation/i18n/eu.po` (987 lines)
- `addons/base_automation/i18n/fa.po` (1,046 lines)
- `addons/base_automation/i18n/fi.po` (1,084 lines)
- `addons/base_automation/i18n/fo.po` (987 lines)
- `addons/base_automation/i18n/fr.po` (1,086 lines)
- `addons/base_automation/i18n/fr_BE.po` (66 lines)
- `addons/base_automation/i18n/fr_CA.po` (54 lines)
- `addons/base_automation/i18n/gl.po` (987 lines)
- `addons/base_automation/i18n/gu.po` (988 lines)
- `addons/base_automation/i18n/he.po` (1,019 lines)
- `addons/base_automation/i18n/hi.po` (1,012 lines)
- `addons/base_automation/i18n/hr.po` (1,150 lines)
- `addons/base_automation/i18n/hu.po` (1,010 lines)
- `addons/base_automation/i18n/id.po` (1,066 lines)
- `addons/base_automation/i18n/is.po` (984 lines)
- `addons/base_automation/i18n/it.po` (1,075 lines)
- `addons/base_automation/i18n/ja.po` (1,068 lines)
- `addons/base_automation/i18n/ka.po` (987 lines)
- `addons/base_automation/i18n/kab.po` (1,016 lines)
- `addons/base_automation/i18n/kk.po` (986 lines)
- `addons/base_automation/i18n/km.po` (989 lines)
- `addons/base_automation/i18n/ko.po` (1,054 lines)
- `addons/base_automation/i18n/ku.po` (998 lines)
- `addons/base_automation/i18n/lo.po` (1,057 lines)
- `addons/base_automation/i18n/lt.po` (1,017 lines)
- `addons/base_automation/i18n/lv.po` (1,048 lines)
- `addons/base_automation/i18n/mk.po` (987 lines)
- `addons/base_automation/i18n/mn.po` (1,012 lines)
- `addons/base_automation/i18n/my.po` (992 lines)
- `addons/base_automation/i18n/nb.po` (1,004 lines)
- `addons/base_automation/i18n/nl.po` (1,082 lines)
- `addons/base_automation/i18n/pl.po` (1,085 lines)
- `addons/base_automation/i18n/pt.po` (1,064 lines)
- `addons/base_automation/i18n/pt_BR.po` (1,071 lines)
- `addons/base_automation/i18n/ro.po` (1,077 lines)
- `addons/base_automation/i18n/ru.po` (1,066 lines)
- `addons/base_automation/i18n/sk.po` (1,052 lines)
- `addons/base_automation/i18n/sl.po` (1,063 lines)
- `addons/base_automation/i18n/sq.po` (987 lines)
- `addons/base_automation/i18n/sr@latin.po` (1,004 lines)
- `addons/base_automation/i18n/sv.po` (1,074 lines)
- `addons/base_automation/i18n/ta.po` (988 lines)
- `addons/base_automation/i18n/th.po` (1,037 lines)
- `addons/base_automation/i18n/tr.po` (1,072 lines)
- `addons/base_automation/i18n/uk.po` (1,056 lines)
- `addons/base_automation/i18n/uz.po` (1,223 lines)
- `addons/base_automation/i18n/vi.po` (1,062 lines)
- `addons/base_automation/i18n/zh_CN.po` (1,041 lines)
- `addons/base_automation/i18n/zh_TW.po` (1,034 lines)
- `addons/base_automation/models/__init__.py` (5 lines)
- `addons/base_automation/models/base_automation.py` (1,202 lines)
- `addons/base_automation/models/ir_actions_server.py` (78 lines)
- `addons/base_automation/security/ir.access.csv` (2 lines)
- `addons/base_automation/static/img/automation.svg` (25 lines)
- `addons/base_automation/static/src/base_automation.scss` (45 lines)
- `addons/base_automation/static/src/base_automation_actions_one2many_field.js` (92 lines)
- `addons/base_automation/static/src/base_automation_actions_one2many_field.xml` (45 lines)
- `addons/base_automation/static/src/base_automation_error_dialog.js` (56 lines)
- `addons/base_automation/static/src/base_automation_error_dialog.xml` (25 lines)
- `addons/base_automation/static/src/base_automation_trigger_selection_field.js` (132 lines)
- `addons/base_automation/static/src/base_automation_trigger_selection_field.xml` (10 lines)
- `addons/base_automation/static/src/group_config_menu_patch.js` (96 lines)
- `addons/base_automation/static/src/utils.js` (23 lines)
- `addons/base_automation/static/tests/base_automation.test.js` (112 lines)
- `addons/base_automation/static/tests/base_automation_error_dialog.test.js` (95 lines)
- `addons/base_automation/static/tests/kanban_header_patch.test.js` (98 lines)
- `addons/base_automation/tests/__init__.py` (5 lines)
- `addons/base_automation/tests/test_automation.py` (307 lines)
- `addons/base_automation/tests/test_mail_composer.py` (82 lines)
- `addons/base_automation/views/base_automation_views.xml` (268 lines)
- `addons/base_automation/views/ir_actions_server_views.xml` (27 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
