# Module: maintenance

- **Module ID:** MOD-359
- **Path:** `addons/maintenance`
- **Manifest:** `addons/maintenance/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Track equipment and manage maintenance requests


Track equipment and maintenance requests

Declared dependencies: `mail`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 9 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 9 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mail"
  ],
  "data": [
    "security/maintenance.xml",
    "data/maintenance_data.xml",
    "data/mail_activity_type_data.xml",
    "data/mail_message_subtype_data.xml",
    "views/maintenance_views.xml",
    "views/mail_activity_views.xml",
    "views/res_config_settings_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/maintenance_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "maintenance/static/src/**/*"
    ],
    "web.assets_tests": [
      "maintenance/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/maintenance/__init__.py` (4 lines)
- `addons/maintenance/__manifest__.py` (33 lines)
- `addons/maintenance/data/mail_activity_type_data.xml` (12 lines)
- `addons/maintenance/data/mail_message_subtype_data.xml` (45 lines)
- `addons/maintenance/data/maintenance_data.xml` (28 lines)
- `addons/maintenance/data/maintenance_demo.xml` (149 lines)
- `addons/maintenance/i18n/af.po` (1,639 lines)
- `addons/maintenance/i18n/am.po` (1,635 lines)
- `addons/maintenance/i18n/ar.po` (1,686 lines)
- `addons/maintenance/i18n/az.po` (1,677 lines)
- `addons/maintenance/i18n/bg.po` (1,685 lines)
- `addons/maintenance/i18n/bs.po` (1,657 lines)
- `addons/maintenance/i18n/ca.po` (1,696 lines)
- `addons/maintenance/i18n/cs.po` (1,688 lines)
- `addons/maintenance/i18n/da.po` (1,682 lines)
- `addons/maintenance/i18n/de.po` (1,699 lines)
- `addons/maintenance/i18n/el.po` (1,701 lines)
- `addons/maintenance/i18n/es.po` (1,695 lines)
- `addons/maintenance/i18n/es_419.po` (1,688 lines)
- `addons/maintenance/i18n/es_CL.po` (105 lines)
- `addons/maintenance/i18n/et.po` (1,693 lines)
- `addons/maintenance/i18n/eu.po` (1,638 lines)
- `addons/maintenance/i18n/fa.po` (1,683 lines)
- `addons/maintenance/i18n/fi.po` (1,711 lines)
- `addons/maintenance/i18n/fo.po` (1,638 lines)
- `addons/maintenance/i18n/fr.po` (1,693 lines)
- `addons/maintenance/i18n/fr_BE.po` (154 lines)
- `addons/maintenance/i18n/fr_CA.po` (100 lines)
- `addons/maintenance/i18n/gl.po` (1,638 lines)
- `addons/maintenance/i18n/gu.po` (1,643 lines)
- `addons/maintenance/i18n/he.po` (1,684 lines)
- `addons/maintenance/i18n/hi.po` (1,646 lines)
- `addons/maintenance/i18n/hr.po` (1,690 lines)
- `addons/maintenance/i18n/hu.po` (1,679 lines)
- `addons/maintenance/i18n/id.po` (1,690 lines)
- `addons/maintenance/i18n/is.po` (1,655 lines)
- `addons/maintenance/i18n/it.po` (1,693 lines)
- `addons/maintenance/i18n/ja.po` (1,684 lines)
- `addons/maintenance/i18n/ka.po` (1,638 lines)
- `addons/maintenance/i18n/kab.po` (1,647 lines)
- `addons/maintenance/i18n/kk.po` (1,637 lines)
- `addons/maintenance/i18n/km.po` (1,643 lines)
- `addons/maintenance/i18n/ko.po` (1,680 lines)
- `addons/maintenance/i18n/ku.po` (1,645 lines)
- `addons/maintenance/i18n/lb.po` (1,640 lines)
- `addons/maintenance/i18n/lo.po` (1,674 lines)
- `addons/maintenance/i18n/lt.po` (1,692 lines)
- `addons/maintenance/i18n/lv.po` (1,678 lines)
- `addons/maintenance/i18n/maintenance.pot` (1,640 lines)
- `addons/maintenance/i18n/mk.po` (1,638 lines)
- `addons/maintenance/i18n/mn.po` (1,685 lines)
- `addons/maintenance/i18n/my.po` (1,647 lines)
- `addons/maintenance/i18n/nb.po` (1,662 lines)
- `addons/maintenance/i18n/nl.po` (1,691 lines)
- `addons/maintenance/i18n/pl.po` (1,708 lines)
- `addons/maintenance/i18n/pt.po` (1,692 lines)
- `addons/maintenance/i18n/pt_BR.po` (1,689 lines)
- `addons/maintenance/i18n/ro.po` (1,682 lines)
- `addons/maintenance/i18n/ru.po` (1,689 lines)
- `addons/maintenance/i18n/sk.po` (1,682 lines)
- `addons/maintenance/i18n/sl.po` (1,689 lines)
- `addons/maintenance/i18n/sq.po` (1,638 lines)
- `addons/maintenance/i18n/sr@latin.po` (1,676 lines)
- `addons/maintenance/i18n/sv.po` (1,697 lines)
- `addons/maintenance/i18n/th.po` (1,672 lines)
- `addons/maintenance/i18n/tr.po` (1,708 lines)
- `addons/maintenance/i18n/uk.po` (1,680 lines)
- `addons/maintenance/i18n/uz.po` (1,938 lines)
- `addons/maintenance/i18n/vi.po` (1,688 lines)
- `addons/maintenance/i18n/zh_CN.po` (1,672 lines)
- `addons/maintenance/i18n/zh_TW.po` (1,667 lines)
- `addons/maintenance/models/__init__.py` (4 lines)
- `addons/maintenance/models/maintenance.py` (553 lines)
- `addons/maintenance/models/res_config_settings.py` (10 lines)
- `addons/maintenance/security/ir.access.csv` (16 lines)
- `addons/maintenance/security/maintenance.xml` (17 lines)
- `addons/maintenance/static/description/icon.png` (37 lines)
- `addons/maintenance/static/description/icon.svg` (1 lines)
- `addons/maintenance/static/description/icon_hi.png` (111 lines)
- `addons/maintenance/static/src/scss/maintenance_team_dashboard.scss` (3 lines)
- `addons/maintenance/static/src/views/calendar_with_recurrence/calendar_with_recurrence_common_renderer.js` (24 lines)
- `addons/maintenance/static/src/views/calendar_with_recurrence/calendar_with_recurrence_model.js` (81 lines)
- `addons/maintenance/static/src/views/calendar_with_recurrence/calendar_with_recurrence_renderer.js` (13 lines)
- `addons/maintenance/static/src/views/calendar_with_recurrence/calendar_with_recurrence_view.js` (12 lines)
- `addons/maintenance/static/src/views/calendar_with_recurrence/calendar_with_recurrence_year_popover.js` (8 lines)
- `addons/maintenance/static/src/views/calendar_with_recurrence/calendar_with_recurrence_year_renderer.js` (9 lines)
- `addons/maintenance/static/src/views/fields/radio/ordered_radio_field.js` (22 lines)
- `addons/maintenance/static/src/widgets/maintenance_request_state_selection.js` (86 lines)
- `addons/maintenance/static/src/widgets/maintenance_request_state_selection.scss` (11 lines)
- `addons/maintenance/static/src/widgets/maintenance_state_selection.xml` (33 lines)
- `addons/maintenance/static/tests/tours/tour_calendar_with_recurrence.js` (87 lines)
- `addons/maintenance/tests/__init__.py` (5 lines)
- `addons/maintenance/tests/test_calendar_with_recurrence.py` (70 lines)
- `addons/maintenance/tests/test_maintenance.py` (223 lines)
- `addons/maintenance/tests/test_maintenance_multicompany.py` (176 lines)
- `addons/maintenance/views/mail_activity_views.xml` (17 lines)
- `addons/maintenance/views/maintenance_views.xml` (1,046 lines)
- `addons/maintenance/views/res_config_settings_views.xml` (34 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
