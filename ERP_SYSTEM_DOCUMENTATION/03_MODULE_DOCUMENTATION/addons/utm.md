# Module: utm

- **Module ID:** MOD-591
- **Path:** `addons/utm`
- **Manifest:** `addons/utm/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Enable management of UTM trackers: campaign, medium, source.


Declared dependencies: `base`, `web`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 16 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 8 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 12 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 6 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base",
    "web"
  ],
  "data": [
    "data/utm_medium_data.xml",
    "data/utm_source_data.xml",
    "data/utm_stage_data.xml",
    "data/utm_tag_data.xml",
    "views/utm_campaign_views.xml",
    "views/utm_medium_views.xml",
    "views/utm_source_views.xml",
    "views/utm_stage_views.xml",
    "views/utm_tag_views.xml",
    "views/utm_menus.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/utm_campaign_demo.xml",
    "data/utm_stage_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "utm/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/utm/__init__.py` (4 lines)
- `addons/utm/__manifest__.py` (35 lines)
- `addons/utm/data/utm_campaign_demo.xml` (15 lines)
- `addons/utm/data/utm_medium_data.xml` (21 lines)
- `addons/utm/data/utm_source_data.xml` (46 lines)
- `addons/utm/data/utm_stage_data.xml` (9 lines)
- `addons/utm/data/utm_stage_demo.xml` (17 lines)
- `addons/utm/data/utm_tag_data.xml` (8 lines)
- `addons/utm/i18n/af.po` (677 lines)
- `addons/utm/i18n/ar.po` (702 lines)
- `addons/utm/i18n/az.po` (685 lines)
- `addons/utm/i18n/bg.po` (697 lines)
- `addons/utm/i18n/bs.po` (681 lines)
- `addons/utm/i18n/ca.po` (715 lines)
- `addons/utm/i18n/cs.po` (693 lines)
- `addons/utm/i18n/da.po` (694 lines)
- `addons/utm/i18n/de.po` (717 lines)
- `addons/utm/i18n/el.po` (682 lines)
- `addons/utm/i18n/es.po` (712 lines)
- `addons/utm/i18n/es_419.po` (704 lines)
- `addons/utm/i18n/es_CL.po` (90 lines)
- `addons/utm/i18n/et.po` (714 lines)
- `addons/utm/i18n/eu.po` (675 lines)
- `addons/utm/i18n/fa.po` (702 lines)
- `addons/utm/i18n/fi.po` (715 lines)
- `addons/utm/i18n/fo.po` (675 lines)
- `addons/utm/i18n/fr.po` (714 lines)
- `addons/utm/i18n/fr_BE.po` (72 lines)
- `addons/utm/i18n/fr_CA.po` (83 lines)
- `addons/utm/i18n/gl.po` (675 lines)
- `addons/utm/i18n/gu.po` (677 lines)
- `addons/utm/i18n/he.po` (694 lines)
- `addons/utm/i18n/hi.po` (679 lines)
- `addons/utm/i18n/hr.po` (705 lines)
- `addons/utm/i18n/hu.po` (690 lines)
- `addons/utm/i18n/id.po` (709 lines)
- `addons/utm/i18n/is.po` (673 lines)
- `addons/utm/i18n/it.po` (711 lines)
- `addons/utm/i18n/ja.po` (709 lines)
- `addons/utm/i18n/ka.po` (675 lines)
- `addons/utm/i18n/kab.po` (677 lines)
- `addons/utm/i18n/km.po` (677 lines)
- `addons/utm/i18n/ko.po` (701 lines)
- `addons/utm/i18n/ku.po` (677 lines)
- `addons/utm/i18n/lo.po` (699 lines)
- `addons/utm/i18n/lt.po` (695 lines)
- `addons/utm/i18n/lv.po` (683 lines)
- `addons/utm/i18n/mk.po` (677 lines)
- `addons/utm/i18n/ml_IN.po` (676 lines)
- `addons/utm/i18n/mn.po` (689 lines)
- `addons/utm/i18n/my.po` (678 lines)
- `addons/utm/i18n/nb.po` (686 lines)
- `addons/utm/i18n/nl.po` (710 lines)
- `addons/utm/i18n/pl.po` (718 lines)
- `addons/utm/i18n/pt.po` (707 lines)
- `addons/utm/i18n/pt_BR.po` (714 lines)
- `addons/utm/i18n/ro.po` (694 lines)
- `addons/utm/i18n/ru.po` (708 lines)
- `addons/utm/i18n/sk.po` (692 lines)
- `addons/utm/i18n/sl.po` (690 lines)
- `addons/utm/i18n/sq.po` (675 lines)
- `addons/utm/i18n/sr@latin.po` (685 lines)
- `addons/utm/i18n/sv.po` (715 lines)
- `addons/utm/i18n/ta.po` (678 lines)
- `addons/utm/i18n/th.po` (689 lines)
- `addons/utm/i18n/tr.po` (719 lines)
- `addons/utm/i18n/uk.po` (707 lines)
- `addons/utm/i18n/utm.pot` (673 lines)
- `addons/utm/i18n/uz.po` (817 lines)
- `addons/utm/i18n/vi.po` (708 lines)
- `addons/utm/i18n/zh_CN.po` (692 lines)
- `addons/utm/i18n/zh_TW.po` (685 lines)
- `addons/utm/models/__init__.py` (10 lines)
- `addons/utm/models/ir_http.py` (26 lines)
- `addons/utm/models/utm_campaign.py` (61 lines)
- `addons/utm/models/utm_medium.py` (45 lines)
- `addons/utm/models/utm_mixin.py` (255 lines)
- `addons/utm/models/utm_source.py` (59 lines)
- `addons/utm/models/utm_stage.py` (16 lines)
- `addons/utm/models/utm_tag.py` (27 lines)
- `addons/utm/security/ir.access.csv` (11 lines)
- `addons/utm/static/description/icon.png` (14 lines)
- `addons/utm/static/description/icon.svg` (1 lines)
- `addons/utm/static/description/icon_hi.png` (42 lines)
- `addons/utm/static/src/js/utm_campaign_kanban_examples.js` (30 lines)
- `addons/utm/static/src/scss/utm_views.scss` (12 lines)
- `addons/utm/tests/__init__.py` (8 lines)
- `addons/utm/tests/common.py` (23 lines)
- `addons/utm/tests/test_routes.py` (15 lines)
- `addons/utm/tests/test_utm.py` (196 lines)
- `addons/utm/tests/test_utm_consistency.py` (51 lines)
- `addons/utm/tests/test_utm_security.py` (79 lines)
- `addons/utm/views/utm_campaign_views.xml` (133 lines)
- `addons/utm/views/utm_medium_views.xml` (54 lines)
- `addons/utm/views/utm_menus.xml` (31 lines)
- `addons/utm/views/utm_source_views.xml` (39 lines)
- `addons/utm/views/utm_stage_views.xml` (53 lines)
- `addons/utm/views/utm_tag_views.xml` (24 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
