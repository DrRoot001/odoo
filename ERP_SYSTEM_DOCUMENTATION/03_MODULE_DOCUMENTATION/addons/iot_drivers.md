# Module: iot_drivers

- **Module ID:** MOD-112
- **Path:** `addons/iot_drivers`
- **Manifest:** `addons/iot_drivers/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `False`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Connect the Web Client to Hardware Peripherals


Hardware Poxy
=============

This module allows you to remotely use peripherals connected to this server.

This modules only contains the enabling framework. The actual devices drivers
are found in other modules that must be installed separately.



Declared dependencies: None declared.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 51 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 5 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 19 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 31 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "assets": {
    "iot_drivers.assets": [
      "iot_drivers/static/**/*"
    ]
  }
}
```

### Representative source files

- `addons/iot_drivers/__init__.py` (35 lines)
- `addons/iot_drivers/__manifest__.py` (27 lines)
- `addons/iot_drivers/browser.py` (127 lines)
- `addons/iot_drivers/cli/genproxytoken.py` (28 lines)
- `addons/iot_drivers/connection_manager.py` (118 lines)
- `addons/iot_drivers/controllers/__init__.py` (6 lines)
- `addons/iot_drivers/controllers/driver.py` (94 lines)
- `addons/iot_drivers/controllers/homepage.py` (494 lines)
- `addons/iot_drivers/controllers/l10n_eg_eta_usb.py` (156 lines)
- `addons/iot_drivers/controllers/proxy.py` (10 lines)
- `addons/iot_drivers/driver.py` (104 lines)
- `addons/iot_drivers/event_manager.py` (83 lines)
- `addons/iot_drivers/exception_logger.py` (30 lines)
- `addons/iot_drivers/http.py` (13 lines)
- `addons/iot_drivers/interface.py` (109 lines)
- `addons/iot_drivers/iot_handlers/__init__.py` (23 lines)
- `addons/iot_drivers/iot_handlers/drivers/bluetooth_caliper_driver_L.py` (119 lines)
- `addons/iot_drivers/iot_handlers/drivers/camera_driver_L.py` (44 lines)
- `addons/iot_drivers/iot_handlers/drivers/ctypes_terminal_driver.py` (251 lines)
- `addons/iot_drivers/iot_handlers/drivers/display_driver_L.py` (156 lines)
- `addons/iot_drivers/iot_handlers/drivers/keyboard_driver_L.py` (340 lines)
- `addons/iot_drivers/iot_handlers/drivers/l10n_ke_edi_serial_driver.py` (255 lines)
- `addons/iot_drivers/iot_handlers/drivers/printer_driver_L.py` (256 lines)
- `addons/iot_drivers/iot_handlers/drivers/printer_driver_W.py` (159 lines)
- `addons/iot_drivers/iot_handlers/drivers/printer_driver_base.py` (231 lines)
- `addons/iot_drivers/iot_handlers/drivers/serial_blackbox_be_driver.py` (327 lines)
- `addons/iot_drivers/iot_handlers/drivers/serial_blackbox_se_driver.py` (279 lines)
- `addons/iot_drivers/iot_handlers/drivers/serial_caliper_driver.py` (72 lines)
- `addons/iot_drivers/iot_handlers/drivers/serial_driver_base.py` (116 lines)
- `addons/iot_drivers/iot_handlers/drivers/serial_scale_driver.py` (147 lines)
- `addons/iot_drivers/iot_handlers/drivers/six_driver.py` (163 lines)
- `addons/iot_drivers/iot_handlers/drivers/worldline_driver.py` (122 lines)
- `addons/iot_drivers/iot_handlers/interfaces/bluetooth_interface_L.py` (143 lines)
- `addons/iot_drivers/iot_handlers/interfaces/camera_interface_L.py` (22 lines)
- `addons/iot_drivers/iot_handlers/interfaces/ctep_interface.py` (90 lines)
- `addons/iot_drivers/iot_handlers/interfaces/display_interface_L.py` (38 lines)
- `addons/iot_drivers/iot_handlers/interfaces/printer_interface_L.py` (268 lines)
- `addons/iot_drivers/iot_handlers/interfaces/printer_interface_W.py` (45 lines)
- `addons/iot_drivers/iot_handlers/interfaces/serial_interface.py` (30 lines)
- `addons/iot_drivers/iot_handlers/interfaces/tim_interface.py` (104 lines)
- `addons/iot_drivers/iot_handlers/interfaces/usb_interface_L.py` (49 lines)
- `addons/iot_drivers/main.py` (226 lines)
- `addons/iot_drivers/static/img/background-light.svg` (35 lines)
- `addons/iot_drivers/static/img/favicon.png` (18 lines)
- `addons/iot_drivers/static/src/app/components/dialog/credentials_dialog.js` (84 lines)
- `addons/iot_drivers/static/src/app/components/dialog/database_dialog.js` (91 lines)
- `addons/iot_drivers/static/src/app/components/dialog/debugging_tools_dialog.js` (145 lines)
- `addons/iot_drivers/static/src/app/components/dialog/device_dialog.js` (89 lines)
- `addons/iot_drivers/static/src/app/components/dialog/dialog.js` (49 lines)
- `addons/iot_drivers/static/src/app/components/dialog/handlers_dialog.js` (165 lines)
- `addons/iot_drivers/static/src/app/components/dialog/six_terminal_dialog.js` (86 lines)
- `addons/iot_drivers/static/src/app/components/dialog/time_dialog.js` (70 lines)
- `addons/iot_drivers/static/src/app/components/dialog/update_dialog.js` (58 lines)
- `addons/iot_drivers/static/src/app/components/dialog/wifi_dialog.js` (180 lines)
- `addons/iot_drivers/static/src/app/components/footer_buttons.js` (36 lines)
- `addons/iot_drivers/static/src/app/components/loading_full_screen.js` (41 lines)
- `addons/iot_drivers/static/src/app/components/single_data.js` (45 lines)
- `addons/iot_drivers/static/src/app/css/homepage.css` (103 lines)
- `addons/iot_drivers/static/src/app/css/icons.css` (45 lines)
- `addons/iot_drivers/static/src/app/css/logs.css` (11 lines)
- `addons/iot_drivers/static/src/app/css/status_display.css` (55 lines)
- `addons/iot_drivers/static/src/app/homepage.js` (187 lines)
- `addons/iot_drivers/static/src/app/hooks/store_hook.js` (9 lines)
- `addons/iot_drivers/static/src/app/logs.js` (40 lines)
- `addons/iot_drivers/static/src/app/main.js` (11 lines)
- `addons/iot_drivers/static/src/app/status.js` (176 lines)
- `addons/iot_drivers/static/src/app/store.js` (32 lines)
- `addons/iot_drivers/tools/__init__.py` (5 lines)
- `addons/iot_drivers/tools/certificate.py` (146 lines)
- `addons/iot_drivers/tools/communication.py` (98 lines)
- `addons/iot_drivers/tools/helpers.py` (429 lines)
- `addons/iot_drivers/tools/route.py` (31 lines)
- `addons/iot_drivers/tools/system.py` (326 lines)
- `addons/iot_drivers/tools/upgrade.py` (152 lines)
- `addons/iot_drivers/tools/wifi.py` (331 lines)
- `addons/iot_drivers/views/index.html` (35 lines)
- `addons/iot_drivers/views/logs.html` (16 lines)
- `addons/iot_drivers/views/status_display.html` (19 lines)
- `addons/iot_drivers/websocket_client.py` (124 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
