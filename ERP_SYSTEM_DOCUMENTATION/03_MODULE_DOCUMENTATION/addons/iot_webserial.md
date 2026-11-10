# Module: iot_webserial

- **Module ID:** MOD-113
- **Path:** `addons/iot_webserial`
- **Manifest:** `addons/iot_webserial/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Interface with serial devices directly via the browser using Web Serial.


This module provides support for interfacing with serial devices locally via the Web Serial API.
Since the browser is used directly no IoT box is required.


Declared dependencies: `web`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 2 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 6 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "web"
  ],
  "assets": {
    "web.assets_backend": [
      "iot_webserial/static/src/**/*"
    ],
    "web.assets_unit_tests": [
      "iot_webserial/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/iot_webserial/__init__.py` (0 lines)
- `addons/iot_webserial/__manifest__.py` (21 lines)
- `addons/iot_webserial/i18n/iot_webserial.pot` (85 lines)
- `addons/iot_webserial/static/src/web_serial_device.js` (115 lines)
- `addons/iot_webserial/static/src/web_serial_scale.js` (83 lines)
- `addons/iot_webserial/static/src/widgets/connect_web_serial_scale/connect_web_serial_scale.js` (80 lines)
- `addons/iot_webserial/static/src/widgets/connect_web_serial_scale/connect_web_serial_scale.xml` (10 lines)
- `addons/iot_webserial/static/tests/fake_serial_port.js` (45 lines)
- `addons/iot_webserial/static/tests/web_serial_device.test.js` (54 lines)
- `addons/iot_webserial/static/tests/web_serial_scale.test.js` (107 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
