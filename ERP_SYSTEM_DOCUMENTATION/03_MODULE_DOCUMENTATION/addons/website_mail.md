# Module: website_mail

- **Module ID:** MOD-624
- **Path:** `addons/website_mail`
- **Manifest:** `addons/website_mail/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Website Module for Mail


Module holding mail improvements for website. It holds the follow widget.


Declared dependencies: `website`, `mail`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 2 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website",
    "mail"
  ],
  "data": [
    "views/website_mail_templates.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "website_mail/static/src/interactions/follow.js",
      "website_mail/static/src/css/website_mail.scss"
    ],
    "web.assets_inside_builder_iframe": [
      "website/static/src/interactions/follow.edit.js"
    ]
  }
}
```

### Representative source files

- `addons/website_mail/__init__.py` (5 lines)
- `addons/website_mail/__manifest__.py` (27 lines)
- `addons/website_mail/controllers/__init__.py` (4 lines)
- `addons/website_mail/controllers/main.py` (99 lines)
- `addons/website_mail/i18n/ar.po` (90 lines)
- `addons/website_mail/i18n/az.po` (86 lines)
- `addons/website_mail/i18n/bg.po` (87 lines)
- `addons/website_mail/i18n/bs.po` (87 lines)
- `addons/website_mail/i18n/ca.po` (89 lines)
- `addons/website_mail/i18n/cs.po` (88 lines)
- `addons/website_mail/i18n/da.po` (89 lines)
- `addons/website_mail/i18n/de.po` (92 lines)
- `addons/website_mail/i18n/el.po` (88 lines)
- `addons/website_mail/i18n/es.po` (93 lines)
- `addons/website_mail/i18n/es_419.po` (84 lines)
- `addons/website_mail/i18n/et.po` (87 lines)
- `addons/website_mail/i18n/fa.po` (86 lines)
- `addons/website_mail/i18n/fi.po` (91 lines)
- `addons/website_mail/i18n/fr.po` (90 lines)
- `addons/website_mail/i18n/gu.po` (84 lines)
- `addons/website_mail/i18n/he.po` (88 lines)
- `addons/website_mail/i18n/hi.po` (84 lines)
- `addons/website_mail/i18n/hr.po` (88 lines)
- `addons/website_mail/i18n/hu.po` (87 lines)
- `addons/website_mail/i18n/id.po` (89 lines)
- `addons/website_mail/i18n/is.po` (80 lines)
- `addons/website_mail/i18n/it.po` (89 lines)
- `addons/website_mail/i18n/ja.po` (88 lines)
- `addons/website_mail/i18n/kab.po` (84 lines)
- `addons/website_mail/i18n/ko.po` (88 lines)
- `addons/website_mail/i18n/ku.po` (84 lines)
- `addons/website_mail/i18n/lo.po` (83 lines)
- `addons/website_mail/i18n/lt.po` (90 lines)
- `addons/website_mail/i18n/lv.po` (86 lines)
- `addons/website_mail/i18n/mk.po` (84 lines)
- `addons/website_mail/i18n/mn.po` (88 lines)
- `addons/website_mail/i18n/my.po` (84 lines)
- `addons/website_mail/i18n/nb.po` (89 lines)
- `addons/website_mail/i18n/nl.po` (89 lines)
- `addons/website_mail/i18n/pl.po` (91 lines)
- `addons/website_mail/i18n/pt.po` (88 lines)
- `addons/website_mail/i18n/pt_BR.po` (93 lines)
- `addons/website_mail/i18n/ro.po` (89 lines)
- `addons/website_mail/i18n/ru.po` (89 lines)
- `addons/website_mail/i18n/sk.po` (87 lines)
- `addons/website_mail/i18n/sl.po` (89 lines)
- `addons/website_mail/i18n/sr@latin.po` (88 lines)
- `addons/website_mail/i18n/sv.po` (90 lines)
- `addons/website_mail/i18n/th.po` (88 lines)
- `addons/website_mail/i18n/tr.po` (89 lines)
- `addons/website_mail/i18n/uk.po` (90 lines)
- `addons/website_mail/i18n/uz.po` (98 lines)
- `addons/website_mail/i18n/vi.po` (89 lines)
- `addons/website_mail/i18n/website_mail.pot` (80 lines)
- `addons/website_mail/i18n/zh_CN.po` (87 lines)
- `addons/website_mail/i18n/zh_TW.po` (87 lines)
- `addons/website_mail/models/__init__.py` (5 lines)
- `addons/website_mail/models/ir_http.py` (12 lines)
- `addons/website_mail/models/update.py` (14 lines)
- `addons/website_mail/static/src/css/website_mail.scss` (49 lines)
- `addons/website_mail/static/src/img/thumbnail/airmail.png` (321 lines)
- `addons/website_mail/static/src/img/thumbnail/basic.png` (461 lines)
- `addons/website_mail/static/src/img/thumbnail/cleave.png` (204 lines)
- `addons/website_mail/static/src/img/thumbnail/go.png` (283 lines)
- `addons/website_mail/static/src/img/thumbnail/narrative.png` (303 lines)
- `addons/website_mail/static/src/img/thumbnail/neopolitan.png` (185 lines)
- `addons/website_mail/static/src/img/thumbnail/skyline.png` (606 lines)
- `addons/website_mail/static/src/img/thumbnail/sunday.png` (310 lines)
- `addons/website_mail/static/src/img/thumbnail/zenflat.png` (134 lines)
- `addons/website_mail/static/src/interactions/follow.edit.js` (13 lines)
- `addons/website_mail/static/src/interactions/follow.js` (142 lines)
- `addons/website_mail/views/website_mail_templates.xml` (31 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
