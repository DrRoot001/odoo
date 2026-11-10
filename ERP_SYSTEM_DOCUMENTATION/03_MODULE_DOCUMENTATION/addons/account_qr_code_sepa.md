# Module: account_qr_code_sepa

- **Module ID:** MOD-013
- **Path:** `addons/account_qr_code_sepa`
- **Manifest:** `addons/account_qr_code_sepa/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This module adds support for SEPA Credit Transfer QR-code generation.
    

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account"
  ]
}
```

### Representative source files

- `addons/account_qr_code_sepa/__init__.py` (3 lines)
- `addons/account_qr_code_sepa/__manifest__.py` (12 lines)
- `addons/account_qr_code_sepa/i18n/account_qr_code_sepa.pot` (75 lines)
- `addons/account_qr_code_sepa/i18n/ar.po` (84 lines)
- `addons/account_qr_code_sepa/i18n/az.po` (79 lines)
- `addons/account_qr_code_sepa/i18n/bg.po` (79 lines)
- `addons/account_qr_code_sepa/i18n/bs.po` (81 lines)
- `addons/account_qr_code_sepa/i18n/ca.po` (84 lines)
- `addons/account_qr_code_sepa/i18n/cs.po` (82 lines)
- `addons/account_qr_code_sepa/i18n/da.po` (86 lines)
- `addons/account_qr_code_sepa/i18n/de.po` (86 lines)
- `addons/account_qr_code_sepa/i18n/el.po` (80 lines)
- `addons/account_qr_code_sepa/i18n/es.po` (85 lines)
- `addons/account_qr_code_sepa/i18n/es_419.po` (86 lines)
- `addons/account_qr_code_sepa/i18n/et.po` (81 lines)
- `addons/account_qr_code_sepa/i18n/fa.po` (81 lines)
- `addons/account_qr_code_sepa/i18n/fi.po` (84 lines)
- `addons/account_qr_code_sepa/i18n/fr.po` (87 lines)
- `addons/account_qr_code_sepa/i18n/he.po` (80 lines)
- `addons/account_qr_code_sepa/i18n/hi.po` (79 lines)
- `addons/account_qr_code_sepa/i18n/hr.po` (82 lines)
- `addons/account_qr_code_sepa/i18n/hu.po` (80 lines)
- `addons/account_qr_code_sepa/i18n/id.po` (82 lines)
- `addons/account_qr_code_sepa/i18n/it.po` (87 lines)
- `addons/account_qr_code_sepa/i18n/ja.po` (85 lines)
- `addons/account_qr_code_sepa/i18n/kab.po` (80 lines)
- `addons/account_qr_code_sepa/i18n/ko.po` (82 lines)
- `addons/account_qr_code_sepa/i18n/ku.po` (81 lines)
- `addons/account_qr_code_sepa/i18n/lo.po` (78 lines)
- `addons/account_qr_code_sepa/i18n/lt.po` (81 lines)
- `addons/account_qr_code_sepa/i18n/lv.po` (81 lines)
- `addons/account_qr_code_sepa/i18n/mn.po` (79 lines)
- `addons/account_qr_code_sepa/i18n/my.po` (79 lines)
- `addons/account_qr_code_sepa/i18n/nb.po` (79 lines)
- `addons/account_qr_code_sepa/i18n/nl.po` (82 lines)
- `addons/account_qr_code_sepa/i18n/pl.po` (85 lines)
- `addons/account_qr_code_sepa/i18n/pt.po` (83 lines)
- `addons/account_qr_code_sepa/i18n/pt_BR.po` (86 lines)
- `addons/account_qr_code_sepa/i18n/ro.po` (82 lines)
- `addons/account_qr_code_sepa/i18n/ru.po` (84 lines)
- `addons/account_qr_code_sepa/i18n/sk.po` (80 lines)
- `addons/account_qr_code_sepa/i18n/sl.po` (82 lines)
- `addons/account_qr_code_sepa/i18n/sr@latin.po` (81 lines)
- `addons/account_qr_code_sepa/i18n/sv.po` (89 lines)
- `addons/account_qr_code_sepa/i18n/th.po` (80 lines)
- `addons/account_qr_code_sepa/i18n/tr.po` (85 lines)
- `addons/account_qr_code_sepa/i18n/uk.po` (83 lines)
- `addons/account_qr_code_sepa/i18n/uz.po` (95 lines)
- `addons/account_qr_code_sepa/i18n/vi.po` (81 lines)
- `addons/account_qr_code_sepa/i18n/zh_CN.po` (82 lines)
- `addons/account_qr_code_sepa/i18n/zh_TW.po` (81 lines)
- `addons/account_qr_code_sepa/models/__init__.py` (3 lines)
- `addons/account_qr_code_sepa/models/res_bank.py` (80 lines)
- `addons/account_qr_code_sepa/tests/__init__.py` (3 lines)
- `addons/account_qr_code_sepa/tests/test_sepa_qr.py` (139 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
