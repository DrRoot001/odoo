# Module: account_qr_code_emv

- **Module ID:** MOD-012
- **Path:** `addons/account_qr_code_emv`
- **Manifest:** `addons/account_qr_code_emv/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Bridge module addings support for EMV Merchant-Presented QR-code generation for Payment System.
    

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 5 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account"
  ],
  "data": [
    "views/res_bank_views.xml"
  ]
}
```

### Representative source files

- `addons/account_qr_code_emv/__init__.py` (3 lines)
- `addons/account_qr_code_emv/__manifest__.py` (15 lines)
- `addons/account_qr_code_emv/const.py` (53 lines)
- `addons/account_qr_code_emv/i18n/account_qr_code_emv.pot` (155 lines)
- `addons/account_qr_code_emv/i18n/ar.po` (169 lines)
- `addons/account_qr_code_emv/i18n/az.po` (160 lines)
- `addons/account_qr_code_emv/i18n/bg.po` (160 lines)
- `addons/account_qr_code_emv/i18n/bs.po` (162 lines)
- `addons/account_qr_code_emv/i18n/ca.po` (163 lines)
- `addons/account_qr_code_emv/i18n/cs.po` (161 lines)
- `addons/account_qr_code_emv/i18n/da.po` (164 lines)
- `addons/account_qr_code_emv/i18n/de.po` (175 lines)
- `addons/account_qr_code_emv/i18n/el.po` (161 lines)
- `addons/account_qr_code_emv/i18n/es.po` (171 lines)
- `addons/account_qr_code_emv/i18n/es_419.po` (175 lines)
- `addons/account_qr_code_emv/i18n/et.po` (161 lines)
- `addons/account_qr_code_emv/i18n/fa.po` (160 lines)
- `addons/account_qr_code_emv/i18n/fi.po` (172 lines)
- `addons/account_qr_code_emv/i18n/fr.po` (174 lines)
- `addons/account_qr_code_emv/i18n/he.po` (161 lines)
- `addons/account_qr_code_emv/i18n/hi.po` (163 lines)
- `addons/account_qr_code_emv/i18n/hr.po` (161 lines)
- `addons/account_qr_code_emv/i18n/hu.po` (161 lines)
- `addons/account_qr_code_emv/i18n/id.po` (163 lines)
- `addons/account_qr_code_emv/i18n/it.po` (173 lines)
- `addons/account_qr_code_emv/i18n/ja.po` (171 lines)
- `addons/account_qr_code_emv/i18n/kab.po` (161 lines)
- `addons/account_qr_code_emv/i18n/ko.po` (162 lines)
- `addons/account_qr_code_emv/i18n/ku.po` (160 lines)
- `addons/account_qr_code_emv/i18n/lo.po` (159 lines)
- `addons/account_qr_code_emv/i18n/lt.po` (162 lines)
- `addons/account_qr_code_emv/i18n/lv.po` (162 lines)
- `addons/account_qr_code_emv/i18n/mn.po` (160 lines)
- `addons/account_qr_code_emv/i18n/my.po` (160 lines)
- `addons/account_qr_code_emv/i18n/nb.po` (160 lines)
- `addons/account_qr_code_emv/i18n/nl.po` (169 lines)
- `addons/account_qr_code_emv/i18n/pl.po` (166 lines)
- `addons/account_qr_code_emv/i18n/pt.po` (163 lines)
- `addons/account_qr_code_emv/i18n/pt_BR.po` (174 lines)
- `addons/account_qr_code_emv/i18n/ro.po` (162 lines)
- `addons/account_qr_code_emv/i18n/ru.po` (165 lines)
- `addons/account_qr_code_emv/i18n/sk.po` (159 lines)
- `addons/account_qr_code_emv/i18n/sl.po` (163 lines)
- `addons/account_qr_code_emv/i18n/sr@latin.po` (162 lines)
- `addons/account_qr_code_emv/i18n/sv.po` (172 lines)
- `addons/account_qr_code_emv/i18n/th.po` (161 lines)
- `addons/account_qr_code_emv/i18n/tr.po` (172 lines)
- `addons/account_qr_code_emv/i18n/uk.po` (174 lines)
- `addons/account_qr_code_emv/i18n/uz.po` (180 lines)
- `addons/account_qr_code_emv/i18n/vi.po` (161 lines)
- `addons/account_qr_code_emv/i18n/zh_CN.po` (170 lines)
- `addons/account_qr_code_emv/i18n/zh_TW.po` (162 lines)
- `addons/account_qr_code_emv/models/__init__.py` (3 lines)
- `addons/account_qr_code_emv/models/res_bank.py` (162 lines)
- `addons/account_qr_code_emv/views/res_bank_views.xml` (23 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
