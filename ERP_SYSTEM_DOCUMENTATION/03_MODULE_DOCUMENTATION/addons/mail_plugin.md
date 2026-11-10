# Module: mail_plugin

- **Module ID:** MOD-355
- **Path:** `addons/mail_plugin`
- **Manifest:** `addons/mail_plugin/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Allows integration with mail plugins.

Integrate Odoo with your mailbox, get information about contacts directly inside your mailbox, log content of emails as internal notes

Declared dependencies: `digest`, `web`, `contacts`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 10 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "digest",
    "web",
    "contacts"
  ],
  "data": [
    "data/digest_tips.xml",
    "views/mail_plugin_login.xml"
  ]
}
```

### Representative source files

- `addons/mail_plugin/__init__.py` (5 lines)
- `addons/mail_plugin/__manifest__.py` (22 lines)
- `addons/mail_plugin/controllers/__init__.py` (5 lines)
- `addons/mail_plugin/controllers/authenticate.py` (128 lines)
- `addons/mail_plugin/controllers/mail_plugin.py` (246 lines)
- `addons/mail_plugin/data/digest_tips.xml` (34 lines)
- `addons/mail_plugin/i18n/ar.po` (363 lines)
- `addons/mail_plugin/i18n/az.po` (353 lines)
- `addons/mail_plugin/i18n/bg.po` (353 lines)
- `addons/mail_plugin/i18n/bs.po` (355 lines)
- `addons/mail_plugin/i18n/ca.po` (358 lines)
- `addons/mail_plugin/i18n/cs.po` (355 lines)
- `addons/mail_plugin/i18n/da.po` (355 lines)
- `addons/mail_plugin/i18n/de.po` (368 lines)
- `addons/mail_plugin/i18n/el.po` (354 lines)
- `addons/mail_plugin/i18n/es.po` (363 lines)
- `addons/mail_plugin/i18n/es_419.po` (364 lines)
- `addons/mail_plugin/i18n/et.po` (353 lines)
- `addons/mail_plugin/i18n/fa.po` (353 lines)
- `addons/mail_plugin/i18n/fi.po` (370 lines)
- `addons/mail_plugin/i18n/fr.po` (365 lines)
- `addons/mail_plugin/i18n/he.po` (354 lines)
- `addons/mail_plugin/i18n/hi.po` (353 lines)
- `addons/mail_plugin/i18n/hr.po` (354 lines)
- `addons/mail_plugin/i18n/hu.po` (354 lines)
- `addons/mail_plugin/i18n/id.po` (361 lines)
- `addons/mail_plugin/i18n/it.po` (364 lines)
- `addons/mail_plugin/i18n/ja.po` (365 lines)
- `addons/mail_plugin/i18n/kab.po` (354 lines)
- `addons/mail_plugin/i18n/ko.po` (358 lines)
- `addons/mail_plugin/i18n/ku.po` (353 lines)
- `addons/mail_plugin/i18n/lo.po` (361 lines)
- `addons/mail_plugin/i18n/lt.po` (355 lines)
- `addons/mail_plugin/i18n/lv.po` (354 lines)
- `addons/mail_plugin/i18n/mail_plugin.pot` (350 lines)
- `addons/mail_plugin/i18n/mn.po` (353 lines)
- `addons/mail_plugin/i18n/my.po` (354 lines)
- `addons/mail_plugin/i18n/nb.po` (354 lines)
- `addons/mail_plugin/i18n/nl.po` (363 lines)
- `addons/mail_plugin/i18n/pl.po` (362 lines)
- `addons/mail_plugin/i18n/pt.po` (362 lines)
- `addons/mail_plugin/i18n/pt_BR.po` (368 lines)
- `addons/mail_plugin/i18n/ro.po` (357 lines)
- `addons/mail_plugin/i18n/ru.po` (363 lines)
- `addons/mail_plugin/i18n/sk.po` (353 lines)
- `addons/mail_plugin/i18n/sl.po` (363 lines)
- `addons/mail_plugin/i18n/sr@latin.po` (354 lines)
- `addons/mail_plugin/i18n/sv.po` (361 lines)
- `addons/mail_plugin/i18n/th.po` (357 lines)
- `addons/mail_plugin/i18n/tr.po` (364 lines)
- `addons/mail_plugin/i18n/uk.po` (354 lines)
- `addons/mail_plugin/i18n/uz.po` (396 lines)
- `addons/mail_plugin/i18n/vi.po` (361 lines)
- `addons/mail_plugin/i18n/zh_CN.po` (358 lines)
- `addons/mail_plugin/i18n/zh_TW.po` (356 lines)
- `addons/mail_plugin/models/__init__.py` (4 lines)
- `addons/mail_plugin/models/ir_http.py` (34 lines)
- `addons/mail_plugin/static/src/img/gmail.png` (12 lines)
- `addons/mail_plugin/static/src/img/outlook.png` (30 lines)
- `addons/mail_plugin/static/src/to_translate/translations_gmail.xml` (38 lines)
- `addons/mail_plugin/static/src/to_translate/translations_outlook.xml` (27 lines)
- `addons/mail_plugin/tests/__init__.py` (3 lines)
- `addons/mail_plugin/tests/common.py` (100 lines)
- `addons/mail_plugin/tests/test_controller.py` (90 lines)
- `addons/mail_plugin/views/mail_plugin_login.xml` (26 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
