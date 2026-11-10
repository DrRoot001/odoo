# Module: test_mail_sms

- **Module ID:** MOD-577
- **Path:** `addons/test_mail_sms`
- **Manifest:** `addons/test_mail_sms/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

SMS Tests: performances and tests specific to SMS

This module contains tests related to SMS. Those are
present in a separate module as it contains models used only to perform
tests independently to functional aspects of other models. 

Declared dependencies: `mail`, `mail_tracking_sms`, `sms`, `sms_twilio`, `test_base`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 18 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 15 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mail",
    "mail_tracking_sms",
    "sms",
    "sms_twilio",
    "test_base"
  ],
  "data": [
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/test_mail_sms/__init__.py` (4 lines)
- `addons/test_mail_sms/__manifest__.py` (22 lines)
- `addons/test_mail_sms/models/__init__.py` (4 lines)
- `addons/test_mail_sms/models/test_mail_sms_models.py` (164 lines)
- `addons/test_mail_sms/security/ir.access.csv` (8 lines)
- `addons/test_mail_sms/tests/__init__.py` (15 lines)
- `addons/test_mail_sms/tests/common.py` (16 lines)
- `addons/test_mail_sms/tests/test_mail_thread_phone.py` (142 lines)
- `addons/test_mail_sms/tests/test_phone_blacklist.py` (115 lines)
- `addons/test_mail_sms/tests/test_phone_format.py` (103 lines)
- `addons/test_mail_sms/tests/test_sms_composer.py` (719 lines)
- `addons/test_mail_sms/tests/test_sms_controller.py` (98 lines)
- `addons/test_mail_sms/tests/test_sms_management.py` (141 lines)
- `addons/test_mail_sms/tests/test_sms_mixin.py` (115 lines)
- `addons/test_mail_sms/tests/test_sms_performance.py` (140 lines)
- `addons/test_mail_sms/tests/test_sms_post.py` (483 lines)
- `addons/test_mail_sms/tests/test_sms_server_actions.py` (70 lines)
- `addons/test_mail_sms/tests/test_sms_sms.py` (127 lines)
- `addons/test_mail_sms/tests/test_sms_template.py` (92 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
