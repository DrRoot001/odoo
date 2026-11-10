# Module: base_sparse_field

- **Module ID:** MOD-043
- **Path:** `addons/base_sparse_field`
- **Manifest:** `addons/base_sparse_field/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Implementation of sparse fields.


The purpose of this module is to implement "sparse" fields, i.e., fields
that are mostly null. This implementation circumvents the PostgreSQL
limitation on the number of columns in a table. The values of all sparse
fields are stored in a "serialized" field in the form of a JSON mapping.
    

Declared dependencies: `base`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
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
    "views/views.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/base_sparse_field/__init__.py` (3 lines)
- `addons/base_sparse_field/__manifest__.py` (18 lines)
- `addons/base_sparse_field/i18n/af.po` (175 lines)
- `addons/base_sparse_field/i18n/am.po` (171 lines)
- `addons/base_sparse_field/i18n/ar.po` (183 lines)
- `addons/base_sparse_field/i18n/az.po` (178 lines)
- `addons/base_sparse_field/i18n/base_sparse_field.pot` (171 lines)
- `addons/base_sparse_field/i18n/bg.po` (183 lines)
- `addons/base_sparse_field/i18n/bs.po` (183 lines)
- `addons/base_sparse_field/i18n/ca.po` (185 lines)
- `addons/base_sparse_field/i18n/cs.po` (183 lines)
- `addons/base_sparse_field/i18n/da.po` (183 lines)
- `addons/base_sparse_field/i18n/de.po` (192 lines)
- `addons/base_sparse_field/i18n/el.po` (182 lines)
- `addons/base_sparse_field/i18n/es.po` (195 lines)
- `addons/base_sparse_field/i18n/es_419.po` (191 lines)
- `addons/base_sparse_field/i18n/es_CL.po` (57 lines)
- `addons/base_sparse_field/i18n/et.po` (185 lines)
- `addons/base_sparse_field/i18n/eu.po` (174 lines)
- `addons/base_sparse_field/i18n/fa.po` (184 lines)
- `addons/base_sparse_field/i18n/fi.po` (193 lines)
- `addons/base_sparse_field/i18n/fo.po` (174 lines)
- `addons/base_sparse_field/i18n/fr.po` (197 lines)
- `addons/base_sparse_field/i18n/fr_CA.po` (57 lines)
- `addons/base_sparse_field/i18n/gl.po` (174 lines)
- `addons/base_sparse_field/i18n/gu.po` (175 lines)
- `addons/base_sparse_field/i18n/he.po` (184 lines)
- `addons/base_sparse_field/i18n/hi.po` (175 lines)
- `addons/base_sparse_field/i18n/hr.po` (186 lines)
- `addons/base_sparse_field/i18n/hu.po` (185 lines)
- `addons/base_sparse_field/i18n/id.po` (185 lines)
- `addons/base_sparse_field/i18n/is.po` (174 lines)
- `addons/base_sparse_field/i18n/it.po` (194 lines)
- `addons/base_sparse_field/i18n/ja.po` (190 lines)
- `addons/base_sparse_field/i18n/ka.po` (174 lines)
- `addons/base_sparse_field/i18n/kab.po` (177 lines)
- `addons/base_sparse_field/i18n/km.po` (174 lines)
- `addons/base_sparse_field/i18n/ko.po` (183 lines)
- `addons/base_sparse_field/i18n/ku.po` (175 lines)
- `addons/base_sparse_field/i18n/lo.po` (186 lines)
- `addons/base_sparse_field/i18n/lt.po` (188 lines)
- `addons/base_sparse_field/i18n/lv.po` (183 lines)
- `addons/base_sparse_field/i18n/mk.po` (174 lines)
- `addons/base_sparse_field/i18n/mn.po` (182 lines)
- `addons/base_sparse_field/i18n/my.po` (176 lines)
- `addons/base_sparse_field/i18n/nb.po` (180 lines)
- `addons/base_sparse_field/i18n/nl.po` (185 lines)
- `addons/base_sparse_field/i18n/pl.po` (193 lines)
- `addons/base_sparse_field/i18n/pt.po` (190 lines)
- `addons/base_sparse_field/i18n/pt_BR.po` (193 lines)
- `addons/base_sparse_field/i18n/ro.po` (184 lines)
- `addons/base_sparse_field/i18n/ru.po` (183 lines)
- `addons/base_sparse_field/i18n/sk.po` (181 lines)
- `addons/base_sparse_field/i18n/sl.po` (186 lines)
- `addons/base_sparse_field/i18n/sq.po` (174 lines)
- `addons/base_sparse_field/i18n/sr@latin.po` (180 lines)
- `addons/base_sparse_field/i18n/sv.po` (188 lines)
- `addons/base_sparse_field/i18n/th.po` (183 lines)
- `addons/base_sparse_field/i18n/tr.po` (187 lines)
- `addons/base_sparse_field/i18n/uk.po` (186 lines)
- `addons/base_sparse_field/i18n/uz.po` (211 lines)
- `addons/base_sparse_field/i18n/vi.po` (184 lines)
- `addons/base_sparse_field/i18n/zh_CN.po` (186 lines)
- `addons/base_sparse_field/i18n/zh_TW.po` (181 lines)
- `addons/base_sparse_field/models/__init__.py` (4 lines)
- `addons/base_sparse_field/models/fields.py` (96 lines)
- `addons/base_sparse_field/models/models.py` (102 lines)
- `addons/base_sparse_field/security/ir.access.csv` (2 lines)
- `addons/base_sparse_field/tests/__init__.py` (3 lines)
- `addons/base_sparse_field/tests/test_sparse_fields.py` (41 lines)
- `addons/base_sparse_field/views/views.xml` (32 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
