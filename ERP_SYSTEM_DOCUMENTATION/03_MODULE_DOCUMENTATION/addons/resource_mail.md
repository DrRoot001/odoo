# Module: resource_mail

- **Module ID:** MOD-507
- **Path:** `addons/resource_mail`
- **Manifest:** `addons/resource_mail/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Integrate features developped in Mail in use case involving resources instead of users

Declared dependencies: `resource`, `mail`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 10 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "resource",
    "mail"
  ],
  "assets": {
    "web.assets_backend": [
      "resource_mail/static/src/core/common/**/*",
      "resource_mail/static/src/core/web/**/*",
      "resource_mail/static/src/**/*"
    ],
    "im_livechat.assets_embed_core": [
      "resource_mail/static/src/core/common/**/*"
    ],
    "mail.assets_public": [
      "resource_mail/static/src/core/common/**/*"
    ],
    "portal.assets_chatter_helpers": [
      "resource_mail/static/src/core/common/**/*"
    ],
    "web.assets_unit_tests": [
      "resource_mail/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/resource_mail/__init__.py` (5 lines)
- `addons/resource_mail/__manifest__.py` (30 lines)
- `addons/resource_mail/controllers/__init__.py` (3 lines)
- `addons/resource_mail/controllers/webclient.py` (9 lines)
- `addons/resource_mail/i18n/ar.po` (73 lines)
- `addons/resource_mail/i18n/az.po` (71 lines)
- `addons/resource_mail/i18n/bg.po` (71 lines)
- `addons/resource_mail/i18n/bs.po` (72 lines)
- `addons/resource_mail/i18n/ca.po` (72 lines)
- `addons/resource_mail/i18n/cs.po` (72 lines)
- `addons/resource_mail/i18n/da.po` (73 lines)
- `addons/resource_mail/i18n/de.po` (74 lines)
- `addons/resource_mail/i18n/el.po` (72 lines)
- `addons/resource_mail/i18n/es.po` (75 lines)
- `addons/resource_mail/i18n/es_419.po` (73 lines)
- `addons/resource_mail/i18n/et.po` (71 lines)
- `addons/resource_mail/i18n/fa.po` (71 lines)
- `addons/resource_mail/i18n/fi.po` (73 lines)
- `addons/resource_mail/i18n/fr.po` (73 lines)
- `addons/resource_mail/i18n/he.po` (72 lines)
- `addons/resource_mail/i18n/hi.po` (71 lines)
- `addons/resource_mail/i18n/hr.po` (72 lines)
- `addons/resource_mail/i18n/hu.po` (72 lines)
- `addons/resource_mail/i18n/id.po` (73 lines)
- `addons/resource_mail/i18n/it.po` (72 lines)
- `addons/resource_mail/i18n/ja.po` (72 lines)
- `addons/resource_mail/i18n/kab.po` (71 lines)
- `addons/resource_mail/i18n/ko.po` (73 lines)
- `addons/resource_mail/i18n/ku.po` (71 lines)
- `addons/resource_mail/i18n/lo.po` (70 lines)
- `addons/resource_mail/i18n/lt.po` (73 lines)
- `addons/resource_mail/i18n/lv.po` (71 lines)
- `addons/resource_mail/i18n/mn.po` (71 lines)
- `addons/resource_mail/i18n/my.po` (71 lines)
- `addons/resource_mail/i18n/nb.po` (72 lines)
- `addons/resource_mail/i18n/nl.po` (72 lines)
- `addons/resource_mail/i18n/pl.po` (73 lines)
- `addons/resource_mail/i18n/pt.po` (73 lines)
- `addons/resource_mail/i18n/pt_BR.po` (77 lines)
- `addons/resource_mail/i18n/resource_mail.pot` (67 lines)
- `addons/resource_mail/i18n/ro.po` (72 lines)
- `addons/resource_mail/i18n/ru.po` (75 lines)
- `addons/resource_mail/i18n/sk.po` (70 lines)
- `addons/resource_mail/i18n/sl.po` (73 lines)
- `addons/resource_mail/i18n/sr@latin.po` (72 lines)
- `addons/resource_mail/i18n/sv.po` (73 lines)
- `addons/resource_mail/i18n/th.po` (73 lines)
- `addons/resource_mail/i18n/tr.po` (77 lines)
- `addons/resource_mail/i18n/uk.po` (72 lines)
- `addons/resource_mail/i18n/uz.po` (82 lines)
- `addons/resource_mail/i18n/vi.po` (73 lines)
- `addons/resource_mail/i18n/zh_CN.po` (73 lines)
- `addons/resource_mail/i18n/zh_TW.po` (74 lines)
- `addons/resource_mail/models/__init__.py` (4 lines)
- `addons/resource_mail/models/resource_resource.py` (13 lines)
- `addons/resource_mail/static/src/core/common/@types/models.d.ts` (13 lines)
- `addons/resource_mail/static/src/core/common/resource_resource_model.js` (15 lines)
- `addons/resource_mail/static/src/core/web/avatar_card/avatar_card_patch.js` (36 lines)
- `addons/resource_mail/static/src/views/fields/many2many_avatar_resource/many2many_avatar_resource_field.js` (124 lines)
- `addons/resource_mail/static/src/views/fields/many2many_avatar_resource/many2many_avatar_resource_field.scss` (3 lines)
- `addons/resource_mail/static/src/views/fields/many2many_avatar_resource/many2many_avatar_resource_field.xml` (30 lines)
- `addons/resource_mail/static/src/views/fields/many2one_avatar_resource/kanban_many2one_avatar_resource_field.js` (38 lines)
- `addons/resource_mail/static/src/views/fields/many2one_avatar_resource/kanban_many2one_avatar_resource_field.xml` (36 lines)
- `addons/resource_mail/static/src/views/fields/many2one_avatar_resource/many2one_avatar_resource_field.js` (45 lines)
- `addons/resource_mail/static/src/views/fields/many2one_avatar_resource/many2one_avatar_resource_field.scss` (4 lines)
- `addons/resource_mail/static/src/views/fields/many2one_avatar_resource/many2one_avatar_resource_field.xml` (38 lines)
- `addons/resource_mail/static/tests/many2many_avatar_resource.test.js` (309 lines)
- `addons/resource_mail/static/tests/many2one_avatar_resource.test.js` (168 lines)
- `addons/resource_mail/static/tests/mock_server/mock_models/resource_resource.js` (10 lines)
- `addons/resource_mail/static/tests/resource_mail_test_helpers.js` (7 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
