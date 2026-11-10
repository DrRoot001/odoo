# Module: rpc

- **Module ID:** MOD-508
- **Path:** `addons/rpc`
- **Manifest:** `addons/rpc/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Standard Odoo RPC endpoints to models
=====================================

This module provides the /xmlrpc and /jsonrpc endpoints used to
programmatically access models.


Declared dependencies: `base`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 4 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 6 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base"
  ]
}
```

### Representative source files

- `addons/rpc/__init__.py` (1 lines)
- `addons/rpc/__manifest__.py` (15 lines)
- `addons/rpc/controllers/__init__.py` (29 lines)
- `addons/rpc/controllers/json2.py` (90 lines)
- `addons/rpc/controllers/jsonrpc.py` (17 lines)
- `addons/rpc/controllers/xmlrpc.py` (171 lines)
- `addons/rpc/i18n/ar.po` (31 lines)
- `addons/rpc/i18n/az.po` (31 lines)
- `addons/rpc/i18n/bg.po` (31 lines)
- `addons/rpc/i18n/bs.po` (31 lines)
- `addons/rpc/i18n/ca.po` (31 lines)
- `addons/rpc/i18n/cs.po` (31 lines)
- `addons/rpc/i18n/da.po` (31 lines)
- `addons/rpc/i18n/de.po` (39 lines)
- `addons/rpc/i18n/el.po` (31 lines)
- `addons/rpc/i18n/es.po` (41 lines)
- `addons/rpc/i18n/es_419.po` (31 lines)
- `addons/rpc/i18n/et.po` (31 lines)
- `addons/rpc/i18n/fa.po` (31 lines)
- `addons/rpc/i18n/fi.po` (31 lines)
- `addons/rpc/i18n/fr.po` (31 lines)
- `addons/rpc/i18n/he.po` (31 lines)
- `addons/rpc/i18n/hi.po` (31 lines)
- `addons/rpc/i18n/hr.po` (31 lines)
- `addons/rpc/i18n/hu.po` (31 lines)
- `addons/rpc/i18n/id.po` (31 lines)
- `addons/rpc/i18n/it.po` (40 lines)
- `addons/rpc/i18n/ja.po` (31 lines)
- `addons/rpc/i18n/kab.po` (31 lines)
- `addons/rpc/i18n/ko.po` (31 lines)
- `addons/rpc/i18n/ku.po` (31 lines)
- `addons/rpc/i18n/lo.po` (31 lines)
- `addons/rpc/i18n/lt.po` (31 lines)
- `addons/rpc/i18n/lv.po` (31 lines)
- `addons/rpc/i18n/mn.po` (31 lines)
- `addons/rpc/i18n/my.po` (31 lines)
- `addons/rpc/i18n/nb.po` (31 lines)
- `addons/rpc/i18n/nl.po` (39 lines)
- `addons/rpc/i18n/pl.po` (31 lines)
- `addons/rpc/i18n/pt.po` (31 lines)
- `addons/rpc/i18n/pt_BR.po` (43 lines)
- `addons/rpc/i18n/ro.po` (31 lines)
- `addons/rpc/i18n/rpc.pot` (31 lines)
- `addons/rpc/i18n/ru.po` (31 lines)
- `addons/rpc/i18n/sk.po` (31 lines)
- `addons/rpc/i18n/sl.po` (31 lines)
- `addons/rpc/i18n/sr@latin.po` (31 lines)
- `addons/rpc/i18n/sv.po` (31 lines)
- `addons/rpc/i18n/th.po` (31 lines)
- `addons/rpc/i18n/tr.po` (31 lines)
- `addons/rpc/i18n/uk.po` (31 lines)
- `addons/rpc/i18n/uz.po` (31 lines)
- `addons/rpc/i18n/vi.po` (31 lines)
- `addons/rpc/i18n/zh_CN.po` (31 lines)
- `addons/rpc/i18n/zh_TW.po` (31 lines)
- `addons/rpc/tests/__init__.py` (1 lines)
- `addons/rpc/tests/test_xmlrpc.py` (358 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
