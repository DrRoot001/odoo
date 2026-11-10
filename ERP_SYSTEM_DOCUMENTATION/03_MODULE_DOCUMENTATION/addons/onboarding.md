# Module: onboarding

- **Module ID:** MOD-389
- **Path:** `addons/onboarding`
- **Manifest:** `addons/onboarding/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This module allows to manage onboardings and their progress
================================================================================
    

Declared dependencies: `web`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "web"
  ],
  "data": [
    "views/onboarding_templates.xml",
    "views/onboarding_views.xml",
    "views/onboarding_menus.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "onboarding/static/src/**/*",
      [
        "remove",
        "onboarding/static/src/scss/onboarding.variables.dark.scss"
      ]
    ],
    "web.dark_mode_variables": [
      [
        "before",
        "onboarding/static/src/scss/onboarding.variables.scss",
        "onboarding/static/src/scss/onboarding.variables.dark.scss"
      ]
    ],
    "web._assets_primary_variables": [
      "onboarding/static/src/scss/onboarding.variables.scss"
    ]
  }
}
```

### Representative source files

- `addons/onboarding/__init__.py` (4 lines)
- `addons/onboarding/__manifest__.py` (33 lines)
- `addons/onboarding/i18n/ar.po` (440 lines)
- `addons/onboarding/i18n/az.po` (434 lines)
- `addons/onboarding/i18n/bg.po` (434 lines)
- `addons/onboarding/i18n/bs.po` (436 lines)
- `addons/onboarding/i18n/ca.po` (438 lines)
- `addons/onboarding/i18n/cs.po` (435 lines)
- `addons/onboarding/i18n/da.po` (436 lines)
- `addons/onboarding/i18n/de.po` (449 lines)
- `addons/onboarding/i18n/el.po` (435 lines)
- `addons/onboarding/i18n/es.po` (448 lines)
- `addons/onboarding/i18n/es_419.po` (447 lines)
- `addons/onboarding/i18n/et.po` (434 lines)
- `addons/onboarding/i18n/fa.po` (434 lines)
- `addons/onboarding/i18n/fi.po` (448 lines)
- `addons/onboarding/i18n/fr.po` (450 lines)
- `addons/onboarding/i18n/he.po` (435 lines)
- `addons/onboarding/i18n/hi.po` (434 lines)
- `addons/onboarding/i18n/hr.po` (435 lines)
- `addons/onboarding/i18n/hu.po` (435 lines)
- `addons/onboarding/i18n/id.po` (442 lines)
- `addons/onboarding/i18n/it.po` (448 lines)
- `addons/onboarding/i18n/ja.po` (440 lines)
- `addons/onboarding/i18n/kab.po` (435 lines)
- `addons/onboarding/i18n/ko.po` (440 lines)
- `addons/onboarding/i18n/ku.po` (434 lines)
- `addons/onboarding/i18n/lo.po` (443 lines)
- `addons/onboarding/i18n/lt.po` (436 lines)
- `addons/onboarding/i18n/lv.po` (435 lines)
- `addons/onboarding/i18n/mn.po` (434 lines)
- `addons/onboarding/i18n/my.po` (435 lines)
- `addons/onboarding/i18n/nb.po` (435 lines)
- `addons/onboarding/i18n/nl.po` (447 lines)
- `addons/onboarding/i18n/onboarding.pot` (431 lines)
- `addons/onboarding/i18n/pl.po` (438 lines)
- `addons/onboarding/i18n/pt.po` (443 lines)
- `addons/onboarding/i18n/pt_BR.po` (448 lines)
- `addons/onboarding/i18n/ro.po` (443 lines)
- `addons/onboarding/i18n/ru.po` (448 lines)
- `addons/onboarding/i18n/sk.po` (434 lines)
- `addons/onboarding/i18n/sl.po` (436 lines)
- `addons/onboarding/i18n/sr@latin.po` (436 lines)
- `addons/onboarding/i18n/sv.po` (443 lines)
- `addons/onboarding/i18n/th.po` (439 lines)
- `addons/onboarding/i18n/tr.po` (441 lines)
- `addons/onboarding/i18n/uk.po` (435 lines)
- `addons/onboarding/i18n/uz.po` (516 lines)
- `addons/onboarding/i18n/vi.po` (440 lines)
- `addons/onboarding/i18n/zh_CN.po` (440 lines)
- `addons/onboarding/i18n/zh_TW.po` (441 lines)
- `addons/onboarding/models/__init__.py` (7 lines)
- `addons/onboarding/models/onboarding_onboarding.py` (135 lines)
- `addons/onboarding/models/onboarding_onboarding_step.py` (133 lines)
- `addons/onboarding/models/onboarding_progress.py` (78 lines)
- `addons/onboarding/models/onboarding_progress_step.py` (31 lines)
- `addons/onboarding/security/ir.access.csv` (5 lines)
- `addons/onboarding/static/src/img/onboarding_bg.png` (698 lines)
- `addons/onboarding/static/src/scss/onboarding.scss` (157 lines)
- `addons/onboarding/static/src/scss/onboarding.variables.dark.scss` (6 lines)
- `addons/onboarding/static/src/scss/onboarding.variables.scss` (6 lines)
- `addons/onboarding/static/src/views/form/onboarding_step_form_controller.js` (53 lines)
- `addons/onboarding/tests/__init__.py` (6 lines)
- `addons/onboarding/tests/case.py` (40 lines)
- `addons/onboarding/tests/common.py` (59 lines)
- `addons/onboarding/tests/test_onboarding.py` (241 lines)
- `addons/onboarding/tests/test_onboarding_concurrency.py` (84 lines)
- `addons/onboarding/views/onboarding_menus.xml` (14 lines)
- `addons/onboarding/views/onboarding_templates.xml` (103 lines)
- `addons/onboarding/views/onboarding_views.xml` (109 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
