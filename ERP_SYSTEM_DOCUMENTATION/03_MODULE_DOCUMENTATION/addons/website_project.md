# Module: website_project

- **Module ID:** MOD-633
- **Path:** `addons/website_project`
- **Manifest:** `addons/website_project/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Add a task suggestion form to your website


Generate tasks in Project app from a form published on your website. This module requires the use of the *Form Builder* module in order to build the form.
    

Declared dependencies: `website`, `project`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website",
    "project"
  ],
  "data": [
    "data/website_project_data.xml",
    "views/project_portal_project_task_template.xml",
    "views/project_portal_project_project_template.xml"
  ],
  "assets": {
    "website.website_builder_assets": [
      "website_project/static/src/js/website_project_editor.js"
    ],
    "website.assets_inside_builder_iframe": [
      "website_project/static/src/js/*.edit.*"
    ],
    "project.webclient": [
      "website/static/src/js/utils.js",
      "web/static/src/core/autocomplete/*",
      "website/static/src/components/autocomplete_with_pages/*"
    ]
  }
}
```

### Representative source files

- `addons/website_project/__init__.py` (4 lines)
- `addons/website_project/__manifest__.py` (37 lines)
- `addons/website_project/controllers/__init__.py` (1 lines)
- `addons/website_project/controllers/main.py` (72 lines)
- `addons/website_project/data/website_project_data.xml` (23 lines)
- `addons/website_project/i18n/ar.po` (200 lines)
- `addons/website_project/i18n/az.po` (182 lines)
- `addons/website_project/i18n/bg.po` (182 lines)
- `addons/website_project/i18n/bs.po` (184 lines)
- `addons/website_project/i18n/ca.po` (183 lines)
- `addons/website_project/i18n/cs.po` (187 lines)
- `addons/website_project/i18n/da.po` (186 lines)
- `addons/website_project/i18n/de.po` (203 lines)
- `addons/website_project/i18n/el.po` (183 lines)
- `addons/website_project/i18n/es.po` (201 lines)
- `addons/website_project/i18n/es_419.po` (196 lines)
- `addons/website_project/i18n/et.po` (182 lines)
- `addons/website_project/i18n/fa.po` (182 lines)
- `addons/website_project/i18n/fi.po` (195 lines)
- `addons/website_project/i18n/fr.po` (198 lines)
- `addons/website_project/i18n/he.po` (186 lines)
- `addons/website_project/i18n/hi.po` (182 lines)
- `addons/website_project/i18n/hr.po` (189 lines)
- `addons/website_project/i18n/hu.po` (187 lines)
- `addons/website_project/i18n/id.po` (196 lines)
- `addons/website_project/i18n/it.po` (202 lines)
- `addons/website_project/i18n/ja.po` (195 lines)
- `addons/website_project/i18n/kab.po` (183 lines)
- `addons/website_project/i18n/ko.po` (195 lines)
- `addons/website_project/i18n/ku.po` (182 lines)
- `addons/website_project/i18n/lo.po` (197 lines)
- `addons/website_project/i18n/lt.po` (188 lines)
- `addons/website_project/i18n/lv.po` (183 lines)
- `addons/website_project/i18n/mn.po` (186 lines)
- `addons/website_project/i18n/my.po` (183 lines)
- `addons/website_project/i18n/nb.po` (185 lines)
- `addons/website_project/i18n/nl.po` (198 lines)
- `addons/website_project/i18n/pl.po` (202 lines)
- `addons/website_project/i18n/pt.po` (183 lines)
- `addons/website_project/i18n/pt_BR.po` (204 lines)
- `addons/website_project/i18n/ro.po` (184 lines)
- `addons/website_project/i18n/ru.po` (198 lines)
- `addons/website_project/i18n/sk.po` (182 lines)
- `addons/website_project/i18n/sl.po` (184 lines)
- `addons/website_project/i18n/sr@latin.po` (183 lines)
- `addons/website_project/i18n/sv.po` (184 lines)
- `addons/website_project/i18n/th.po` (195 lines)
- `addons/website_project/i18n/tr.po` (200 lines)
- `addons/website_project/i18n/uk.po` (189 lines)
- `addons/website_project/i18n/uz.po` (218 lines)
- `addons/website_project/i18n/vi.po` (199 lines)
- `addons/website_project/i18n/website_project.pot` (176 lines)
- `addons/website_project/i18n/zh_CN.po` (201 lines)
- `addons/website_project/i18n/zh_TW.po` (198 lines)
- `addons/website_project/models/__init__.py` (3 lines)
- `addons/website_project/models/project_task.py` (9 lines)
- `addons/website_project/static/description/icon.png` (25 lines)
- `addons/website_project/static/description/icon.svg` (1 lines)
- `addons/website_project/static/src/js/website_project_editor.edit.js` (53 lines)
- `addons/website_project/static/src/js/website_project_editor.js` (17 lines)
- `addons/website_project/tests/__init__.py` (3 lines)
- `addons/website_project/tests/test_project_portal_access.py` (182 lines)
- `addons/website_project/views/project_portal_project_project_template.xml` (9 lines)
- `addons/website_project/views/project_portal_project_task_template.xml` (42 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
