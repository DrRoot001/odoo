# Module: portal_rating

- **Module ID:** MOD-421
- **Path:** `addons/portal_rating`
- **Manifest:** `addons/portal_rating/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Bridge module adding rating capabilities on portal. It includes notably
inclusion of rating directly within the customer portal discuss widget.
        

Declared dependencies: `portal`, `rating`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 10 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 19 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "portal",
    "rating"
  ],
  "data": [
    "views/rating_rating_views.xml",
    "views/portal_templates.xml",
    "views/rating_templates.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "portal_rating/static/src/core/common/**/*"
    ],
    "mail.assets_public": [
      "portal_rating/static/src/core/common/**/*"
    ],
    "im_livechat.assets_embed_core": [
      "portal_rating/static/src/core/common/**/*"
    ],
    "portal.assets_chatter_helpers": [
      "portal_rating/static/src/core/common/**/*"
    ],
    "web.assets_frontend": [
      "portal_rating/static/src/scss/portal_rating.scss",
      "portal_rating/static/src/xml/portal_chatter.xml",
      "portal_rating/static/src/interactions/**/*",
      "portal_rating/static/src/xml/portal_rating_composer.xml",
      "portal_rating/static/src/xml/portal_tools.xml"
    ],
    "web.assets_unit_tests_setup": [
      "portal_rating/static/src/interactions/**/*",
      "portal_rating/static/src/xml/**/*"
    ],
    "portal.assets_chatter": [
      "portal_rating/static/src/chatter/portal/**/*"
    ],
    "portal.assets_chatter_style": [
      "portal_rating/static/src/scss/portal_rating.scss"
    ]
  }
}
```

### Representative source files

- `addons/portal_rating/__init__.py` (5 lines)
- `addons/portal_rating/__manifest__.py` (53 lines)
- `addons/portal_rating/controllers/__init__.py` (4 lines)
- `addons/portal_rating/controllers/portal_rating.py` (22 lines)
- `addons/portal_rating/controllers/thread.py` (14 lines)
- `addons/portal_rating/i18n/ar.po` (261 lines)
- `addons/portal_rating/i18n/az.po` (282 lines)
- `addons/portal_rating/i18n/bg.po` (279 lines)
- `addons/portal_rating/i18n/bs.po` (268 lines)
- `addons/portal_rating/i18n/ca.po` (274 lines)
- `addons/portal_rating/i18n/cs.po` (268 lines)
- `addons/portal_rating/i18n/da.po` (275 lines)
- `addons/portal_rating/i18n/de.po` (268 lines)
- `addons/portal_rating/i18n/el.po` (262 lines)
- `addons/portal_rating/i18n/es.po` (268 lines)
- `addons/portal_rating/i18n/es_419.po` (258 lines)
- `addons/portal_rating/i18n/et.po` (273 lines)
- `addons/portal_rating/i18n/fa.po` (280 lines)
- `addons/portal_rating/i18n/fi.po` (274 lines)
- `addons/portal_rating/i18n/fr.po` (264 lines)
- `addons/portal_rating/i18n/gu.po` (254 lines)
- `addons/portal_rating/i18n/he.po` (276 lines)
- `addons/portal_rating/i18n/hi.po` (267 lines)
- `addons/portal_rating/i18n/hr.po` (286 lines)
- `addons/portal_rating/i18n/hu.po` (268 lines)
- `addons/portal_rating/i18n/id.po` (268 lines)
- `addons/portal_rating/i18n/is.po` (250 lines)
- `addons/portal_rating/i18n/it.po` (267 lines)
- `addons/portal_rating/i18n/ja.po` (258 lines)
- `addons/portal_rating/i18n/kab.po` (261 lines)
- `addons/portal_rating/i18n/km.po` (254 lines)
- `addons/portal_rating/i18n/ko.po` (264 lines)
- `addons/portal_rating/i18n/ku.po` (261 lines)
- `addons/portal_rating/i18n/lo.po` (259 lines)
- `addons/portal_rating/i18n/lt.po` (269 lines)
- `addons/portal_rating/i18n/lv.po` (268 lines)
- `addons/portal_rating/i18n/mn.po` (267 lines)
- `addons/portal_rating/i18n/my.po` (261 lines)
- `addons/portal_rating/i18n/nb.po` (263 lines)
- `addons/portal_rating/i18n/nl.po` (263 lines)
- `addons/portal_rating/i18n/pl.po` (278 lines)
- `addons/portal_rating/i18n/portal_rating.pot` (250 lines)
- `addons/portal_rating/i18n/pt.po` (274 lines)
- `addons/portal_rating/i18n/pt_BR.po` (270 lines)
- `addons/portal_rating/i18n/ro.po` (280 lines)
- `addons/portal_rating/i18n/ru.po` (268 lines)
- `addons/portal_rating/i18n/sk.po` (265 lines)
- `addons/portal_rating/i18n/sl.po` (267 lines)
- `addons/portal_rating/i18n/sr@latin.po` (266 lines)
- `addons/portal_rating/i18n/sv.po` (264 lines)
- `addons/portal_rating/i18n/th.po` (264 lines)
- `addons/portal_rating/i18n/tr.po` (275 lines)
- `addons/portal_rating/i18n/uk.po` (275 lines)
- `addons/portal_rating/i18n/uz.po` (288 lines)
- `addons/portal_rating/i18n/vi.po` (267 lines)
- `addons/portal_rating/i18n/zh_CN.po` (267 lines)
- `addons/portal_rating/i18n/zh_TW.po` (263 lines)
- `addons/portal_rating/models/__init__.py` (5 lines)
- `addons/portal_rating/models/ir_http.py` (13 lines)
- `addons/portal_rating/models/mail_message.py` (69 lines)
- `addons/portal_rating/models/rating_rating.py` (54 lines)
- `addons/portal_rating/static/src/chatter/portal/@types/models.d.ts` (7 lines)
- `addons/portal_rating/static/src/chatter/portal/chatter_patch.js` (69 lines)
- `addons/portal_rating/static/src/chatter/portal/composer_model_patch.js` (8 lines)
- `addons/portal_rating/static/src/chatter/portal/composer_patch.js` (101 lines)
- `addons/portal_rating/static/src/chatter/portal/composer_patch.xml` (20 lines)
- `addons/portal_rating/static/src/chatter/portal/message_model_patch.js` (32 lines)
- `addons/portal_rating/static/src/chatter/portal/message_patch.js` (117 lines)
- `addons/portal_rating/static/src/chatter/portal/message_patch.xml` (79 lines)
- `addons/portal_rating/static/src/chatter/portal/portal_chatter_patch.js` (17 lines)
- `addons/portal_rating/static/src/chatter/portal/portal_chatter_patch.xml` (57 lines)
- `addons/portal_rating/static/src/chatter/portal/portal_chatter_service_patch.js` (15 lines)
- `addons/portal_rating/static/src/chatter/portal/portal_rating_plugin.js` (5 lines)
- `addons/portal_rating/static/src/chatter/portal/store_service_patch.js` (13 lines)
- `addons/portal_rating/static/src/chatter/portal/suggestion_service_patch.js` (12 lines)
- `addons/portal_rating/static/src/chatter/portal/thread_model_patch.js` (55 lines)
- `addons/portal_rating/static/src/chatter/portal/thread_patch.js` (55 lines)
- `addons/portal_rating/static/src/chatter/portal/thread_patch.xml` (18 lines)
- `addons/portal_rating/static/src/core/common/@types/models.d.ts` (16 lines)
- `addons/portal_rating/static/src/core/common/message_model_patch.js` (13 lines)
- `addons/portal_rating/static/src/core/common/rating_model_patch.js` (19 lines)
- `addons/portal_rating/static/src/core/common/res_partner_model_patch.js` (11 lines)
- `addons/portal_rating/static/src/interactions/portal_composer.js` (162 lines)
- `addons/portal_rating/static/src/interactions/portal_rating_composer.js` (137 lines)
- `addons/portal_rating/static/src/scss/portal_rating.scss` (96 lines)
- `addons/portal_rating/static/src/xml/portal_chatter.xml` (16 lines)
- `addons/portal_rating/static/src/xml/portal_rating_composer.xml` (29 lines)
- `addons/portal_rating/static/src/xml/portal_tools.xml` (115 lines)
- `addons/portal_rating/views/portal_templates.xml` (8 lines)
- `addons/portal_rating/views/rating_rating_views.xml` (22 lines)
- `addons/portal_rating/views/rating_templates.xml` (95 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
