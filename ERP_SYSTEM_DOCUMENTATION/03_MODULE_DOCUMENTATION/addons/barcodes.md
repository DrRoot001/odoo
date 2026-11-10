# Module: barcodes

- **Module ID:** MOD-032
- **Path:** `addons/barcodes`
- **Manifest:** `addons/barcodes/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Scan and Parse Barcodes

No manifest description declared.

Declared dependencies: `web`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 7 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 11 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
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
    "data/barcodes_data.xml",
    "views/barcodes_view.xml",
    "views/res_partner_views.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "barcodes/static/src/**/*"
    ],
    "web.assets_unit_tests": [
      "barcodes/static/tests/*.test.js"
    ]
  }
}
```

### Representative source files

- `addons/barcodes/__init__.py` (14 lines)
- `addons/barcodes/__manifest__.py` (24 lines)
- `addons/barcodes/data/barcodes_data.xml` (15 lines)
- `addons/barcodes/i18n/af.po` (368 lines)
- `addons/barcodes/i18n/am.po` (364 lines)
- `addons/barcodes/i18n/ar.po` (422 lines)
- `addons/barcodes/i18n/az.po` (393 lines)
- `addons/barcodes/i18n/barcodes.pot` (376 lines)
- `addons/barcodes/i18n/bg.po` (413 lines)
- `addons/barcodes/i18n/bs.po` (393 lines)
- `addons/barcodes/i18n/ca.po` (443 lines)
- `addons/barcodes/i18n/cs.po` (427 lines)
- `addons/barcodes/i18n/da.po` (427 lines)
- `addons/barcodes/i18n/de.po` (439 lines)
- `addons/barcodes/i18n/el.po` (424 lines)
- `addons/barcodes/i18n/es.po` (441 lines)
- `addons/barcodes/i18n/es_419.po` (437 lines)
- `addons/barcodes/i18n/es_CL.po` (65 lines)
- `addons/barcodes/i18n/et.po` (434 lines)
- `addons/barcodes/i18n/eu.po` (367 lines)
- `addons/barcodes/i18n/fa.po` (423 lines)
- `addons/barcodes/i18n/fi.po` (436 lines)
- `addons/barcodes/i18n/fo.po` (367 lines)
- `addons/barcodes/i18n/fr.po` (442 lines)
- `addons/barcodes/i18n/fr_BE.po` (61 lines)
- `addons/barcodes/i18n/fr_CA.po` (65 lines)
- `addons/barcodes/i18n/gl.po` (367 lines)
- `addons/barcodes/i18n/gu.po` (368 lines)
- `addons/barcodes/i18n/he.po` (422 lines)
- `addons/barcodes/i18n/hi.po` (389 lines)
- `addons/barcodes/i18n/hr.po` (420 lines)
- `addons/barcodes/i18n/hu.po` (412 lines)
- `addons/barcodes/i18n/id.po` (433 lines)
- `addons/barcodes/i18n/is.po` (364 lines)
- `addons/barcodes/i18n/it.po` (440 lines)
- `addons/barcodes/i18n/ja.po` (430 lines)
- `addons/barcodes/i18n/ka.po` (367 lines)
- `addons/barcodes/i18n/kab.po` (390 lines)
- `addons/barcodes/i18n/km.po` (368 lines)
- `addons/barcodes/i18n/ko.po` (424 lines)
- `addons/barcodes/i18n/ku.po` (392 lines)
- `addons/barcodes/i18n/lo.po` (414 lines)
- `addons/barcodes/i18n/lt.po` (416 lines)
- `addons/barcodes/i18n/lv.po` (394 lines)
- `addons/barcodes/i18n/mk.po` (367 lines)
- `addons/barcodes/i18n/mn.po` (430 lines)
- `addons/barcodes/i18n/my.po` (389 lines)
- `addons/barcodes/i18n/nb.po` (394 lines)
- `addons/barcodes/i18n/nl.po` (434 lines)
- `addons/barcodes/i18n/pl.po` (442 lines)
- `addons/barcodes/i18n/pt.po` (436 lines)
- `addons/barcodes/i18n/pt_BR.po` (439 lines)
- `addons/barcodes/i18n/ro.po` (435 lines)
- `addons/barcodes/i18n/ru.po` (431 lines)
- `addons/barcodes/i18n/sk.po` (409 lines)
- `addons/barcodes/i18n/sl.po` (436 lines)
- `addons/barcodes/i18n/sq.po` (367 lines)
- `addons/barcodes/i18n/sr@latin.po` (393 lines)
- `addons/barcodes/i18n/sv.po` (438 lines)
- `addons/barcodes/i18n/ta.po` (368 lines)
- `addons/barcodes/i18n/th.po` (413 lines)
- `addons/barcodes/i18n/tr.po` (439 lines)
- `addons/barcodes/i18n/uk.po` (428 lines)
- `addons/barcodes/i18n/uz.po` (480 lines)
- `addons/barcodes/i18n/vi.po` (429 lines)
- `addons/barcodes/i18n/zh_CN.po` (414 lines)
- `addons/barcodes/i18n/zh_TW.po` (414 lines)
- `addons/barcodes/models/__init__.py` (5 lines)
- `addons/barcodes/models/barcode_nomenclature.py` (215 lines)
- `addons/barcodes/models/barcode_rule.py` (47 lines)
- `addons/barcodes/models/ir_http.py` (14 lines)
- `addons/barcodes/models/res_company.py` (16 lines)
- `addons/barcodes/security/ir.access.csv` (5 lines)
- `addons/barcodes/static/img/barcode.png` (7 lines)
- `addons/barcodes/static/src/audio/error.mp3` (329 lines)
- `addons/barcodes/static/src/audio/error.ogg` (104 lines)
- `addons/barcodes/static/src/barcode_handlers.js` (110 lines)
- `addons/barcodes/static/src/barcode_plugin.js` (162 lines)
- `addons/barcodes/static/src/components/barcode_input.js` (38 lines)
- `addons/barcodes/static/src/components/barcode_input.scss` (11 lines)
- `addons/barcodes/static/src/components/barcode_input.xml` (23 lines)
- `addons/barcodes/static/src/components/barcode_scanner.js` (44 lines)
- `addons/barcodes/static/src/components/barcode_scanner.scss` (66 lines)
- `addons/barcodes/static/src/components/barcode_scanner.xml` (15 lines)
- `addons/barcodes/static/src/components/barcode_view.js` (75 lines)
- `addons/barcodes/static/src/components/barcode_view.scss` (3 lines)
- `addons/barcodes/static/src/components/barcode_view.xml` (44 lines)
- `addons/barcodes/static/src/components/manual_barcode.js` (12 lines)
- `addons/barcodes/static/src/components/manual_barcode.xml` (13 lines)
- `addons/barcodes/static/src/js/barcode_parser.js` (306 lines)
- `addons/barcodes/static/tests/barcode.test.js` (190 lines)
- `addons/barcodes/static/tests/barcode_mobile.test.js` (75 lines)
- `addons/barcodes/static/tests/barcode_parser.test.js` (38 lines)
- `addons/barcodes/static/tests/barcode_scan.test.js` (34 lines)
- `addons/barcodes/tests/__init__.py` (1 lines)
- `addons/barcodes/tests/test_barcode_nomenclature.py` (291 lines)
- `addons/barcodes/views/barcodes_view.xml` (82 lines)
- `addons/barcodes/views/res_partner_views.xml` (16 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
