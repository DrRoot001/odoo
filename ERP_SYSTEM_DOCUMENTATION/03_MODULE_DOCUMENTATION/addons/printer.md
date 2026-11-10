# Module: printer

- **Module ID:** MOD-468
- **Path:** `addons/printer`
- **Manifest:** `addons/printer/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Base module to manage external printers (e.g. ePOS, ZPL)

No manifest description declared.

Declared dependencies: `base`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 10 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base"
  ],
  "data": [
    "views/ir_actions_report.xml",
    "views/printer_views.xml",
    "wizard/select_printers_wizard.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "demo/printers.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "printer/static/src/**/*"
    ],
    "web.assets_unit_tests": [
      "printer/static/tests/unit/**/*"
    ],
    "printer.assets_tests": [
      "printer/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/printer/__init__.py` (2 lines)
- `addons/printer/__manifest__.py` (28 lines)
- `addons/printer/demo/printers.xml` (15 lines)
- `addons/printer/i18n/ar.po` (196 lines)
- `addons/printer/i18n/az.po` (195 lines)
- `addons/printer/i18n/bg.po` (195 lines)
- `addons/printer/i18n/bs.po` (196 lines)
- `addons/printer/i18n/ca.po` (195 lines)
- `addons/printer/i18n/cs.po` (196 lines)
- `addons/printer/i18n/da.po` (195 lines)
- `addons/printer/i18n/de.po` (200 lines)
- `addons/printer/i18n/el.po` (195 lines)
- `addons/printer/i18n/es.po` (196 lines)
- `addons/printer/i18n/es_419.po` (201 lines)
- `addons/printer/i18n/et.po` (195 lines)
- `addons/printer/i18n/fa.po` (195 lines)
- `addons/printer/i18n/fi.po` (196 lines)
- `addons/printer/i18n/fr.po` (201 lines)
- `addons/printer/i18n/he.po` (196 lines)
- `addons/printer/i18n/hi.po` (195 lines)
- `addons/printer/i18n/hr.po` (196 lines)
- `addons/printer/i18n/hu.po` (195 lines)
- `addons/printer/i18n/id.po` (199 lines)
- `addons/printer/i18n/it.po` (200 lines)
- `addons/printer/i18n/ja.po` (195 lines)
- `addons/printer/i18n/kab.po` (195 lines)
- `addons/printer/i18n/ko.po` (195 lines)
- `addons/printer/i18n/ku.po` (195 lines)
- `addons/printer/i18n/lo.po` (199 lines)
- `addons/printer/i18n/lt.po` (197 lines)
- `addons/printer/i18n/lv.po` (196 lines)
- `addons/printer/i18n/mn.po` (195 lines)
- `addons/printer/i18n/my.po` (196 lines)
- `addons/printer/i18n/nb.po` (195 lines)
- `addons/printer/i18n/nl.po` (201 lines)
- `addons/printer/i18n/pl.po` (196 lines)
- `addons/printer/i18n/printer.pot` (192 lines)
- `addons/printer/i18n/pt.po` (195 lines)
- `addons/printer/i18n/pt_BR.po` (216 lines)
- `addons/printer/i18n/ro.po` (196 lines)
- `addons/printer/i18n/ru.po` (196 lines)
- `addons/printer/i18n/sk.po` (195 lines)
- `addons/printer/i18n/sl.po` (196 lines)
- `addons/printer/i18n/sr@latin.po` (196 lines)
- `addons/printer/i18n/sv.po` (196 lines)
- `addons/printer/i18n/th.po` (198 lines)
- `addons/printer/i18n/tr.po` (195 lines)
- `addons/printer/i18n/uk.po` (196 lines)
- `addons/printer/i18n/uz.po` (195 lines)
- `addons/printer/i18n/vi.po` (195 lines)
- `addons/printer/i18n/zh_CN.po` (197 lines)
- `addons/printer/i18n/zh_TW.po` (196 lines)
- `addons/printer/models/__init__.py` (2 lines)
- `addons/printer/models/ir_actions_report.py` (140 lines)
- `addons/printer/models/printer.py` (26 lines)
- `addons/printer/security/ir.access.csv` (3 lines)
- `addons/printer/static/src/@types/registry.d.ts` (12 lines)
- `addons/printer/static/src/@types/services.d.ts` (7 lines)
- `addons/printer/static/src/client_actions/reset_cached_printers.js` (27 lines)
- `addons/printer/static/src/client_actions/reset_cached_printers.xml` (17 lines)
- `addons/printer/static/src/print_action_handler.js` (128 lines)
- `addons/printer/static/src/services/report_printers_cache.js` (87 lines)
- `addons/printer/static/src/wizard/select_printers_wizard.js` (60 lines)
- `addons/printer/static/tests/tours/test_print_label_epos_tour.js` (50 lines)
- `addons/printer/static/tests/tours/test_print_label_zebra_tour.js` (55 lines)
- `addons/printer/static/tests/tours/utils.js` (45 lines)
- `addons/printer/static/tests/unit/print_action_handler.test.js` (250 lines)
- `addons/printer/tests/__init__.py` (2 lines)
- `addons/printer/tests/test_get_print_jobs.py` (89 lines)
- `addons/printer/tests/test_thermal_printer_format.py` (82 lines)
- `addons/printer/views/ir_actions_report.xml` (15 lines)
- `addons/printer/views/printer_views.xml` (55 lines)
- `addons/printer/wizard/__init__.py` (1 lines)
- `addons/printer/wizard/select_printers_wizard.py` (20 lines)
- `addons/printer/wizard/select_printers_wizard.xml` (20 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
