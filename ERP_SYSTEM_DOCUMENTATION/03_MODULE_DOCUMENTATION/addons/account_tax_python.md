# Module: account_tax_python

- **Module ID:** MOD-014
- **Path:** `addons/account_tax_python`
- **Manifest:** `addons/account_tax_python/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Use python code to define taxes


A tax defined as python code consists of two snippets of python code which are executed in a local environment containing data such as the unit price, product or partner.

"Applicable Code" defines if the tax is to be applied.

"Python Code" defines the amount of the tax.
        

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account"
  ],
  "data": [
    "views/account_tax_views.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "account_tax_python/static/src/helpers/*.js"
    ],
    "web.assets_frontend": [
      "account_tax_python/static/src/helpers/*.js"
    ]
  }
}
```

### Representative source files

- `addons/account_tax_python/__init__.py` (4 lines)
- `addons/account_tax_python/__manifest__.py` (28 lines)
- `addons/account_tax_python/i18n/account_tax_python.pot` (158 lines)
- `addons/account_tax_python/i18n/ar.po` (192 lines)
- `addons/account_tax_python/i18n/az.po` (166 lines)
- `addons/account_tax_python/i18n/bg.po` (168 lines)
- `addons/account_tax_python/i18n/bs.po` (167 lines)
- `addons/account_tax_python/i18n/ca.po` (186 lines)
- `addons/account_tax_python/i18n/cs.po` (180 lines)
- `addons/account_tax_python/i18n/da.po` (185 lines)
- `addons/account_tax_python/i18n/de.po` (196 lines)
- `addons/account_tax_python/i18n/el.po` (178 lines)
- `addons/account_tax_python/i18n/es.po` (201 lines)
- `addons/account_tax_python/i18n/es_419.po` (195 lines)
- `addons/account_tax_python/i18n/et.po` (185 lines)
- `addons/account_tax_python/i18n/fa.po` (180 lines)
- `addons/account_tax_python/i18n/fi.po` (195 lines)
- `addons/account_tax_python/i18n/fr.po` (200 lines)
- `addons/account_tax_python/i18n/gu.po` (164 lines)
- `addons/account_tax_python/i18n/he.po` (177 lines)
- `addons/account_tax_python/i18n/hi.po` (181 lines)
- `addons/account_tax_python/i18n/hr.po` (170 lines)
- `addons/account_tax_python/i18n/hu.po` (178 lines)
- `addons/account_tax_python/i18n/id.po` (194 lines)
- `addons/account_tax_python/i18n/is.po` (160 lines)
- `addons/account_tax_python/i18n/it.po` (198 lines)
- `addons/account_tax_python/i18n/ja.po` (193 lines)
- `addons/account_tax_python/i18n/kab.po` (164 lines)
- `addons/account_tax_python/i18n/kk.po` (162 lines)
- `addons/account_tax_python/i18n/ko.po` (184 lines)
- `addons/account_tax_python/i18n/ku.po` (164 lines)
- `addons/account_tax_python/i18n/lo.po` (188 lines)
- `addons/account_tax_python/i18n/lt.po` (170 lines)
- `addons/account_tax_python/i18n/lv.po` (168 lines)
- `addons/account_tax_python/i18n/mn.po` (178 lines)
- `addons/account_tax_python/i18n/my.po` (164 lines)
- `addons/account_tax_python/i18n/nb.po` (168 lines)
- `addons/account_tax_python/i18n/nl.po` (186 lines)
- `addons/account_tax_python/i18n/pl.po` (198 lines)
- `addons/account_tax_python/i18n/pt.po` (188 lines)
- `addons/account_tax_python/i18n/pt_BR.po` (196 lines)
- `addons/account_tax_python/i18n/ro.po` (187 lines)
- `addons/account_tax_python/i18n/ru.po` (188 lines)
- `addons/account_tax_python/i18n/sk.po` (168 lines)
- `addons/account_tax_python/i18n/sl.po` (184 lines)
- `addons/account_tax_python/i18n/sr@latin.po` (184 lines)
- `addons/account_tax_python/i18n/sv.po` (199 lines)
- `addons/account_tax_python/i18n/ta.po` (162 lines)
- `addons/account_tax_python/i18n/te.po` (162 lines)
- `addons/account_tax_python/i18n/th.po` (185 lines)
- `addons/account_tax_python/i18n/tr.po` (198 lines)
- `addons/account_tax_python/i18n/uk.po` (187 lines)
- `addons/account_tax_python/i18n/uz.po` (200 lines)
- `addons/account_tax_python/i18n/vi.po` (185 lines)
- `addons/account_tax_python/i18n/zh_CN.po` (193 lines)
- `addons/account_tax_python/i18n/zh_TW.po` (183 lines)
- `addons/account_tax_python/models/__init__.py` (4 lines)
- `addons/account_tax_python/models/account_tax.py` (120 lines)
- `addons/account_tax_python/static/src/helpers/account_tax.js` (33 lines)
- `addons/account_tax_python/tests/__init__.py` (2 lines)
- `addons/account_tax_python/tests/common.py` (38 lines)
- `addons/account_tax_python/tests/test_taxes_computation.py` (242 lines)
- `addons/account_tax_python/tools/formula_utils.py` (165 lines)
- `addons/account_tax_python/views/account_tax_views.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
