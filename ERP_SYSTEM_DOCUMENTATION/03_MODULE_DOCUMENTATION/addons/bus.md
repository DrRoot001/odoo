# Module: bus

- **Module ID:** MOD-045
- **Path:** `addons/bus`
- **Manifest:** `addons/bus/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Instant Messaging Bus allow you to send messages to users, in live.

Declared dependencies: `base`, `web`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 41 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 12 | Files under `models/` or `models.py`. |
| Controller-path Python files | 4 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 34 | Client behavior/assets. |
| Tests | 15 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 6 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base",
    "web"
  ],
  "assets": {
    "web.assets_backend": [
      "bus/static/src/*.js",
      "bus/static/src/debug/**/*",
      "bus/static/src/services/**/*.js",
      "bus/static/src/workers/*",
      [
        "remove",
        "bus/static/src/workers/bus_worker_script.js"
      ]
    ],
    "web.assets_frontend": [
      "bus/static/src/*.js",
      "bus/static/src/services/**/*.js",
      [
        "remove",
        "bus/static/src/services/assets_watchdog_plugin.js"
      ],
      [
        "remove",
        "bus/static/src/simple_notification_plugin.js"
      ],
      "bus/static/src/workers/*",
      [
        "remove",
        "bus/static/src/workers/bus_worker_script.js"
      ]
    ],
    "web.assets_unit_tests": [
      "bus/static/tests/**/*"
    ],
    "bus.websocket_worker_assets": [
      "web/static/src/module_loader.js",
      "web/static/src/polyfills/promise.js",
      "bus/static/src/workers/*"
    ]
  }
}
```

### Representative source files

- `addons/bus/__init__.py` (7 lines)
- `addons/bus/__manifest__.py` (35 lines)
- `addons/bus/bus_dispatcher.py` (580 lines)
- `addons/bus/controllers/__init__.py` (5 lines)
- `addons/bus/controllers/home.py` (38 lines)
- `addons/bus/controllers/main.py` (13 lines)
- `addons/bus/controllers/websocket.py` (61 lines)
- `addons/bus/i18n/af.po` (203 lines)
- `addons/bus/i18n/ar.po` (220 lines)
- `addons/bus/i18n/az.po` (206 lines)
- `addons/bus/i18n/bg.po` (208 lines)
- `addons/bus/i18n/bs.po` (208 lines)
- `addons/bus/i18n/bus.pot` (199 lines)
- `addons/bus/i18n/ca.po` (227 lines)
- `addons/bus/i18n/cs.po` (214 lines)
- `addons/bus/i18n/da.po` (213 lines)
- `addons/bus/i18n/de.po` (226 lines)
- `addons/bus/i18n/el.po` (208 lines)
- `addons/bus/i18n/es.po` (223 lines)
- `addons/bus/i18n/es_419.po` (222 lines)
- `addons/bus/i18n/es_CL.po` (65 lines)
- `addons/bus/i18n/et.po` (213 lines)
- `addons/bus/i18n/eu.po` (202 lines)
- `addons/bus/i18n/fa.po` (213 lines)
- `addons/bus/i18n/fi.po` (227 lines)
- `addons/bus/i18n/fo.po` (202 lines)
- `addons/bus/i18n/fr.po` (226 lines)
- `addons/bus/i18n/fr_BE.po` (54 lines)
- `addons/bus/i18n/fr_CA.po` (65 lines)
- `addons/bus/i18n/gl.po` (202 lines)
- `addons/bus/i18n/gu.po` (203 lines)
- `addons/bus/i18n/he.po` (213 lines)
- `addons/bus/i18n/hi.po` (203 lines)
- `addons/bus/i18n/hr.po` (209 lines)
- `addons/bus/i18n/hu.po` (211 lines)
- `addons/bus/i18n/hy.po` (201 lines)
- `addons/bus/i18n/id.po` (224 lines)
- `addons/bus/i18n/is.po` (199 lines)
- `addons/bus/i18n/it.po` (226 lines)
- `addons/bus/i18n/ja.po` (224 lines)
- `addons/bus/i18n/ka.po` (202 lines)
- `addons/bus/i18n/kab.po` (205 lines)
- `addons/bus/i18n/km.po` (203 lines)
- `addons/bus/i18n/ko.po` (220 lines)
- `addons/bus/i18n/ku.po` (203 lines)
- `addons/bus/i18n/lo.po` (205 lines)
- `addons/bus/i18n/lt.po` (214 lines)
- `addons/bus/i18n/lv.po` (211 lines)
- `addons/bus/i18n/mk.po` (202 lines)
- `addons/bus/i18n/ml_IN.po` (202 lines)
- `addons/bus/i18n/mn.po` (207 lines)
- `addons/bus/i18n/my.po` (204 lines)
- `addons/bus/i18n/nb.po` (206 lines)
- `addons/bus/i18n/nl.po` (222 lines)
- `addons/bus/i18n/pl.po` (230 lines)
- `addons/bus/i18n/pt.po` (216 lines)
- `addons/bus/i18n/pt_BR.po` (225 lines)
- `addons/bus/i18n/ro.po` (222 lines)
- `addons/bus/i18n/ru.po` (221 lines)
- `addons/bus/i18n/sk.po` (206 lines)
- `addons/bus/i18n/sl.po` (223 lines)
- `addons/bus/i18n/sq.po` (202 lines)
- `addons/bus/i18n/sr@latin.po` (208 lines)
- `addons/bus/i18n/sv.po` (226 lines)
- `addons/bus/i18n/ta.po` (201 lines)
- `addons/bus/i18n/th.po` (218 lines)
- `addons/bus/i18n/tr.po` (233 lines)
- `addons/bus/i18n/uk.po` (222 lines)
- `addons/bus/i18n/uz.po` (246 lines)
- `addons/bus/i18n/vi.po` (221 lines)
- `addons/bus/i18n/zh_CN.po` (218 lines)
- `addons/bus/i18n/zh_TW.po` (217 lines)
- `addons/bus/models/__init__.py` (13 lines)
- `addons/bus/models/bus.py` (184 lines)
- `addons/bus/models/bus_listener_mixin.py` (25 lines)
- `addons/bus/models/ir_attachment.py` (11 lines)
- `addons/bus/models/ir_http.py` (28 lines)
- `addons/bus/models/ir_model.py` (36 lines)
- `addons/bus/models/ir_qweb.py` (11 lines)
- `addons/bus/models/ir_websocket.py` (108 lines)
- `addons/bus/models/res_groups.py` (8 lines)
- `addons/bus/models/res_partner.py` (12 lines)
- `addons/bus/models/res_users.py` (8 lines)
- `addons/bus/models/res_users_settings.py` (11 lines)
- `addons/bus/session_helpers.py` (141 lines)
- `addons/bus/static/src/@types/services.d.ts` (15 lines)
- `addons/bus/static/src/bus_parameters_plugin.js` (28 lines)
- `addons/bus/static/src/debug/bus_logs_menu_item.js` (49 lines)
- `addons/bus/static/src/debug/bus_logs_menu_item.xml` (15 lines)
- `addons/bus/static/src/debug/bus_logs_plugin.js` (71 lines)
- `addons/bus/static/src/misc.js` (63 lines)
- `addons/bus/static/src/multi_tab_fallback_plugin.js` (191 lines)
- `addons/bus/static/src/multi_tab_plugin.js` (25 lines)
- `addons/bus/static/src/multi_tab_shared_worker_plugin.js` (87 lines)
- `addons/bus/static/src/services/assets_watchdog_plugin.js` (88 lines)
- `addons/bus/static/src/services/bus_monitoring_plugin.js` (63 lines)
- `addons/bus/static/src/services/bus_plugin.js` (282 lines)
- `addons/bus/static/src/services/presence_plugin.js` (92 lines)
- `addons/bus/static/src/services/worker_plugin.js` (167 lines)
- `addons/bus/static/src/simple_notification_plugin.js` (23 lines)
- `addons/bus/static/src/workers/base_worker.js` (17 lines)
- `addons/bus/static/src/workers/bus_worker_script.js` (33 lines)
- `addons/bus/static/src/workers/bus_worker_utils.js` (199 lines)
- `addons/bus/static/src/workers/election_worker.js` (103 lines)
- `addons/bus/static/src/workers/websocket_worker.js` (627 lines)
- `addons/bus/static/tests/assets_watchdog.test.js` (23 lines)
- `addons/bus/static/tests/bus_logger.test.js` (64 lines)
- `addons/bus/static/tests/bus_monitoring_plugin.test.js` (88 lines)
- `addons/bus/static/tests/bus_plugin.test.js` (613 lines)
- `addons/bus/static/tests/bus_test_helpers.js` (342 lines)
- `addons/bus/static/tests/mock_base_worker.js` (23 lines)
- `addons/bus/static/tests/mock_election_worker.js` (16 lines)
- `addons/bus/static/tests/mock_server/mock_models/@types/mock_models.d.ts` (12 lines)
- `addons/bus/static/tests/mock_server/mock_models/bus_bus.js` (78 lines)
- `addons/bus/static/tests/mock_server/mock_models/ir_websocket.js` (32 lines)
- `addons/bus/static/tests/mock_websocket.js` (125 lines)
- `addons/bus/static/tests/multi_tab_fallback_plugin.test.js` (38 lines)
- `addons/bus/static/tests/multi_tab_shared_worker_plugin.test.js` (66 lines)
- `addons/bus/static/tests/simple_notification.test.js` (48 lines)
- `addons/bus/static/tests/websocket_worker.test.js` (215 lines)
- `addons/bus/tests/__init__.py` (16 lines)
- `addons/bus/tests/common.py` (447 lines)
- `addons/bus/tests/test_assetsbundle.py` (45 lines)
- `addons/bus/tests/test_bus_gc.py` (36 lines)
- `addons/bus/tests/test_close_websocket_after_tour.py` (51 lines)
- `addons/bus/tests/test_health.py` (13 lines)
- `addons/bus/tests/test_ir_model.py` (46 lines)
- `addons/bus/tests/test_ir_websocket.py` (38 lines)
- `addons/bus/tests/test_notify.py` (154 lines)
- `addons/bus/tests/test_websocket_caryall.py` (352 lines)
- `addons/bus/tests/test_websocket_check_session.py` (221 lines)
- `addons/bus/tests/test_websocket_controller.py` (99 lines)
- `addons/bus/tests/test_websocket_dispatching.py` (75 lines)
- `addons/bus/tests/test_websocket_rate_limiting.py` (88 lines)
- `addons/bus/tests/test_websocket_timeouts.py` (95 lines)
- `addons/bus/tools/__init__.py` (3 lines)
- `addons/bus/tools/misc.py` (44 lines)
- `addons/bus/tools/notifications.py` (57 lines)
- `addons/bus/tools/orjson.py` (16 lines)
- `addons/bus/websocket.py` (1,018 lines)
- `addons/bus/websocket_protocol.py` (84 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
