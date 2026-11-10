# Module: mass_mailing_themes

- **Module ID:** MOD-373
- **Path:** `addons/mass_mailing_themes`
- **Manifest:** `addons/mass_mailing_themes/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Design gorgeous mails


Design gorgeous mails
    

Declared dependencies: `mass_mailing`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 2 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mass_mailing"
  ],
  "data": [
    "data/ir_attachment_data.xml",
    "views/mass_mailing_themes_templates.xml"
  ]
}
```

### Representative source files

- `addons/mass_mailing_themes/__init__.py` (0 lines)
- `addons/mass_mailing_themes/__manifest__.py` (23 lines)
- `addons/mass_mailing_themes/data/ir_attachment_data.xml` (75 lines)
- `addons/mass_mailing_themes/i18n/ar.po` (2,206 lines)
- `addons/mass_mailing_themes/i18n/az.po` (1,958 lines)
- `addons/mass_mailing_themes/i18n/bg.po` (1,964 lines)
- `addons/mass_mailing_themes/i18n/bs.po` (1,958 lines)
- `addons/mass_mailing_themes/i18n/ca.po` (2,027 lines)
- `addons/mass_mailing_themes/i18n/cs.po` (2,227 lines)
- `addons/mass_mailing_themes/i18n/da.po` (1,962 lines)
- `addons/mass_mailing_themes/i18n/de.po` (2,267 lines)
- `addons/mass_mailing_themes/i18n/el.po` (1,960 lines)
- `addons/mass_mailing_themes/i18n/es.po` (2,244 lines)
- `addons/mass_mailing_themes/i18n/es_419.po` (2,247 lines)
- `addons/mass_mailing_themes/i18n/et.po` (2,084 lines)
- `addons/mass_mailing_themes/i18n/fa.po` (2,188 lines)
- `addons/mass_mailing_themes/i18n/fi.po` (2,242 lines)
- `addons/mass_mailing_themes/i18n/fr.po` (2,259 lines)
- `addons/mass_mailing_themes/i18n/he.po` (1,964 lines)
- `addons/mass_mailing_themes/i18n/hi.po` (1,957 lines)
- `addons/mass_mailing_themes/i18n/hr.po` (1,963 lines)
- `addons/mass_mailing_themes/i18n/hu.po` (1,960 lines)
- `addons/mass_mailing_themes/i18n/id.po` (2,231 lines)
- `addons/mass_mailing_themes/i18n/it.po` (2,241 lines)
- `addons/mass_mailing_themes/i18n/ja.po` (2,206 lines)
- `addons/mass_mailing_themes/i18n/kab.po` (1,956 lines)
- `addons/mass_mailing_themes/i18n/ko.po` (2,204 lines)
- `addons/mass_mailing_themes/i18n/ku.po` (1,955 lines)
- `addons/mass_mailing_themes/i18n/lo.po` (2,264 lines)
- `addons/mass_mailing_themes/i18n/lt.po` (1,964 lines)
- `addons/mass_mailing_themes/i18n/lv.po` (1,959 lines)
- `addons/mass_mailing_themes/i18n/mass_mailing_themes.pot` (1,925 lines)
- `addons/mass_mailing_themes/i18n/mn.po` (1,960 lines)
- `addons/mass_mailing_themes/i18n/my.po` (1,955 lines)
- `addons/mass_mailing_themes/i18n/nb.po` (1,960 lines)
- `addons/mass_mailing_themes/i18n/nl.po` (2,333 lines)
- `addons/mass_mailing_themes/i18n/pl.po` (2,242 lines)
- `addons/mass_mailing_themes/i18n/pt.po` (2,008 lines)
- `addons/mass_mailing_themes/i18n/pt_BR.po` (2,388 lines)
- `addons/mass_mailing_themes/i18n/ro.po` (2,211 lines)
- `addons/mass_mailing_themes/i18n/ru.po` (2,242 lines)
- `addons/mass_mailing_themes/i18n/sk.po` (1,962 lines)
- `addons/mass_mailing_themes/i18n/sl.po` (1,961 lines)
- `addons/mass_mailing_themes/i18n/sr@latin.po` (1,959 lines)
- `addons/mass_mailing_themes/i18n/sv.po` (2,213 lines)
- `addons/mass_mailing_themes/i18n/th.po` (2,159 lines)
- `addons/mass_mailing_themes/i18n/tr.po` (2,235 lines)
- `addons/mass_mailing_themes/i18n/uk.po` (2,204 lines)
- `addons/mass_mailing_themes/i18n/uz.po` (2,410 lines)
- `addons/mass_mailing_themes/i18n/vi.po` (2,248 lines)
- `addons/mass_mailing_themes/i18n/zh_CN.po` (2,185 lines)
- `addons/mass_mailing_themes/i18n/zh_TW.po` (2,144 lines)
- `addons/mass_mailing_themes/static/src/img/theme_bignews/s_default_image_logo.png` (21 lines)
- `addons/mass_mailing_themes/static/src/img/theme_bignews/s_picture_default_image_2.jpg` (256 lines)
- `addons/mass_mailing_themes/static/src/img/theme_bignews/set_ui_landscape_sm_1.webp` (35 lines)
- `addons/mass_mailing_themes/static/src/img/theme_bignews/set_ui_landscape_sm_2.webp` (38 lines)
- `addons/mass_mailing_themes/static/src/img/theme_bignews/set_ui_landscape_sm_3.webp` (84 lines)
- `addons/mass_mailing_themes/static/src/img/theme_bignews/set_ui_landscape_sm_4.webp` (85 lines)
- `addons/mass_mailing_themes/static/src/img/theme_blogging/s_default_image_media_list_1.jpg` (72 lines)
- `addons/mass_mailing_themes/static/src/img/theme_blogging/s_default_image_media_list_2.jpg` (39 lines)
- `addons/mass_mailing_themes/static/src/img/theme_blogging/s_default_image_media_list_3.jpg` (103 lines)
- `addons/mass_mailing_themes/static/src/img/theme_blogging/s_tech_default_image.jpg` (427 lines)
- `addons/mass_mailing_themes/static/src/img/theme_blogging/tech_logo.png` (41 lines)
- `addons/mass_mailing_themes/static/src/img/theme_coffeebreak/s_default_image_block_banner.jpg` (349 lines)
- `addons/mass_mailing_themes/static/src/img/theme_coffeebreak/s_default_image_block_image_text.jpg` (132 lines)
- `addons/mass_mailing_themes/static/src/img/theme_coffeebreak/s_default_image_logo.png` (117 lines)
- `addons/mass_mailing_themes/static/src/img/theme_coupon/company_logo.png` (18 lines)
- `addons/mass_mailing_themes/static/src/img/theme_cta_centric/company_logo_dark.png` (50 lines)
- `addons/mass_mailing_themes/static/src/img/theme_cta_centric/s_bento_block_default_image_1.webp` (115 lines)
- `addons/mass_mailing_themes/static/src/img/theme_cta_centric/s_bento_block_default_image_2.webp` (181 lines)
- `addons/mass_mailing_themes/static/src/img/theme_event/s_cover_default_image.jpg` (654 lines)
- `addons/mass_mailing_themes/static/src/img/theme_event/s_default_image_logo.png` (13 lines)
- `addons/mass_mailing_themes/static/src/img/theme_event/s_default_image_media_list_1.jpg` (62 lines)
- `addons/mass_mailing_themes/static/src/img/theme_event/s_default_image_media_list_2.jpg` (111 lines)
- `addons/mass_mailing_themes/static/src/img/theme_event/s_default_image_media_list_3.jpg` (75 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/bignews_thumb_large.webp` (90 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/bignews_thumb_logo.png` (16 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/bignews_thumb_small.webp` (21 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/blogging_thumb_large.webp` (201 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/blogging_thumb_logo.png` (19 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/blogging_thumb_small.webp` (25 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/catalog_thumb_large.webp` (100 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/catalog_thumb_small.webp` (14 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/coffee_break_thumb_large.webp` (142 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/coffee_break_thumb_logo.png` (4 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/coffee_break_thumb_small.webp` (24 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/coupon_thumb_large.webp` (94 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/coupon_thumb_logo.png` (14 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/coupon_thumb_small.webp` (12 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/event_thumb_large.webp` (159 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/event_thumb_logo.png` (19 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/event_thumb_small.webp` (35 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/event_updates_thumb_large.webp` (59 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/event_updates_thumb_small.webp` (15 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/magazine_thumb_large.webp` (211 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/magazine_thumb_logo.png` (14 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/magazine_thumb_small.webp` (23 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/newsletter_thumb_large.webp` (312 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/newsletter_thumb_logo.png` (5 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/newsletter_thumb_small.webp` (34 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/promotion_thumb_large.webp` (149 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/promotion_thumb_logo.png` (17 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/promotion_thumb_small.webp` (24 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/roadshow_followup_thumb_large.webp` (189 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/roadshow_followup_thumb_small.webp` (13 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/roadshow_schedule_thumb_large.webp` (148 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/roadshow_schedule_thumb_small.webp` (19 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/roadshow_thumb_logo.png` (6 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/terms_thumb_large.webp` (158 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/terms_thumb_small.webp` (18 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/training_thumb_large.webp` (125 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/training_thumb_logo.png` (5 lines)
- `addons/mass_mailing_themes/static/src/img/theme_imgs/training_thumb_small.webp` (25 lines)
- `addons/mass_mailing_themes/static/src/img/theme_magazine/s_default_image_image_text.jpg` (160 lines)
- `addons/mass_mailing_themes/static/src/img/theme_magazine/s_default_image_image_text_2.jpg` (339 lines)
- `addons/mass_mailing_themes/static/src/img/theme_magazine/s_default_image_product_1.jpg` (209 lines)
- `addons/mass_mailing_themes/static/src/img/theme_magazine/s_default_image_product_2.jpg` (171 lines)
- `addons/mass_mailing_themes/static/src/img/theme_newsletter/FPsignature.gif` (28 lines)
- `addons/mass_mailing_themes/static/src/img/theme_newsletter/s_default_image_block_banner.jpg` (707 lines)
- `addons/mass_mailing_themes/static/src/img/theme_newsletter/s_default_image_block_banner_2.jpg` (227 lines)
- `addons/mass_mailing_themes/static/src/img/theme_newsletter/s_default_image_block_banner_3.jpg` (247 lines)
- `addons/mass_mailing_themes/static/src/img/theme_newsletter/social-facebook.png` (16 lines)
- `addons/mass_mailing_themes/static/src/img/theme_newsletter/social-linkedin.png` (19 lines)
- `addons/mass_mailing_themes/static/src/img/theme_newsletter/social-twitter.png` (9 lines)
- `addons/mass_mailing_themes/static/src/img/theme_promotion/company_logo.png` (24 lines)
- `addons/mass_mailing_themes/static/src/img/theme_promotion/company_logo_dark.png` (20 lines)
- `addons/mass_mailing_themes/static/src/img/theme_promotion/s_picture_default_image.jpg` (647 lines)
- `addons/mass_mailing_themes/static/src/img/theme_training/s_default_image_block_banner.jpg` (617 lines)
- `addons/mass_mailing_themes/static/src/img/theme_training/s_default_image_block_image.jpg` (266 lines)
- `addons/mass_mailing_themes/static/src/img/theme_training/see_you_soon.svg` (38 lines)
- `addons/mass_mailing_themes/static/src/img/theme_vip/vip_logo.png` (52 lines)
- `addons/mass_mailing_themes/views/mass_mailing_themes_templates.xml` (2,158 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
