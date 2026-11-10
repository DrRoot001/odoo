# Module: http_routing

- **Module ID:** MOD-107
- **Path:** `addons/http_routing`
- **Manifest:** `addons/http_routing/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Web Routing


Proposes advanced routing options not available in web or base to keep
base modules simple.


Declared dependencies: `web`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 11 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 2 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "web"
  ],
  "data": [
    "views/http_routing_template.xml",
    "views/res_lang_views.xml"
  ]
}
```

### Representative source files

- `addons/http_routing/__init__.py` (12 lines)
- `addons/http_routing/__manifest__.py` (20 lines)
- `addons/http_routing/controllers/__init__.py` (4 lines)
- `addons/http_routing/controllers/main.py` (25 lines)
- `addons/http_routing/i18n/ar.po` (202 lines)
- `addons/http_routing/i18n/az.po` (201 lines)
- `addons/http_routing/i18n/bg.po` (197 lines)
- `addons/http_routing/i18n/bs.po` (200 lines)
- `addons/http_routing/i18n/ca.po` (210 lines)
- `addons/http_routing/i18n/cs.po` (202 lines)
- `addons/http_routing/i18n/da.po` (204 lines)
- `addons/http_routing/i18n/de.po` (212 lines)
- `addons/http_routing/i18n/el.po` (200 lines)
- `addons/http_routing/i18n/es.po` (208 lines)
- `addons/http_routing/i18n/es_419.po` (210 lines)
- `addons/http_routing/i18n/et.po` (209 lines)
- `addons/http_routing/i18n/fa.po` (202 lines)
- `addons/http_routing/i18n/fi.po` (212 lines)
- `addons/http_routing/i18n/fr.po` (207 lines)
- `addons/http_routing/i18n/he.po` (204 lines)
- `addons/http_routing/i18n/hi.po` (197 lines)
- `addons/http_routing/i18n/hr.po` (207 lines)
- `addons/http_routing/i18n/http_routing.pot` (194 lines)
- `addons/http_routing/i18n/hu.po` (207 lines)
- `addons/http_routing/i18n/id.po` (201 lines)
- `addons/http_routing/i18n/it.po` (212 lines)
- `addons/http_routing/i18n/ja.po` (204 lines)
- `addons/http_routing/i18n/kab.po` (198 lines)
- `addons/http_routing/i18n/ko.po` (204 lines)
- `addons/http_routing/i18n/ku.po` (197 lines)
- `addons/http_routing/i18n/lo.po` (203 lines)
- `addons/http_routing/i18n/lt.po` (205 lines)
- `addons/http_routing/i18n/lv.po` (198 lines)
- `addons/http_routing/i18n/mn.po` (202 lines)
- `addons/http_routing/i18n/my.po` (197 lines)
- `addons/http_routing/i18n/nb.po` (202 lines)
- `addons/http_routing/i18n/nl.po` (204 lines)
- `addons/http_routing/i18n/pl.po` (210 lines)
- `addons/http_routing/i18n/pt.po` (205 lines)
- `addons/http_routing/i18n/pt_BR.po` (213 lines)
- `addons/http_routing/i18n/ro.po` (208 lines)
- `addons/http_routing/i18n/ru.po` (204 lines)
- `addons/http_routing/i18n/sk.po` (201 lines)
- `addons/http_routing/i18n/sl.po` (201 lines)
- `addons/http_routing/i18n/sr@latin.po` (202 lines)
- `addons/http_routing/i18n/sv.po` (211 lines)
- `addons/http_routing/i18n/th.po` (203 lines)
- `addons/http_routing/i18n/tr.po` (211 lines)
- `addons/http_routing/i18n/uk.po` (205 lines)
- `addons/http_routing/i18n/uz.po` (229 lines)
- `addons/http_routing/i18n/vi.po` (204 lines)
- `addons/http_routing/i18n/zh_CN.po` (205 lines)
- `addons/http_routing/i18n/zh_TW.po` (202 lines)
- `addons/http_routing/models/__init__.py` (6 lines)
- `addons/http_routing/models/ir_http.py` (644 lines)
- `addons/http_routing/models/ir_qweb.py` (15 lines)
- `addons/http_routing/models/res_lang.py` (14 lines)
- `addons/http_routing/static/shapes/404.svg` (15 lines)
- `addons/http_routing/tests/__init__.py` (2 lines)
- `addons/http_routing/tests/common.py` (126 lines)
- `addons/http_routing/tests/test_res_lang.py` (14 lines)
- `addons/http_routing/views/http_routing_template.xml` (270 lines)
- `addons/http_routing/views/res_lang_views.xml` (24 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
