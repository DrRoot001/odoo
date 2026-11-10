# Module: web_tour

- **Module ID:** MOD-594
- **Path:** `addons/web_tour`
- **Manifest:** `addons/web_tour/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Odoo Web tours.
========================



Declared dependencies: `web`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 28 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
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
    "views/tour_views.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      [
        "include",
        "web_tour.assets"
      ],
      "web_tour/static/src/tour_pointer/tour_pointer.scss",
      "web_tour/static/src/views/**/*",
      "web_tour/static/src/widgets/**/*"
    ],
    "web.assets_frontend": [
      [
        "include",
        "web_tour.assets"
      ],
      "web_tour/static/src/tour_pointer/tour_pointer.scss"
    ],
    "web.assets_unit_tests": [
      [
        "include",
        "web_tour.recorder"
      ],
      [
        "include",
        "web_tour.automatic"
      ],
      [
        "include",
        "web_tour.interactive"
      ],
      "web_tour/static/tests/tour_models.js",
      "web_tour/static/tests/*.test.js"
    ],
    "web.assets_tests": [
      "web_tour/static/src/tour_helpers/tour_helpers.js",
      [
        "include",
        "web_tour.automatic"
      ]
    ],
    "web_tour.common": [
      "web/static/lib/hoot-dom/**/*",
      "web_tour/static/src/tour_step.js"
    ],
    "web_tour.helpers": [
      [
        "include",
        "web_tour.common"
      ],
      "web_tour/static/src/tour_helpers/**/*"
    ],
    "web_tour.interactive": [
      [
        "include",
        "web_tour.helpers"
      ],
      "web_tour/static/src/tour_interactive/**/*"
    ],
    "web_tour.automatic": [
      [
        "include",
        "web_tour.helpers"
      ],
      "web_tour/static/src/tour_automatic/tour_automatic.js",
      "web_tour/static/src/tour_automatic/tour_step_automatic.js"
    ],
    "web_tour.recorder": [
      [
        "include",
        "web_tour.common"
      ],
      "web_tour/static/src/tour_recorder/**/*",
      "web_tour/static/src/views/**/*",
      "web_tour/static/src/widgets/**/*"
    ],
    "web_tour.assets": [
      "web_tour/static/src/tour_pointer/tour_pointer.js",
      "web_tour/static/src/tour_pointer/tour_pointer.xml",
      "web_tour/static/src/tour_helpers/tour_helpers.js",
      "web_tour/static/src/tour_state.js",
      "web_tour/static/src/tour_plugin.js",
      "web_tour/static/src/tour_recorder/tour_recorder_state.js",
      "web_tour/static/src/tour_recorder/tour_recorder_plugin.js",
      "web_tour/static/src/tour_recorder/tour_recorder_command_provider.js",
      "web_tour/static/src/tour_utils.js",
      "web_tour/static/src/tour_scenarios.js",
      "web_tour/static/src/widgets/onboarding_item.js",
      "web_tour/static/src/widgets/onboarding_item.xml"
    ]
  }
}
```

### Representative source files

- `addons/web_tour/__init__.py` (1 lines)
- `addons/web_tour/__manifest__.py` (79 lines)
- `addons/web_tour/i18n/ar.po` (445 lines)
- `addons/web_tour/i18n/az.po` (441 lines)
- `addons/web_tour/i18n/bg.po` (438 lines)
- `addons/web_tour/i18n/bs.po` (442 lines)
- `addons/web_tour/i18n/ca.po` (450 lines)
- `addons/web_tour/i18n/cs.po` (446 lines)
- `addons/web_tour/i18n/da.po` (452 lines)
- `addons/web_tour/i18n/de.po` (452 lines)
- `addons/web_tour/i18n/el.po` (443 lines)
- `addons/web_tour/i18n/es.po` (452 lines)
- `addons/web_tour/i18n/es_419.po` (444 lines)
- `addons/web_tour/i18n/et.po` (448 lines)
- `addons/web_tour/i18n/fa.po` (445 lines)
- `addons/web_tour/i18n/fi.po` (454 lines)
- `addons/web_tour/i18n/fr.po` (451 lines)
- `addons/web_tour/i18n/gu.po` (427 lines)
- `addons/web_tour/i18n/he.po` (447 lines)
- `addons/web_tour/i18n/hi.po` (438 lines)
- `addons/web_tour/i18n/hr.po` (446 lines)
- `addons/web_tour/i18n/hu.po` (445 lines)
- `addons/web_tour/i18n/id.po` (450 lines)
- `addons/web_tour/i18n/is.po` (423 lines)
- `addons/web_tour/i18n/it.po` (449 lines)
- `addons/web_tour/i18n/ja.po` (447 lines)
- `addons/web_tour/i18n/kab.po` (438 lines)
- `addons/web_tour/i18n/km.po` (426 lines)
- `addons/web_tour/i18n/ko.po` (443 lines)
- `addons/web_tour/i18n/ku.po` (438 lines)
- `addons/web_tour/i18n/lo.po` (446 lines)
- `addons/web_tour/i18n/lt.po` (449 lines)
- `addons/web_tour/i18n/lv.po` (444 lines)
- `addons/web_tour/i18n/mn.po` (444 lines)
- `addons/web_tour/i18n/my.po` (439 lines)
- `addons/web_tour/i18n/nb.po` (443 lines)
- `addons/web_tour/i18n/nl.po` (448 lines)
- `addons/web_tour/i18n/pl.po` (462 lines)
- `addons/web_tour/i18n/pt.po` (448 lines)
- `addons/web_tour/i18n/pt_BR.po` (454 lines)
- `addons/web_tour/i18n/ro.po` (444 lines)
- `addons/web_tour/i18n/ru.po` (443 lines)
- `addons/web_tour/i18n/sk.po` (443 lines)
- `addons/web_tour/i18n/sl.po` (446 lines)
- `addons/web_tour/i18n/sr@latin.po` (442 lines)
- `addons/web_tour/i18n/sv.po` (449 lines)
- `addons/web_tour/i18n/th.po` (445 lines)
- `addons/web_tour/i18n/tr.po` (451 lines)
- `addons/web_tour/i18n/uk.po` (444 lines)
- `addons/web_tour/i18n/uz.po` (493 lines)
- `addons/web_tour/i18n/vi.po` (444 lines)
- `addons/web_tour/i18n/web_tour.pot` (434 lines)
- `addons/web_tour/i18n/zh_CN.po` (457 lines)
- `addons/web_tour/i18n/zh_TW.po` (444 lines)
- `addons/web_tour/models/__init__.py` (3 lines)
- `addons/web_tour/models/ir_http.py` (11 lines)
- `addons/web_tour/models/res_users.py` (18 lines)
- `addons/web_tour/models/tour.py` (111 lines)
- `addons/web_tour/security/ir.access.csv` (5 lines)
- `addons/web_tour/static/src/@types/registries.d.ts` (17 lines)
- `addons/web_tour/static/src/tour_automatic/tour_automatic.js` (167 lines)
- `addons/web_tour/static/src/tour_automatic/tour_step_automatic.js` (76 lines)
- `addons/web_tour/static/src/tour_helpers/tour_helpers.js` (15 lines)
- `addons/web_tour/static/src/tour_helpers/tour_helpers_clipboard.js` (30 lines)
- `addons/web_tour/static/src/tour_helpers/tour_helpers_hoot.js` (440 lines)
- `addons/web_tour/static/src/tour_interactive/tour_interactive.js` (452 lines)
- `addons/web_tour/static/src/tour_interactive/tour_interactive_observer.js` (76 lines)
- `addons/web_tour/static/src/tour_interactive/tour_step_interactive.js` (151 lines)
- `addons/web_tour/static/src/tour_plugin.js` (325 lines)
- `addons/web_tour/static/src/tour_pointer/tour_pointer.js` (371 lines)
- `addons/web_tour/static/src/tour_pointer/tour_pointer.scss` (117 lines)
- `addons/web_tour/static/src/tour_pointer/tour_pointer.xml` (47 lines)
- `addons/web_tour/static/src/tour_recorder/tour_recorder.js` (407 lines)
- `addons/web_tour/static/src/tour_recorder/tour_recorder.xml` (82 lines)
- `addons/web_tour/static/src/tour_recorder/tour_recorder_command_provider.js` (20 lines)
- `addons/web_tour/static/src/tour_recorder/tour_recorder_plugin.js` (63 lines)
- `addons/web_tour/static/src/tour_recorder/tour_recorder_state.js` (33 lines)
- `addons/web_tour/static/src/tour_scenarios.js` (128 lines)
- `addons/web_tour/static/src/tour_state.js` (44 lines)
- `addons/web_tour/static/src/tour_step.js` (293 lines)
- `addons/web_tour/static/src/tour_utils.js` (174 lines)
- `addons/web_tour/static/src/views/tour_controller.xml` (11 lines)
- `addons/web_tour/static/src/views/tour_list.js` (7 lines)
- `addons/web_tour/static/src/widgets/onboarding_item.js` (12 lines)
- `addons/web_tour/static/src/widgets/onboarding_item.xml` (15 lines)
- `addons/web_tour/static/src/widgets/tour_start.js` (49 lines)
- `addons/web_tour/static/src/widgets/tour_start.xml` (15 lines)
- `addons/web_tour/static/tests/tour_automatic.test.js` (787 lines)
- `addons/web_tour/static/tests/tour_interactive.test.js` (986 lines)
- `addons/web_tour/static/tests/tour_list.test.js` (38 lines)
- `addons/web_tour/static/tests/tour_models.js` (29 lines)
- `addons/web_tour/static/tests/tour_pointer.test.js` (612 lines)
- `addons/web_tour/static/tests/tour_recorder.test.js` (467 lines)
- `addons/web_tour/tests/__init__.py` (2 lines)
- `addons/web_tour/tests/test_onboarding_tours.py` (51 lines)
- `addons/web_tour/tests/test_tours.py` (179 lines)
- `addons/web_tour/views/tour_views.xml` (89 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
