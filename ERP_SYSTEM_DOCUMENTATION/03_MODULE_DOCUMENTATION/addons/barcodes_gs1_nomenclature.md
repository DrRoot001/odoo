# Module: barcodes_gs1_nomenclature

- **Module ID:** MOD-033
- **Path:** `addons/barcodes_gs1_nomenclature`
- **Manifest:** `addons/barcodes_gs1_nomenclature/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Parse barcodes according to the GS1-128 specifications

No manifest description declared.

Declared dependencies: `barcodes`, `uom`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 6 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "barcodes",
    "uom"
  ],
  "data": [
    "data/barcodes_gs1_rules.xml",
    "views/barcodes_view.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "barcodes_gs1_nomenclature/static/src/js/barcode_parser.js",
      "barcodes_gs1_nomenclature/static/src/js/barcode_plugin.js",
      "barcodes_gs1_nomenclature/static/src/js/epc_model.js",
      "barcodes_gs1_nomenclature/static/src/js/epc_utils.js"
    ],
    "web.assets_unit_tests": [
      "barcodes_gs1_nomenclature/static/src/js/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/barcodes_gs1_nomenclature/__init__.py` (1 lines)
- `addons/barcodes_gs1_nomenclature/__manifest__.py` (25 lines)
- `addons/barcodes_gs1_nomenclature/data/barcodes_gs1_rules.xml` (338 lines)
- `addons/barcodes_gs1_nomenclature/i18n/ar.po` (291 lines)
- `addons/barcodes_gs1_nomenclature/i18n/az.po` (269 lines)
- `addons/barcodes_gs1_nomenclature/i18n/barcodes_gs1_nomenclature.pot` (261 lines)
- `addons/barcodes_gs1_nomenclature/i18n/bg.po` (269 lines)
- `addons/barcodes_gs1_nomenclature/i18n/bs.po` (269 lines)
- `addons/barcodes_gs1_nomenclature/i18n/ca.po` (288 lines)
- `addons/barcodes_gs1_nomenclature/i18n/cs.po` (270 lines)
- `addons/barcodes_gs1_nomenclature/i18n/da.po` (294 lines)
- `addons/barcodes_gs1_nomenclature/i18n/de.po` (296 lines)
- `addons/barcodes_gs1_nomenclature/i18n/el.po` (271 lines)
- `addons/barcodes_gs1_nomenclature/i18n/es.po` (303 lines)
- `addons/barcodes_gs1_nomenclature/i18n/es_419.po` (301 lines)
- `addons/barcodes_gs1_nomenclature/i18n/et.po` (290 lines)
- `addons/barcodes_gs1_nomenclature/i18n/fa.po` (283 lines)
- `addons/barcodes_gs1_nomenclature/i18n/fi.po` (293 lines)
- `addons/barcodes_gs1_nomenclature/i18n/fr.po` (294 lines)
- `addons/barcodes_gs1_nomenclature/i18n/he.po` (268 lines)
- `addons/barcodes_gs1_nomenclature/i18n/hi.po` (267 lines)
- `addons/barcodes_gs1_nomenclature/i18n/hr.po` (269 lines)
- `addons/barcodes_gs1_nomenclature/i18n/hu.po` (269 lines)
- `addons/barcodes_gs1_nomenclature/i18n/id.po` (294 lines)
- `addons/barcodes_gs1_nomenclature/i18n/it.po` (298 lines)
- `addons/barcodes_gs1_nomenclature/i18n/ja.po` (290 lines)
- `addons/barcodes_gs1_nomenclature/i18n/kab.po` (268 lines)
- `addons/barcodes_gs1_nomenclature/i18n/ko.po` (288 lines)
- `addons/barcodes_gs1_nomenclature/i18n/ku.po` (269 lines)
- `addons/barcodes_gs1_nomenclature/i18n/lo.po` (287 lines)
- `addons/barcodes_gs1_nomenclature/i18n/lt.po` (271 lines)
- `addons/barcodes_gs1_nomenclature/i18n/lv.po` (269 lines)
- `addons/barcodes_gs1_nomenclature/i18n/mn.po` (269 lines)
- `addons/barcodes_gs1_nomenclature/i18n/my.po` (267 lines)
- `addons/barcodes_gs1_nomenclature/i18n/nb.po` (267 lines)
- `addons/barcodes_gs1_nomenclature/i18n/nl.po` (293 lines)
- `addons/barcodes_gs1_nomenclature/i18n/pl.po` (297 lines)
- `addons/barcodes_gs1_nomenclature/i18n/pt.po` (294 lines)
- `addons/barcodes_gs1_nomenclature/i18n/pt_BR.po` (296 lines)
- `addons/barcodes_gs1_nomenclature/i18n/ro.po` (286 lines)
- `addons/barcodes_gs1_nomenclature/i18n/ru.po` (301 lines)
- `addons/barcodes_gs1_nomenclature/i18n/sk.po` (270 lines)
- `addons/barcodes_gs1_nomenclature/i18n/sl.po` (289 lines)
- `addons/barcodes_gs1_nomenclature/i18n/sr@latin.po` (268 lines)
- `addons/barcodes_gs1_nomenclature/i18n/sv.po` (290 lines)
- `addons/barcodes_gs1_nomenclature/i18n/th.po` (284 lines)
- `addons/barcodes_gs1_nomenclature/i18n/tr.po` (291 lines)
- `addons/barcodes_gs1_nomenclature/i18n/uk.po` (285 lines)
- `addons/barcodes_gs1_nomenclature/i18n/uz.po` (336 lines)
- `addons/barcodes_gs1_nomenclature/i18n/vi.po` (296 lines)
- `addons/barcodes_gs1_nomenclature/i18n/zh_CN.po` (279 lines)
- `addons/barcodes_gs1_nomenclature/i18n/zh_TW.po` (282 lines)
- `addons/barcodes_gs1_nomenclature/models/__init__.py` (3 lines)
- `addons/barcodes_gs1_nomenclature/models/barcode_nomenclature.py` (205 lines)
- `addons/barcodes_gs1_nomenclature/models/barcode_rule.py` (69 lines)
- `addons/barcodes_gs1_nomenclature/models/ir_http.py` (16 lines)
- `addons/barcodes_gs1_nomenclature/static/src/js/barcode_parser.js` (179 lines)
- `addons/barcodes_gs1_nomenclature/static/src/js/barcode_plugin.js` (16 lines)
- `addons/barcodes_gs1_nomenclature/static/src/js/epc_model.js` (279 lines)
- `addons/barcodes_gs1_nomenclature/static/src/js/epc_utils.js` (285 lines)
- `addons/barcodes_gs1_nomenclature/static/src/js/tests/barcode_parser.test.js` (255 lines)
- `addons/barcodes_gs1_nomenclature/static/src/js/tests/epc_utils.test.js` (64 lines)
- `addons/barcodes_gs1_nomenclature/tests/__init__.py` (1 lines)
- `addons/barcodes_gs1_nomenclature/tests/test_barcodes_gs1_nomenclature.py` (145 lines)
- `addons/barcodes_gs1_nomenclature/views/barcodes_view.xml` (61 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
