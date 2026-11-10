# Module: rating

- **Module ID:** MOD-504
- **Path:** `addons/rating`
- **Manifest:** `addons/rating/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This module allows a customer to give rating.


Declared dependencies: `mail`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 14 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 7 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 9 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 2 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mail"
  ],
  "data": [
    "views/rating_rating_views.xml",
    "views/rating_templates.xml",
    "views/mail_message_views.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "rating/static/src/core/common/**/*",
      "rating/static/src/core/web/**/*"
    ],
    "web.assets_frontend": [
      "rating/static/src/scss/rating_templates.scss"
    ],
    "web.assets_unit_tests": [
      "rating/static/tests/**/*"
    ],
    "im_livechat.assets_embed_core": [
      "rating/static/src/core/common/**/*"
    ],
    "mail.assets_public": [
      "rating/static/src/core/common/**/*"
    ],
    "portal.assets_chatter_helpers": [
      "rating/static/src/core/common/**/*"
    ]
  }
}
```

### Representative source files

- `addons/rating/__init__.py` (5 lines)
- `addons/rating/__manifest__.py` (42 lines)
- `addons/rating/controllers/__init__.py` (3 lines)
- `addons/rating/controllers/main.py` (98 lines)
- `addons/rating/i18n/af.po` (603 lines)
- `addons/rating/i18n/am.po` (599 lines)
- `addons/rating/i18n/ar.po` (614 lines)
- `addons/rating/i18n/az.po` (607 lines)
- `addons/rating/i18n/bg.po` (611 lines)
- `addons/rating/i18n/bs.po` (607 lines)
- `addons/rating/i18n/ca.po` (624 lines)
- `addons/rating/i18n/cs.po` (612 lines)
- `addons/rating/i18n/da.po` (614 lines)
- `addons/rating/i18n/de.po` (621 lines)
- `addons/rating/i18n/el.po` (608 lines)
- `addons/rating/i18n/es.po` (621 lines)
- `addons/rating/i18n/es_419.po` (614 lines)
- `addons/rating/i18n/es_CL.po` (63 lines)
- `addons/rating/i18n/et.po` (623 lines)
- `addons/rating/i18n/eu.po` (601 lines)
- `addons/rating/i18n/fa.po` (616 lines)
- `addons/rating/i18n/fi.po` (622 lines)
- `addons/rating/i18n/fo.po` (601 lines)
- `addons/rating/i18n/fr.po` (620 lines)
- `addons/rating/i18n/fr_BE.po` (43 lines)
- `addons/rating/i18n/fr_CA.po` (63 lines)
- `addons/rating/i18n/gl.po` (601 lines)
- `addons/rating/i18n/gu.po` (603 lines)
- `addons/rating/i18n/he.po` (614 lines)
- `addons/rating/i18n/hi.po` (603 lines)
- `addons/rating/i18n/hr.po` (612 lines)
- `addons/rating/i18n/hu.po` (612 lines)
- `addons/rating/i18n/id.po` (617 lines)
- `addons/rating/i18n/is.po` (599 lines)
- `addons/rating/i18n/it.po` (621 lines)
- `addons/rating/i18n/ja.po` (614 lines)
- `addons/rating/i18n/ka.po` (601 lines)
- `addons/rating/i18n/kab.po` (603 lines)
- `addons/rating/i18n/km.po` (604 lines)
- `addons/rating/i18n/ko.po` (611 lines)
- `addons/rating/i18n/ku.po` (603 lines)
- `addons/rating/i18n/lo.po` (607 lines)
- `addons/rating/i18n/lt.po` (615 lines)
- `addons/rating/i18n/lv.po` (612 lines)
- `addons/rating/i18n/mk.po` (607 lines)
- `addons/rating/i18n/ml_IN.po` (602 lines)
- `addons/rating/i18n/mn.po` (613 lines)
- `addons/rating/i18n/my.po` (604 lines)
- `addons/rating/i18n/nb.po` (607 lines)
- `addons/rating/i18n/nl.po` (617 lines)
- `addons/rating/i18n/pl.po` (632 lines)
- `addons/rating/i18n/pt.po` (626 lines)
- `addons/rating/i18n/pt_BR.po` (622 lines)
- `addons/rating/i18n/rating.pot` (596 lines)
- `addons/rating/i18n/ro.po` (618 lines)
- `addons/rating/i18n/ru.po` (619 lines)
- `addons/rating/i18n/sk.po` (611 lines)
- `addons/rating/i18n/sl.po` (613 lines)
- `addons/rating/i18n/sq.po` (601 lines)
- `addons/rating/i18n/sr@latin.po` (608 lines)
- `addons/rating/i18n/sv.po` (623 lines)
- `addons/rating/i18n/ta.po` (601 lines)
- `addons/rating/i18n/th.po` (611 lines)
- `addons/rating/i18n/tr.po` (627 lines)
- `addons/rating/i18n/uk.po` (616 lines)
- `addons/rating/i18n/uz.po` (707 lines)
- `addons/rating/i18n/vi.po` (610 lines)
- `addons/rating/i18n/zh_CN.po` (615 lines)
- `addons/rating/i18n/zh_TW.po` (610 lines)
- `addons/rating/models/__init__.py` (8 lines)
- `addons/rating/models/mail_message.py` (71 lines)
- `addons/rating/models/mail_thread.py` (219 lines)
- `addons/rating/models/rating.py` (211 lines)
- `addons/rating/models/rating_data.py` (87 lines)
- `addons/rating/models/rating_mixin.py` (240 lines)
- `addons/rating/models/rating_parent_mixin.py` (71 lines)
- `addons/rating/security/ir.access.csv` (3 lines)
- `addons/rating/static/src/core/common/@types/models.d.ts` (21 lines)
- `addons/rating/static/src/core/common/message_model_patch.js` (19 lines)
- `addons/rating/static/src/core/common/rating_model.js` (23 lines)
- `addons/rating/static/src/core/common/thread_model_patch.js` (17 lines)
- `addons/rating/static/src/core/web/messaging_menu_item_patch.js` (16 lines)
- `addons/rating/static/src/core/web/messaging_menu_item_patch.scss` (4 lines)
- `addons/rating/static/src/core/web/notification_item_patch.js` (16 lines)
- `addons/rating/static/src/core/web/notification_item_patch.xml` (12 lines)
- `addons/rating/static/src/img/503.svg` (34 lines)
- `addons/rating/static/src/img/rating_0.png` (15 lines)
- `addons/rating/static/src/img/rating_0_white.png` (17 lines)
- `addons/rating/static/src/img/rating_1.png` (19 lines)
- `addons/rating/static/src/img/rating_1.svg` (1 lines)
- `addons/rating/static/src/img/rating_1_white.png` (19 lines)
- `addons/rating/static/src/img/rating_3.png` (21 lines)
- `addons/rating/static/src/img/rating_3.svg` (1 lines)
- `addons/rating/static/src/img/rating_3_white.png` (14 lines)
- `addons/rating/static/src/img/rating_5.png` (12 lines)
- `addons/rating/static/src/img/rating_5.svg` (1 lines)
- `addons/rating/static/src/img/rating_5_white.png` (11 lines)
- `addons/rating/static/src/scss/rating_rating_views.scss` (5 lines)
- `addons/rating/static/src/scss/rating_templates.scss` (36 lines)
- `addons/rating/static/tests/mock_server/models/mail_message.js` (18 lines)
- `addons/rating/static/tests/mock_server/models/rating_rating.js` (11 lines)
- `addons/rating/static/tests/rating_test_helpers.js` (5 lines)
- `addons/rating/tests/__init__.py` (5 lines)
- `addons/rating/tests/test_controller.py` (57 lines)
- `addons/rating/tests/test_security.py` (76 lines)
- `addons/rating/views/mail_message_views.xml` (15 lines)
- `addons/rating/views/rating_rating_views.xml` (246 lines)
- `addons/rating/views/rating_templates.xml` (89 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
