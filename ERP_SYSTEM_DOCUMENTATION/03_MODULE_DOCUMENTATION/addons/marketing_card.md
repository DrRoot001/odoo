# Module: marketing_card

- **Module ID:** MOD-360
- **Path:** `addons/marketing_card`
- **Manifest:** `addons/marketing_card/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Generate dynamic shareable cards

No manifest description declared.

Declared dependencies: `link_tracker`, `mass_mailing`, `website`, `base_report_wkhtmltox`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 19 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 8 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 12 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 6 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "link_tracker",
    "mass_mailing",
    "website",
    "base_report_wkhtmltox"
  ],
  "data": [
    "security/marketing_card_groups.xml",
    "views/card_card_templates.xml",
    "data/card_template_data.xml",
    "views/card_card_views.xml",
    "views/card_campaign_views.xml",
    "views/card_frontend_templates.xml",
    "views/card_template_views.xml",
    "views/card_menus.xml",
    "views/mailing_mailing_views.xml",
    "views/website_templates.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "demo/card_campaign_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "marketing_card/static/src/scss/*"
    ],
    "web.assets_frontend": [
      "marketing_card/static/src/scss/frontend/*.scss",
      "marketing_card/static/src/interactions/*",
      "marketing_card/static/src/scss/linkedin_share_composer.scss"
    ]
  }
}
```

### Representative source files

- `addons/marketing_card/__init__.py` (3 lines)
- `addons/marketing_card/__manifest__.py` (39 lines)
- `addons/marketing_card/controllers/__init__.py` (2 lines)
- `addons/marketing_card/controllers/marketing_card.py` (114 lines)
- `addons/marketing_card/controllers/marketing_card_linkedin.py` (104 lines)
- `addons/marketing_card/data/card_template_data.xml` (118 lines)
- `addons/marketing_card/data/utm_source_data.xml` (5 lines)
- `addons/marketing_card/demo/card_campaign_demo.xml` (36 lines)
- `addons/marketing_card/i18n/ar.po` (1,292 lines)
- `addons/marketing_card/i18n/az.po` (1,268 lines)
- `addons/marketing_card/i18n/bg.po` (1,269 lines)
- `addons/marketing_card/i18n/bs.po` (1,259 lines)
- `addons/marketing_card/i18n/ca.po` (1,293 lines)
- `addons/marketing_card/i18n/cs.po` (1,274 lines)
- `addons/marketing_card/i18n/da.po` (1,271 lines)
- `addons/marketing_card/i18n/de.po` (1,318 lines)
- `addons/marketing_card/i18n/el.po` (1,270 lines)
- `addons/marketing_card/i18n/es.po` (1,299 lines)
- `addons/marketing_card/i18n/es_419.po` (1,316 lines)
- `addons/marketing_card/i18n/et.po` (1,269 lines)
- `addons/marketing_card/i18n/fa.po` (1,269 lines)
- `addons/marketing_card/i18n/fi.po` (1,293 lines)
- `addons/marketing_card/i18n/fr.po` (1,310 lines)
- `addons/marketing_card/i18n/he.po` (1,269 lines)
- `addons/marketing_card/i18n/hi.po` (1,268 lines)
- `addons/marketing_card/i18n/hr.po` (1,269 lines)
- `addons/marketing_card/i18n/hu.po` (1,269 lines)
- `addons/marketing_card/i18n/id.po` (1,294 lines)
- `addons/marketing_card/i18n/it.po` (1,310 lines)
- `addons/marketing_card/i18n/ja.po` (1,308 lines)
- `addons/marketing_card/i18n/kab.po` (1,258 lines)
- `addons/marketing_card/i18n/ko.po` (1,290 lines)
- `addons/marketing_card/i18n/ku.po` (1,268 lines)
- `addons/marketing_card/i18n/lo.po` (1,295 lines)
- `addons/marketing_card/i18n/lt.po` (1,270 lines)
- `addons/marketing_card/i18n/lv.po` (1,258 lines)
- `addons/marketing_card/i18n/marketing_card.pot` (1,253 lines)
- `addons/marketing_card/i18n/mn.po` (1,268 lines)
- `addons/marketing_card/i18n/my.po` (1,259 lines)
- `addons/marketing_card/i18n/nb.po` (1,269 lines)
- `addons/marketing_card/i18n/nl.po` (1,306 lines)
- `addons/marketing_card/i18n/pl.po` (1,298 lines)
- `addons/marketing_card/i18n/pt.po` (1,293 lines)
- `addons/marketing_card/i18n/pt_BR.po` (1,333 lines)
- `addons/marketing_card/i18n/ro.po` (1,294 lines)
- `addons/marketing_card/i18n/ru.po` (1,298 lines)
- `addons/marketing_card/i18n/sk.po` (1,257 lines)
- `addons/marketing_card/i18n/sl.po` (1,270 lines)
- `addons/marketing_card/i18n/sr@latin.po` (1,269 lines)
- `addons/marketing_card/i18n/sv.po` (1,276 lines)
- `addons/marketing_card/i18n/th.po` (1,284 lines)
- `addons/marketing_card/i18n/tr.po` (1,298 lines)
- `addons/marketing_card/i18n/uk.po` (1,269 lines)
- `addons/marketing_card/i18n/uz.po` (1,473 lines)
- `addons/marketing_card/i18n/vi.po` (1,291 lines)
- `addons/marketing_card/i18n/zh_CN.po` (1,290 lines)
- `addons/marketing_card/i18n/zh_TW.po` (1,290 lines)
- `addons/marketing_card/models/__init__.py` (7 lines)
- `addons/marketing_card/models/card_campaign.py` (527 lines)
- `addons/marketing_card/models/card_campaign_tag.py` (19 lines)
- `addons/marketing_card/models/card_card.py` (65 lines)
- `addons/marketing_card/models/card_template.py` (22 lines)
- `addons/marketing_card/models/ir_model.py` (12 lines)
- `addons/marketing_card/models/mailing_mailing.py` (119 lines)
- `addons/marketing_card/models/utm_source.py` (14 lines)
- `addons/marketing_card/security/ir.access.csv` (11 lines)
- `addons/marketing_card/security/marketing_card_groups.xml` (23 lines)
- `addons/marketing_card/static/card_backgrounds/Blur.png` (380 lines)
- `addons/marketing_card/static/card_backgrounds/Circles.png` (123 lines)
- `addons/marketing_card/static/card_backgrounds/Desert.png` (228 lines)
- `addons/marketing_card/static/card_backgrounds/Drawings.png` (195 lines)
- `addons/marketing_card/static/card_backgrounds/Geometric.png` (147 lines)
- `addons/marketing_card/static/card_backgrounds/Highlight.png` (72 lines)
- `addons/marketing_card/static/card_backgrounds/Image.jpg` (714 lines)
- `addons/marketing_card/static/card_backgrounds/Image.png` (1,300 lines)
- `addons/marketing_card/static/card_backgrounds/Lila.png` (86 lines)
- `addons/marketing_card/static/card_backgrounds/Lines.png` (698 lines)
- `addons/marketing_card/static/card_backgrounds/Organic.png` (111 lines)
- `addons/marketing_card/static/card_backgrounds/Waves.png` (86 lines)
- `addons/marketing_card/static/card_backgrounds/WorldMap.png` (375 lines)
- `addons/marketing_card/static/description/icon.png` (6 lines)
- `addons/marketing_card/static/description/icon.svg` (1 lines)
- `addons/marketing_card/static/src/interactions/linkedin_message_editor.js` (25 lines)
- `addons/marketing_card/static/src/scss/card_campaign.scss` (19 lines)
- `addons/marketing_card/static/src/scss/frontend/card_website.scss` (29 lines)
- `addons/marketing_card/static/src/scss/linkedin_share_composer.scss` (11 lines)
- `addons/marketing_card/tests/__init__.py` (1 lines)
- `addons/marketing_card/tests/common.py` (141 lines)
- `addons/marketing_card/tests/test_campaign.py` (550 lines)
- `addons/marketing_card/utils/linkedin_api.py` (193 lines)
- `addons/marketing_card/views/card_campaign_views.xml` (231 lines)
- `addons/marketing_card/views/card_card_templates.xml` (573 lines)
- `addons/marketing_card/views/card_card_views.xml` (55 lines)
- `addons/marketing_card/views/card_frontend_templates.xml` (125 lines)
- `addons/marketing_card/views/card_menus.xml` (28 lines)
- `addons/marketing_card/views/card_template_views.xml` (38 lines)
- `addons/marketing_card/views/mailing_mailing_views.xml` (28 lines)
- `addons/marketing_card/views/website_templates.xml` (12 lines)
- `addons/marketing_card/wizards/__init__.py` (1 lines)
- `addons/marketing_card/wizards/mail_compose_message.py` (66 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
