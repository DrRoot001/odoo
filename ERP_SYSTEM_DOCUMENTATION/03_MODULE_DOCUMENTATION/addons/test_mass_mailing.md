# Module: test_mass_mailing

- **Module ID:** MOD-578
- **Path:** `addons/test_mass_mailing`
- **Manifest:** `addons/test_mass_mailing/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Mass Mail Tests: feature and performance tests for mass mailing

This module contains tests related to mass mailing. Those
are present in a separate module to use specific test models defined in
test_mail. 

Declared dependencies: `mail_tracking_mass_mailing`, `mass_mailing`, `mass_mailing_sms`, `sms_twilio`, `test_mail`, `test_mail_sms`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 26 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 18 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mail_tracking_mass_mailing",
    "mass_mailing",
    "mass_mailing_sms",
    "sms_twilio",
    "test_mail",
    "test_mail_sms"
  ],
  "data": [
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/test_mass_mailing/__init__.py` (5 lines)
- `addons/test_mass_mailing/__manifest__.py` (23 lines)
- `addons/test_mass_mailing/data/__init__.py` (4 lines)
- `addons/test_mass_mailing/data/mail_test_data.py` (42 lines)
- `addons/test_mass_mailing/models/__init__.py` (6 lines)
- `addons/test_mass_mailing/models/ir_qweb.py` (11 lines)
- `addons/test_mass_mailing/models/mailing_models.py` (129 lines)
- `addons/test_mass_mailing/models/mailing_models_cornercase.py` (32 lines)
- `addons/test_mass_mailing/security/ir.access.csv` (10 lines)
- `addons/test_mass_mailing/tests/__init__.py` (19 lines)
- `addons/test_mass_mailing/tests/common.py` (196 lines)
- `addons/test_mass_mailing/tests/test_blacklist.py` (165 lines)
- `addons/test_mass_mailing/tests/test_blacklist_behavior.py` (94 lines)
- `addons/test_mass_mailing/tests/test_blacklist_mixin.py` (71 lines)
- `addons/test_mass_mailing/tests/test_link_tracker.py` (61 lines)
- `addons/test_mass_mailing/tests/test_link_tracker_sms.py` (119 lines)
- `addons/test_mass_mailing/tests/test_mail_composer.py` (37 lines)
- `addons/test_mass_mailing/tests/test_mail_message.py` (73 lines)
- `addons/test_mass_mailing/tests/test_mailing.py` (730 lines)
- `addons/test_mass_mailing/tests/test_mailing_list.py` (336 lines)
- `addons/test_mass_mailing/tests/test_mailing_server.py` (119 lines)
- `addons/test_mass_mailing/tests/test_mailing_sms.py` (538 lines)
- `addons/test_mass_mailing/tests/test_mailing_statistics.py` (150 lines)
- `addons/test_mass_mailing/tests/test_mailing_statistics_sms.py` (102 lines)
- `addons/test_mass_mailing/tests/test_mailing_test.py` (235 lines)
- `addons/test_mass_mailing/tests/test_performance.py` (105 lines)
- `addons/test_mass_mailing/tests/test_sms_controller.py` (62 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
