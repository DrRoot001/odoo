# Module: microsoft_outlook

- **Module ID:** MOD-376
- **Path:** `addons/microsoft_outlook`
- **Manifest:** `addons/microsoft_outlook/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Outlook support for incoming / outgoing mail servers

Declared dependencies: `mail`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 2 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mail"
  ],
  "data": [
    "views/fetchmail_server_views.xml",
    "views/ir_mail_server_views.xml",
    "views/res_config_settings_views.xml",
    "views/templates.xml"
  ]
}
```

### Representative source files

- `addons/microsoft_outlook/__init__.py` (5 lines)
- `addons/microsoft_outlook/__manifest__.py` (20 lines)
- `addons/microsoft_outlook/controllers/__init__.py` (4 lines)
- `addons/microsoft_outlook/controllers/main.py` (136 lines)
- `addons/microsoft_outlook/i18n/ar.po` (339 lines)
- `addons/microsoft_outlook/i18n/az.po` (309 lines)
- `addons/microsoft_outlook/i18n/bg.po` (310 lines)
- `addons/microsoft_outlook/i18n/bs.po` (310 lines)
- `addons/microsoft_outlook/i18n/ca.po` (332 lines)
- `addons/microsoft_outlook/i18n/cs.po` (322 lines)
- `addons/microsoft_outlook/i18n/da.po` (314 lines)
- `addons/microsoft_outlook/i18n/de.po` (340 lines)
- `addons/microsoft_outlook/i18n/el.po` (310 lines)
- `addons/microsoft_outlook/i18n/es.po` (340 lines)
- `addons/microsoft_outlook/i18n/es_419.po` (337 lines)
- `addons/microsoft_outlook/i18n/et.po` (318 lines)
- `addons/microsoft_outlook/i18n/fa.po` (310 lines)
- `addons/microsoft_outlook/i18n/fi.po` (339 lines)
- `addons/microsoft_outlook/i18n/fr.po` (342 lines)
- `addons/microsoft_outlook/i18n/he.po` (310 lines)
- `addons/microsoft_outlook/i18n/hi.po` (309 lines)
- `addons/microsoft_outlook/i18n/hr.po` (310 lines)
- `addons/microsoft_outlook/i18n/hu.po` (310 lines)
- `addons/microsoft_outlook/i18n/id.po` (337 lines)
- `addons/microsoft_outlook/i18n/it.po` (340 lines)
- `addons/microsoft_outlook/i18n/ja.po` (337 lines)
- `addons/microsoft_outlook/i18n/kab.po` (309 lines)
- `addons/microsoft_outlook/i18n/ko.po` (333 lines)
- `addons/microsoft_outlook/i18n/ku.po` (309 lines)
- `addons/microsoft_outlook/i18n/lo.po` (334 lines)
- `addons/microsoft_outlook/i18n/lt.po` (311 lines)
- `addons/microsoft_outlook/i18n/lv.po` (309 lines)
- `addons/microsoft_outlook/i18n/microsoft_outlook.pot` (300 lines)
- `addons/microsoft_outlook/i18n/mn.po` (309 lines)
- `addons/microsoft_outlook/i18n/my.po` (309 lines)
- `addons/microsoft_outlook/i18n/nb.po` (310 lines)
- `addons/microsoft_outlook/i18n/nl.po` (340 lines)
- `addons/microsoft_outlook/i18n/pl.po` (341 lines)
- `addons/microsoft_outlook/i18n/pt.po` (336 lines)
- `addons/microsoft_outlook/i18n/pt_BR.po` (341 lines)
- `addons/microsoft_outlook/i18n/ro.po` (341 lines)
- `addons/microsoft_outlook/i18n/ru.po` (342 lines)
- `addons/microsoft_outlook/i18n/sk.po` (308 lines)
- `addons/microsoft_outlook/i18n/sl.po` (312 lines)
- `addons/microsoft_outlook/i18n/sr@latin.po` (310 lines)
- `addons/microsoft_outlook/i18n/sv.po` (338 lines)
- `addons/microsoft_outlook/i18n/th.po` (335 lines)
- `addons/microsoft_outlook/i18n/tr.po` (339 lines)
- `addons/microsoft_outlook/i18n/uk.po` (331 lines)
- `addons/microsoft_outlook/i18n/uz.po` (379 lines)
- `addons/microsoft_outlook/i18n/vi.po` (338 lines)
- `addons/microsoft_outlook/i18n/zh_CN.po` (331 lines)
- `addons/microsoft_outlook/i18n/zh_TW.po` (331 lines)
- `addons/microsoft_outlook/models/__init__.py` (9 lines)
- `addons/microsoft_outlook/models/fetchmail_server.py` (63 lines)
- `addons/microsoft_outlook/models/ir_mail_server.py` (91 lines)
- `addons/microsoft_outlook/models/microsoft_outlook_mixin.py` (282 lines)
- `addons/microsoft_outlook/models/res_config_settings.py` (11 lines)
- `addons/microsoft_outlook/models/res_users.py` (28 lines)
- `addons/microsoft_outlook/static/description/icon.png` (30 lines)
- `addons/microsoft_outlook/static/description/icon.svg` (1 lines)
- `addons/microsoft_outlook/static/description/icon_hi.png` (520 lines)
- `addons/microsoft_outlook/tests/__init__.py` (4 lines)
- `addons/microsoft_outlook/tests/test_fetchmail_outlook.py` (50 lines)
- `addons/microsoft_outlook/views/fetchmail_server_views.xml` (32 lines)
- `addons/microsoft_outlook/views/ir_mail_server_views.xml` (38 lines)
- `addons/microsoft_outlook/views/res_config_settings_views.xml` (26 lines)
- `addons/microsoft_outlook/views/templates.xml` (15 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
