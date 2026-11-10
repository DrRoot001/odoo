# Module: test_http

- **Module ID:** MOD-656
- **Path:** `odoo/addons/test_http`
- **Manifest:** `odoo/addons/test_http/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

A module to test HTTP

Declared dependencies: `web`, `web_tour`, `mail`, `rpc`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 27 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 1 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 20 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 44 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "web",
    "web_tour",
    "mail",
    "rpc"
  ],
  "data": [
    "data.xml",
    "views.xml",
    "ir.access.csv"
  ]
}
```

### Representative source files

- `odoo/addons/test_http/__init__.py` (2 lines)
- `odoo/addons/test_http/__manifest__.py` (14 lines)
- `odoo/addons/test_http/controllers.py` (403 lines)
- `odoo/addons/test_http/data.xml` (84 lines)
- `odoo/addons/test_http/ir.access.csv` (8 lines)
- `odoo/addons/test_http/models/__init__.py` (2 lines)
- `odoo/addons/test_http/models/rpc.py` (36 lines)
- `odoo/addons/test_http/models/stargate.py` (89 lines)
- `odoo/addons/test_http/static/src/img/gizeh.png` (13 lines)
- `odoo/addons/test_http/static/src/img/milky_way.jpg` (72 lines)
- `odoo/addons/test_http/static/src/img/pegasus.jpg` (88 lines)
- `odoo/addons/test_http/static/src/img/xss.svg` (3 lines)
- `odoo/addons/test_http/tests/__init__.py` (19 lines)
- `odoo/addons/test_http/tests/test_auth_custom.py` (48 lines)
- `odoo/addons/test_http/tests/test_bearer_scope.py` (32 lines)
- `odoo/addons/test_http/tests/test_captcha.py` (45 lines)
- `odoo/addons/test_http/tests/test_common.py` (64 lines)
- `odoo/addons/test_http/tests/test_device.py` (714 lines)
- `odoo/addons/test_http/tests/test_echo_reply.py` (276 lines)
- `odoo/addons/test_http/tests/test_error_http.py` (111 lines)
- `odoo/addons/test_http/tests/test_error_rpc.py` (90 lines)
- `odoo/addons/test_http/tests/test_greeting.py` (113 lines)
- `odoo/addons/test_http/tests/test_misc.py` (402 lines)
- `odoo/addons/test_http/tests/test_models.py` (113 lines)
- `odoo/addons/test_http/tests/test_rpc_path.py` (80 lines)
- `odoo/addons/test_http/tests/test_security.py` (20 lines)
- `odoo/addons/test_http/tests/test_session.py` (506 lines)
- `odoo/addons/test_http/tests/test_static.py` (742 lines)
- `odoo/addons/test_http/tests/test_web_server.py` (48 lines)
- `odoo/addons/test_http/tests/test_webjson.py` (357 lines)
- `odoo/addons/test_http/tests/test_webjson2.py` (373 lines)
- `odoo/addons/test_http/tests/test_xss.py` (20 lines)
- `odoo/addons/test_http/utils.py` (125 lines)
- `odoo/addons/test_http/views.xml` (118 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
