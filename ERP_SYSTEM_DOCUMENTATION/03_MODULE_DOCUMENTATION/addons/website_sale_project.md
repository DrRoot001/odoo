# Module: website_sale_project

- **Module ID:** MOD-640
- **Path:** `addons/website_sale_project`
- **Manifest:** `addons/website_sale_project/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Bridge module between website_sale and project


Bridge module between website_sale and project.
    

Declared dependencies: `website_sale`, `project`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website_sale",
    "project"
  ],
  "data": [
    "data/website_sale_project_data.xml"
  ],
  "assets": {
    "website.website_builder_assets": [
      "website_sale_project/static/src/website_builder/**/*"
    ]
  }
}
```

### Representative source files

- `addons/website_sale_project/__init__.py` (3 lines)
- `addons/website_sale_project/__manifest__.py` (22 lines)
- `addons/website_sale_project/data/website_sale_project_data.xml` (7 lines)
- `addons/website_sale_project/i18n/ar.po` (71 lines)
- `addons/website_sale_project/i18n/az.po` (71 lines)
- `addons/website_sale_project/i18n/bg.po` (71 lines)
- `addons/website_sale_project/i18n/bs.po` (71 lines)
- `addons/website_sale_project/i18n/ca.po` (71 lines)
- `addons/website_sale_project/i18n/cs.po` (71 lines)
- `addons/website_sale_project/i18n/da.po` (71 lines)
- `addons/website_sale_project/i18n/de.po` (79 lines)
- `addons/website_sale_project/i18n/el.po` (71 lines)
- `addons/website_sale_project/i18n/es.po` (75 lines)
- `addons/website_sale_project/i18n/es_419.po` (75 lines)
- `addons/website_sale_project/i18n/et.po` (71 lines)
- `addons/website_sale_project/i18n/fa.po` (71 lines)
- `addons/website_sale_project/i18n/fi.po` (75 lines)
- `addons/website_sale_project/i18n/fr.po` (71 lines)
- `addons/website_sale_project/i18n/he.po` (71 lines)
- `addons/website_sale_project/i18n/hi.po` (71 lines)
- `addons/website_sale_project/i18n/hr.po` (71 lines)
- `addons/website_sale_project/i18n/hu.po` (71 lines)
- `addons/website_sale_project/i18n/id.po` (71 lines)
- `addons/website_sale_project/i18n/it.po` (77 lines)
- `addons/website_sale_project/i18n/ja.po` (71 lines)
- `addons/website_sale_project/i18n/kab.po` (71 lines)
- `addons/website_sale_project/i18n/ko.po` (71 lines)
- `addons/website_sale_project/i18n/ku.po` (71 lines)
- `addons/website_sale_project/i18n/lo.po` (71 lines)
- `addons/website_sale_project/i18n/lt.po` (71 lines)
- `addons/website_sale_project/i18n/lv.po` (71 lines)
- `addons/website_sale_project/i18n/mn.po` (71 lines)
- `addons/website_sale_project/i18n/my.po` (75 lines)
- `addons/website_sale_project/i18n/nb.po` (71 lines)
- `addons/website_sale_project/i18n/nl.po` (75 lines)
- `addons/website_sale_project/i18n/pl.po` (71 lines)
- `addons/website_sale_project/i18n/pt.po` (71 lines)
- `addons/website_sale_project/i18n/pt_BR.po` (84 lines)
- `addons/website_sale_project/i18n/ro.po` (71 lines)
- `addons/website_sale_project/i18n/ru.po` (71 lines)
- `addons/website_sale_project/i18n/sk.po` (71 lines)
- `addons/website_sale_project/i18n/sl.po` (71 lines)
- `addons/website_sale_project/i18n/sr@latin.po` (71 lines)
- `addons/website_sale_project/i18n/sv.po` (75 lines)
- `addons/website_sale_project/i18n/th.po` (71 lines)
- `addons/website_sale_project/i18n/tr.po` (71 lines)
- `addons/website_sale_project/i18n/uk.po` (71 lines)
- `addons/website_sale_project/i18n/uz.po` (71 lines)
- `addons/website_sale_project/i18n/vi.po` (71 lines)
- `addons/website_sale_project/i18n/website_sale_project.pot` (71 lines)
- `addons/website_sale_project/i18n/zh_CN.po` (77 lines)
- `addons/website_sale_project/i18n/zh_TW.po` (71 lines)
- `addons/website_sale_project/models/__init__.py` (3 lines)
- `addons/website_sale_project/models/withdrawal_request.py` (45 lines)
- `addons/website_sale_project/static/src/website_builder/website_sale_project_form_editor.js` (22 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
