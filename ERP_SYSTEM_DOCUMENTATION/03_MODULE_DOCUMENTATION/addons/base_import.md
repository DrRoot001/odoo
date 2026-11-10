# Module: base_import

- **Module ID:** MOD-037
- **Path:** `addons/base_import`
- **Manifest:** `addons/base_import/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


New extensible file import for Odoo
======================================

Re-implement Odoo's file import system:

* Server side, the previous system forces most of the logic into the
  client which duplicates the effort (between clients), makes the
  import system much harder to use without a client (direct RPC or
  other forms of automation) and makes knowledge about the
  import/export system much harder to gather as it is spread over
  3+ different projects.

* In a more extensible manner, so users and partners can build their
  own front-end to import from other file formats (e.g. OpenDocument
  files) which may be simpler to handle in their work flow or from
  their data production sources.

* In a module, so that administrators and users of Odoo who do not
  need or want an online import can avoid it being available to users.


Declared dependencies: `web`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 8 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 12 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "web"
  ],
  "data": [
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "base_import/static/src/**/*.scss",
      "base_import/static/src/**/*.js",
      "base_import/static/src/**/*.xml"
    ],
    "web.assets_unit_tests": [
      "base_import/static/tests/**/*.test.js"
    ]
  }
}
```

### Representative source files

- `addons/base_import/__init__.py` (5 lines)
- `addons/base_import/__manifest__.py` (43 lines)
- `addons/base_import/controllers/__init__.py` (4 lines)
- `addons/base_import/controllers/main.py` (22 lines)
- `addons/base_import/i18n/af.po` (954 lines)
- `addons/base_import/i18n/am.po` (950 lines)
- `addons/base_import/i18n/ar.po` (993 lines)
- `addons/base_import/i18n/az.po` (983 lines)
- `addons/base_import/i18n/base_import.pot` (950 lines)
- `addons/base_import/i18n/bg.po` (1,022 lines)
- `addons/base_import/i18n/bs.po` (975 lines)
- `addons/base_import/i18n/ca.po` (1,033 lines)
- `addons/base_import/i18n/cs.po` (1,019 lines)
- `addons/base_import/i18n/da.po` (1,011 lines)
- `addons/base_import/i18n/de.po` (1,047 lines)
- `addons/base_import/i18n/el.po` (970 lines)
- `addons/base_import/i18n/es.po` (1,050 lines)
- `addons/base_import/i18n/es_419.po` (1,044 lines)
- `addons/base_import/i18n/es_CL.po` (58 lines)
- `addons/base_import/i18n/et.po` (1,022 lines)
- `addons/base_import/i18n/eu.po` (953 lines)
- `addons/base_import/i18n/fa.po` (1,013 lines)
- `addons/base_import/i18n/fi.po` (1,056 lines)
- `addons/base_import/i18n/fo.po` (953 lines)
- `addons/base_import/i18n/fr.po` (1,053 lines)
- `addons/base_import/i18n/fr_CA.po` (58 lines)
- `addons/base_import/i18n/gl.po` (953 lines)
- `addons/base_import/i18n/gu.po` (954 lines)
- `addons/base_import/i18n/he.po` (1,002 lines)
- `addons/base_import/i18n/hi.po` (1,000 lines)
- `addons/base_import/i18n/hr.po` (1,044 lines)
- `addons/base_import/i18n/hu.po` (980 lines)
- `addons/base_import/i18n/id.po` (1,046 lines)
- `addons/base_import/i18n/is.po` (950 lines)
- `addons/base_import/i18n/it.po` (1,046 lines)
- `addons/base_import/i18n/ja.po` (1,034 lines)
- `addons/base_import/i18n/ka.po` (953 lines)
- `addons/base_import/i18n/kab.po` (968 lines)
- `addons/base_import/i18n/km.po` (955 lines)
- `addons/base_import/i18n/ko.po` (1,020 lines)
- `addons/base_import/i18n/ku.po` (959 lines)
- `addons/base_import/i18n/lo.po` (1,009 lines)
- `addons/base_import/i18n/lt.po` (989 lines)
- `addons/base_import/i18n/lv.po` (975 lines)
- `addons/base_import/i18n/mk.po` (953 lines)
- `addons/base_import/i18n/mn.po` (981 lines)
- `addons/base_import/i18n/my.po` (965 lines)
- `addons/base_import/i18n/nb.po` (974 lines)
- `addons/base_import/i18n/nl.po` (1,038 lines)
- `addons/base_import/i18n/pl.po` (1,040 lines)
- `addons/base_import/i18n/pt.po` (1,035 lines)
- `addons/base_import/i18n/pt_BR.po` (1,043 lines)
- `addons/base_import/i18n/ro.po` (1,024 lines)
- `addons/base_import/i18n/ru.po` (1,029 lines)
- `addons/base_import/i18n/sk.po` (992 lines)
- `addons/base_import/i18n/sl.po` (1,028 lines)
- `addons/base_import/i18n/sq.po` (953 lines)
- `addons/base_import/i18n/sr@latin.po` (965 lines)
- `addons/base_import/i18n/sv.po` (1,021 lines)
- `addons/base_import/i18n/th.po` (1,002 lines)
- `addons/base_import/i18n/tr.po` (1,020 lines)
- `addons/base_import/i18n/uk.po` (1,028 lines)
- `addons/base_import/i18n/uz.po` (1,104 lines)
- `addons/base_import/i18n/vi.po` (1,014 lines)
- `addons/base_import/i18n/zh_CN.po` (996 lines)
- `addons/base_import/i18n/zh_TW.po` (993 lines)
- `addons/base_import/models/__init__.py` (4 lines)
- `addons/base_import/models/base_import.py` (1,905 lines)
- `addons/base_import/models/odf_ods_reader.py` (93 lines)
- `addons/base_import/security/ir.access.csv` (3 lines)
- `addons/base_import/static/csv/External_id_3rd_party_application_product_categories.csv` (6 lines)
- `addons/base_import/static/csv/External_id_3rd_party_application_products.csv` (6 lines)
- `addons/base_import/static/csv/Name_products.csv` (6 lines)
- `addons/base_import/static/csv/database_import_test.sql` (175 lines)
- `addons/base_import/static/csv/m2m_customers_tags.csv` (6 lines)
- `addons/base_import/static/csv/o2m_customers_contacts.csv` (9 lines)
- `addons/base_import/static/csv/o2m_purchase_order_lines.csv` (6 lines)
- `addons/base_import/static/csv/purchase.order_functional_error_line_cant_adpat.csv` (3 lines)
- `addons/base_import/static/src/binary_file_manager.js` (91 lines)
- `addons/base_import/static/src/import_action/import_action.js` (309 lines)
- `addons/base_import/static/src/import_action/import_action.scss` (6 lines)
- `addons/base_import/static/src/import_action/import_action.xml` (80 lines)
- `addons/base_import/static/src/import_block_ui.js` (10 lines)
- `addons/base_import/static/src/import_block_ui.xml` (17 lines)
- `addons/base_import/static/src/import_data_column_error/import_data_column_error.js` (38 lines)
- `addons/base_import/static/src/import_data_column_error/import_data_column_error.xml` (42 lines)
- `addons/base_import/static/src/import_data_content/img/studio_icons.png` (63 lines)
- `addons/base_import/static/src/import_data_content/import_data_content.js` (118 lines)
- `addons/base_import/static/src/import_data_content/import_data_content.scss` (103 lines)
- `addons/base_import/static/src/import_data_content/import_data_content.xml` (130 lines)
- `addons/base_import/static/src/import_data_options/import_data_options.js` (77 lines)
- `addons/base_import/static/src/import_data_options/import_data_options.xml` (13 lines)
- `addons/base_import/static/src/import_data_progress/import_data_progress.js` (45 lines)
- `addons/base_import/static/src/import_data_progress/import_data_progress.scss` (6 lines)
- `addons/base_import/static/src/import_data_progress/import_data_progress.xml` (32 lines)
- `addons/base_import/static/src/import_data_sidepanel/import_data_sidepanel.js` (79 lines)
- `addons/base_import/static/src/import_data_sidepanel/import_data_sidepanel.scss` (26 lines)
- `addons/base_import/static/src/import_data_sidepanel/import_data_sidepanel.xml` (144 lines)
- `addons/base_import/static/src/import_model.js` (932 lines)
- `addons/base_import/static/src/import_records/import_records.js` (53 lines)
- `addons/base_import/static/src/import_records/import_records.xml` (10 lines)
- `addons/base_import/static/tests/import_action.test.js` (1,838 lines)
- `addons/base_import/static/tests/import_records.test.js` (228 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
