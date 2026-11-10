# Module: digest

- **Module ID:** MOD-063
- **Path:** `addons/digest`
- **Manifest:** `addons/digest/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Send KPI Digests periodically
=============================


Declared dependencies: `mail`, `portal`, `resource`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 14 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 8 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 3 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mail",
    "portal",
    "resource"
  ],
  "data": [
    "data/digest_data.xml",
    "data/digest_tips_data.xml",
    "data/ir_cron_data.xml",
    "data/res_config_settings_data.xml",
    "views/digest_views.xml",
    "views/digest_templates.xml",
    "views/res_config_settings_views.xml",
    "wizard/digest_test_views.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/digest/__init__.py` (6 lines)
- `addons/digest/__manifest__.py` (28 lines)
- `addons/digest/controllers/__init__.py` (4 lines)
- `addons/digest/controllers/portal.py` (73 lines)
- `addons/digest/data/digest_data.xml` (528 lines)
- `addons/digest/data/digest_tips_data.xml` (100 lines)
- `addons/digest/data/ir_cron_data.xml` (13 lines)
- `addons/digest/data/res_config_settings_data.xml` (11 lines)
- `addons/digest/i18n/ar.po` (675 lines)
- `addons/digest/i18n/az.po` (660 lines)
- `addons/digest/i18n/bg.po` (643 lines)
- `addons/digest/i18n/bs.po` (648 lines)
- `addons/digest/i18n/ca.po` (683 lines)
- `addons/digest/i18n/cs.po` (657 lines)
- `addons/digest/i18n/da.po` (671 lines)
- `addons/digest/i18n/de.po` (688 lines)
- `addons/digest/i18n/digest.pot` (638 lines)
- `addons/digest/i18n/el.po` (649 lines)
- `addons/digest/i18n/es.po` (684 lines)
- `addons/digest/i18n/es_419.po` (682 lines)
- `addons/digest/i18n/et.po` (686 lines)
- `addons/digest/i18n/fa.po` (678 lines)
- `addons/digest/i18n/fi.po` (692 lines)
- `addons/digest/i18n/fr.po` (692 lines)
- `addons/digest/i18n/gu.po` (643 lines)
- `addons/digest/i18n/he.po` (671 lines)
- `addons/digest/i18n/hi.po` (667 lines)
- `addons/digest/i18n/hr.po` (657 lines)
- `addons/digest/i18n/hu.po` (653 lines)
- `addons/digest/i18n/id.po` (677 lines)
- `addons/digest/i18n/is.po` (639 lines)
- `addons/digest/i18n/it.po` (687 lines)
- `addons/digest/i18n/ja.po` (673 lines)
- `addons/digest/i18n/kab.po` (644 lines)
- `addons/digest/i18n/km.po` (644 lines)
- `addons/digest/i18n/ko.po` (669 lines)
- `addons/digest/i18n/ku.po` (643 lines)
- `addons/digest/i18n/lo.po` (656 lines)
- `addons/digest/i18n/lt.po` (658 lines)
- `addons/digest/i18n/lv.po` (645 lines)
- `addons/digest/i18n/mn.po` (653 lines)
- `addons/digest/i18n/my.po` (644 lines)
- `addons/digest/i18n/nb.po` (649 lines)
- `addons/digest/i18n/nl.po` (686 lines)
- `addons/digest/i18n/pl.po` (691 lines)
- `addons/digest/i18n/pt.po` (682 lines)
- `addons/digest/i18n/pt_BR.po` (685 lines)
- `addons/digest/i18n/ro.po` (681 lines)
- `addons/digest/i18n/ru.po` (679 lines)
- `addons/digest/i18n/sk.po` (648 lines)
- `addons/digest/i18n/sl.po` (673 lines)
- `addons/digest/i18n/sr@latin.po` (671 lines)
- `addons/digest/i18n/sv.po` (675 lines)
- `addons/digest/i18n/th.po` (664 lines)
- `addons/digest/i18n/tr.po` (691 lines)
- `addons/digest/i18n/uk.po` (677 lines)
- `addons/digest/i18n/uz.po` (781 lines)
- `addons/digest/i18n/vi.po` (672 lines)
- `addons/digest/i18n/zh_CN.po` (668 lines)
- `addons/digest/i18n/zh_TW.po` (663 lines)
- `addons/digest/models/__init__.py` (7 lines)
- `addons/digest/models/digest.py` (571 lines)
- `addons/digest/models/digest_tip.py` (22 lines)
- `addons/digest/models/res_config_settings.py` (10 lines)
- `addons/digest/models/res_users.py` (19 lines)
- `addons/digest/security/ir.access.csv` (6 lines)
- `addons/digest/static/src/img/app_store.png` (105 lines)
- `addons/digest/static/src/img/google_play.png` (112 lines)
- `addons/digest/static/src/img/milk-alt-shortcuts.gif` (214 lines)
- `addons/digest/static/src/img/milk-avatar.gif` (355 lines)
- `addons/digest/static/src/img/milk-calculator.gif` (158 lines)
- `addons/digest/static/src/img/milk-ctrl+k.gif` (649 lines)
- `addons/digest/static/src/img/milk-following.png` (140 lines)
- `addons/digest/static/src/img/milk-notifications.png` (130 lines)
- `addons/digest/tests/__init__.py` (4 lines)
- `addons/digest/tests/common.py` (78 lines)
- `addons/digest/tests/test_digest.py` (385 lines)
- `addons/digest/views/digest_templates.xml` (17 lines)
- `addons/digest/views/digest_views.xml` (158 lines)
- `addons/digest/views/res_config_settings_views.xml` (24 lines)
- `addons/digest/wizard/__init__.py` (3 lines)
- `addons/digest/wizard/digest_test.py` (18 lines)
- `addons/digest/wizard/digest_test_views.xml` (18 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
