# Module: crm_mail_plugin

- **Module ID:** MOD-058
- **Path:** `addons/crm_mail_plugin`
- **Manifest:** `addons/crm_mail_plugin/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Turn emails received in your mailbox into leads and log their content as internal notes.

Turn emails received in your mailbox into leads and log their content as internal notes.

Declared dependencies: `crm`, `mail_plugin`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "crm",
    "mail_plugin"
  ]
}
```

### Representative source files

- `addons/crm_mail_plugin/__init__.py` (3 lines)
- `addons/crm_mail_plugin/__manifest__.py` (17 lines)
- `addons/crm_mail_plugin/controllers/__init__.py` (3 lines)
- `addons/crm_mail_plugin/controllers/mail_plugin.py` (156 lines)
- `addons/crm_mail_plugin/i18n/ar.po` (104 lines)
- `addons/crm_mail_plugin/i18n/az.po` (103 lines)
- `addons/crm_mail_plugin/i18n/bg.po` (103 lines)
- `addons/crm_mail_plugin/i18n/bs.po` (105 lines)
- `addons/crm_mail_plugin/i18n/ca.po` (104 lines)
- `addons/crm_mail_plugin/i18n/crm_mail_plugin.pot` (99 lines)
- `addons/crm_mail_plugin/i18n/cs.po` (103 lines)
- `addons/crm_mail_plugin/i18n/da.po` (106 lines)
- `addons/crm_mail_plugin/i18n/de.po` (109 lines)
- `addons/crm_mail_plugin/i18n/el.po` (104 lines)
- `addons/crm_mail_plugin/i18n/es.po` (106 lines)
- `addons/crm_mail_plugin/i18n/es_419.po` (108 lines)
- `addons/crm_mail_plugin/i18n/et.po` (103 lines)
- `addons/crm_mail_plugin/i18n/fa.po` (103 lines)
- `addons/crm_mail_plugin/i18n/fi.po` (108 lines)
- `addons/crm_mail_plugin/i18n/fr.po` (109 lines)
- `addons/crm_mail_plugin/i18n/he.po` (104 lines)
- `addons/crm_mail_plugin/i18n/hi.po` (103 lines)
- `addons/crm_mail_plugin/i18n/hr.po` (104 lines)
- `addons/crm_mail_plugin/i18n/hu.po` (104 lines)
- `addons/crm_mail_plugin/i18n/id.po` (107 lines)
- `addons/crm_mail_plugin/i18n/it.po` (108 lines)
- `addons/crm_mail_plugin/i18n/ja.po` (109 lines)
- `addons/crm_mail_plugin/i18n/kab.po` (104 lines)
- `addons/crm_mail_plugin/i18n/ko.po` (106 lines)
- `addons/crm_mail_plugin/i18n/ku.po` (103 lines)
- `addons/crm_mail_plugin/i18n/lo.po` (102 lines)
- `addons/crm_mail_plugin/i18n/lt.po` (105 lines)
- `addons/crm_mail_plugin/i18n/lv.po` (105 lines)
- `addons/crm_mail_plugin/i18n/mn.po` (103 lines)
- `addons/crm_mail_plugin/i18n/my.po` (103 lines)
- `addons/crm_mail_plugin/i18n/nb.po` (103 lines)
- `addons/crm_mail_plugin/i18n/nl.po` (106 lines)
- `addons/crm_mail_plugin/i18n/pl.po` (104 lines)
- `addons/crm_mail_plugin/i18n/pt.po` (103 lines)
- `addons/crm_mail_plugin/i18n/pt_BR.po` (108 lines)
- `addons/crm_mail_plugin/i18n/ro.po` (104 lines)
- `addons/crm_mail_plugin/i18n/ru.po` (111 lines)
- `addons/crm_mail_plugin/i18n/sk.po` (104 lines)
- `addons/crm_mail_plugin/i18n/sl.po` (104 lines)
- `addons/crm_mail_plugin/i18n/sr@latin.po` (104 lines)
- `addons/crm_mail_plugin/i18n/sv.po` (105 lines)
- `addons/crm_mail_plugin/i18n/th.po` (106 lines)
- `addons/crm_mail_plugin/i18n/tr.po` (109 lines)
- `addons/crm_mail_plugin/i18n/uk.po` (104 lines)
- `addons/crm_mail_plugin/i18n/uz.po` (112 lines)
- `addons/crm_mail_plugin/i18n/vi.po` (103 lines)
- `addons/crm_mail_plugin/i18n/zh_CN.po` (104 lines)
- `addons/crm_mail_plugin/i18n/zh_TW.po` (105 lines)
- `addons/crm_mail_plugin/static/src/to_translate/translations_gmail.xml` (14 lines)
- `addons/crm_mail_plugin/static/src/to_translate/translations_outlook.xml` (15 lines)
- `addons/crm_mail_plugin/tests/__init__.py` (3 lines)
- `addons/crm_mail_plugin/tests/test_crm_mail_plugin.py` (90 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
