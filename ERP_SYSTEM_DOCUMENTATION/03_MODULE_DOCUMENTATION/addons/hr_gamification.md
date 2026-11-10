# Module: hr_gamification

- **Module ID:** MOD-088
- **Path:** `addons/hr_gamification`
- **Manifest:** `addons/hr_gamification/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Use the HR resources for the gamification process.

The HR officer can now manage challenges and badges.
This allow the user to send badges to employees instead of simple users.
Badge received are displayed on the user profile.


Declared dependencies: `gamification`, `hr`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 11 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 6 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "gamification",
    "hr"
  ],
  "data": [
    "security/gamification_security.xml",
    "wizard/gamification_badge_user_wizard_views.xml",
    "views/gamification_views.xml",
    "views/hr_employee_views.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "hr_gamification/static/src/**/*"
    ],
    "web.assets_unit_tests": [
      "hr_gamification/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/hr_gamification/__init__.py` (9 lines)
- `addons/hr_gamification/__manifest__.py` (31 lines)
- `addons/hr_gamification/i18n/af.po` (287 lines)
- `addons/hr_gamification/i18n/am.po` (283 lines)
- `addons/hr_gamification/i18n/ar.po` (306 lines)
- `addons/hr_gamification/i18n/az.po` (290 lines)
- `addons/hr_gamification/i18n/bg.po` (300 lines)
- `addons/hr_gamification/i18n/bs.po` (289 lines)
- `addons/hr_gamification/i18n/ca.po` (304 lines)
- `addons/hr_gamification/i18n/cs.po` (301 lines)
- `addons/hr_gamification/i18n/da.po` (309 lines)
- `addons/hr_gamification/i18n/de.po` (318 lines)
- `addons/hr_gamification/i18n/el.po` (291 lines)
- `addons/hr_gamification/i18n/es.po` (315 lines)
- `addons/hr_gamification/i18n/es_419.po` (312 lines)
- `addons/hr_gamification/i18n/es_CL.po` (274 lines)
- `addons/hr_gamification/i18n/et.po` (303 lines)
- `addons/hr_gamification/i18n/eu.po` (286 lines)
- `addons/hr_gamification/i18n/fa.po` (300 lines)
- `addons/hr_gamification/i18n/fi.po` (319 lines)
- `addons/hr_gamification/i18n/fo.po` (286 lines)
- `addons/hr_gamification/i18n/fr.po` (312 lines)
- `addons/hr_gamification/i18n/fr_CA.po` (274 lines)
- `addons/hr_gamification/i18n/gl.po` (286 lines)
- `addons/hr_gamification/i18n/gu.po` (287 lines)
- `addons/hr_gamification/i18n/he.po` (296 lines)
- `addons/hr_gamification/i18n/hi.po` (286 lines)
- `addons/hr_gamification/i18n/hr.po` (300 lines)
- `addons/hr_gamification/i18n/hr_gamification.pot` (281 lines)
- `addons/hr_gamification/i18n/hu.po` (303 lines)
- `addons/hr_gamification/i18n/id.po` (307 lines)
- `addons/hr_gamification/i18n/is.po` (283 lines)
- `addons/hr_gamification/i18n/it.po` (317 lines)
- `addons/hr_gamification/i18n/ja.po` (305 lines)
- `addons/hr_gamification/i18n/ka.po` (286 lines)
- `addons/hr_gamification/i18n/kab.po` (288 lines)
- `addons/hr_gamification/i18n/km.po` (286 lines)
- `addons/hr_gamification/i18n/ko.po` (306 lines)
- `addons/hr_gamification/i18n/ku.po` (286 lines)
- `addons/hr_gamification/i18n/lo.po` (300 lines)
- `addons/hr_gamification/i18n/lt.po` (303 lines)
- `addons/hr_gamification/i18n/lv.po` (293 lines)
- `addons/hr_gamification/i18n/mk.po` (286 lines)
- `addons/hr_gamification/i18n/mn.po` (300 lines)
- `addons/hr_gamification/i18n/my.po` (286 lines)
- `addons/hr_gamification/i18n/nb.po` (294 lines)
- `addons/hr_gamification/i18n/nl.po` (310 lines)
- `addons/hr_gamification/i18n/pl.po` (315 lines)
- `addons/hr_gamification/i18n/pt.po` (302 lines)
- `addons/hr_gamification/i18n/pt_BR.po` (313 lines)
- `addons/hr_gamification/i18n/ro.po` (302 lines)
- `addons/hr_gamification/i18n/ru.po` (299 lines)
- `addons/hr_gamification/i18n/sk.po` (298 lines)
- `addons/hr_gamification/i18n/sl.po` (303 lines)
- `addons/hr_gamification/i18n/sq.po` (286 lines)
- `addons/hr_gamification/i18n/sr@latin.po` (291 lines)
- `addons/hr_gamification/i18n/sv.po` (305 lines)
- `addons/hr_gamification/i18n/th.po` (298 lines)
- `addons/hr_gamification/i18n/tr.po` (315 lines)
- `addons/hr_gamification/i18n/uk.po` (301 lines)
- `addons/hr_gamification/i18n/uz.po` (352 lines)
- `addons/hr_gamification/i18n/vi.po` (303 lines)
- `addons/hr_gamification/i18n/zh_CN.po` (308 lines)
- `addons/hr_gamification/i18n/zh_TW.po` (303 lines)
- `addons/hr_gamification/models/__init__.py` (7 lines)
- `addons/hr_gamification/models/gamification.py` (83 lines)
- `addons/hr_gamification/models/hr_employee.py` (38 lines)
- `addons/hr_gamification/models/hr_employee_public.py` (14 lines)
- `addons/hr_gamification/models/res_users.py` (11 lines)
- `addons/hr_gamification/security/gamification_security.xml` (7 lines)
- `addons/hr_gamification/security/ir.access.csv` (8 lines)
- `addons/hr_gamification/static/src/form_view.js` (33 lines)
- `addons/hr_gamification/static/src/messaging_menu_patch.js` (58 lines)
- `addons/hr_gamification/static/src/scss/hr_gamification.scss` (35 lines)
- `addons/hr_gamification/static/tests/hr_gamification_test_helpers.js` (14 lines)
- `addons/hr_gamification/static/tests/messaging_menu_patch.test.js` (57 lines)
- `addons/hr_gamification/static/tests/mock_server/mock_models/gamification_badge.js` (5 lines)
- `addons/hr_gamification/static/tests/mock_server/mock_models/gamification_badge_user.js` (5 lines)
- `addons/hr_gamification/tests/__init__.py` (1 lines)
- `addons/hr_gamification/tests/test_gamification_current_badge.py` (85 lines)
- `addons/hr_gamification/views/gamification_views.xml` (143 lines)
- `addons/hr_gamification/views/hr_employee_views.xml` (55 lines)
- `addons/hr_gamification/wizard/__init__.py` (4 lines)
- `addons/hr_gamification/wizard/gamification_badge_user_wizard.py` (32 lines)
- `addons/hr_gamification/wizard/gamification_badge_user_wizard_views.xml` (61 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
