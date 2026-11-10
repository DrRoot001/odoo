# Module: base_install_request

- **Module ID:** MOD-039
- **Path:** `addons/base_install_request`
- **Manifest:** `addons/base_install_request/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Allow internal users requesting a module installation
=====================================================
    

Declared dependencies: `mail`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mail"
  ],
  "data": [
    "wizard/base_module_install_request_views.xml",
    "data/mail_templates.xml",
    "data/mail_templates_module_install.xml",
    "views/ir_module_module_views.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/base_install_request/__init__.py` (21 lines)
- `addons/base_install_request/__manifest__.py` (22 lines)
- `addons/base_install_request/data/mail_templates.xml` (26 lines)
- `addons/base_install_request/data/mail_templates_module_install.xml` (18 lines)
- `addons/base_install_request/i18n/ar.po` (219 lines)
- `addons/base_install_request/i18n/az.po` (217 lines)
- `addons/base_install_request/i18n/base_install_request.pot` (213 lines)
- `addons/base_install_request/i18n/bg.po` (217 lines)
- `addons/base_install_request/i18n/bs.po` (219 lines)
- `addons/base_install_request/i18n/ca.po` (219 lines)
- `addons/base_install_request/i18n/cs.po` (217 lines)
- `addons/base_install_request/i18n/da.po` (222 lines)
- `addons/base_install_request/i18n/de.po` (226 lines)
- `addons/base_install_request/i18n/el.po` (217 lines)
- `addons/base_install_request/i18n/es.po` (221 lines)
- `addons/base_install_request/i18n/es_419.po` (226 lines)
- `addons/base_install_request/i18n/et.po` (217 lines)
- `addons/base_install_request/i18n/fa.po` (217 lines)
- `addons/base_install_request/i18n/fi.po` (222 lines)
- `addons/base_install_request/i18n/fr.po` (226 lines)
- `addons/base_install_request/i18n/he.po` (218 lines)
- `addons/base_install_request/i18n/hi.po` (217 lines)
- `addons/base_install_request/i18n/hr.po` (218 lines)
- `addons/base_install_request/i18n/hu.po` (217 lines)
- `addons/base_install_request/i18n/id.po` (219 lines)
- `addons/base_install_request/i18n/it.po` (225 lines)
- `addons/base_install_request/i18n/ja.po` (225 lines)
- `addons/base_install_request/i18n/kab.po` (218 lines)
- `addons/base_install_request/i18n/ko.po` (218 lines)
- `addons/base_install_request/i18n/ku.po` (217 lines)
- `addons/base_install_request/i18n/lo.po` (224 lines)
- `addons/base_install_request/i18n/lt.po` (219 lines)
- `addons/base_install_request/i18n/lv.po` (219 lines)
- `addons/base_install_request/i18n/mn.po` (217 lines)
- `addons/base_install_request/i18n/my.po` (218 lines)
- `addons/base_install_request/i18n/nb.po` (217 lines)
- `addons/base_install_request/i18n/nl.po` (225 lines)
- `addons/base_install_request/i18n/pl.po` (224 lines)
- `addons/base_install_request/i18n/pt.po` (219 lines)
- `addons/base_install_request/i18n/pt_BR.po` (225 lines)
- `addons/base_install_request/i18n/ro.po` (219 lines)
- `addons/base_install_request/i18n/ru.po` (225 lines)
- `addons/base_install_request/i18n/sk.po` (218 lines)
- `addons/base_install_request/i18n/sl.po` (218 lines)
- `addons/base_install_request/i18n/sr@latin.po` (218 lines)
- `addons/base_install_request/i18n/sv.po` (219 lines)
- `addons/base_install_request/i18n/th.po` (223 lines)
- `addons/base_install_request/i18n/tr.po` (219 lines)
- `addons/base_install_request/i18n/uk.po` (218 lines)
- `addons/base_install_request/i18n/uz.po` (245 lines)
- `addons/base_install_request/i18n/vi.po` (218 lines)
- `addons/base_install_request/i18n/zh_CN.po` (226 lines)
- `addons/base_install_request/i18n/zh_TW.po` (223 lines)
- `addons/base_install_request/models/__init__.py` (4 lines)
- `addons/base_install_request/models/ir_module_module.py` (19 lines)
- `addons/base_install_request/security/ir.access.csv` (7 lines)
- `addons/base_install_request/views/ir_module_module_views.xml` (17 lines)
- `addons/base_install_request/wizard/__init__.py` (4 lines)
- `addons/base_install_request/wizard/base_module_install_request.py` (111 lines)
- `addons/base_install_request/wizard/base_module_install_request_views.xml` (44 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
