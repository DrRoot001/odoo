# Module: snailmail_account

- **Module ID:** MOD-542
- **Path:** `addons/snailmail_account`
- **Manifest:** `addons/snailmail_account/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Allows users to send invoices by post
=====================================================
        

Declared dependencies: `account`, `snailmail`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 13 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account",
    "snailmail"
  ],
  "data": [
    "views/res_config_settings_views.xml"
  ]
}
```

### Representative source files

- `addons/snailmail_account/__init__.py` (3 lines)
- `addons/snailmail_account/__manifest__.py` (16 lines)
- `addons/snailmail_account/controllers/__init__.py` (1 lines)
- `addons/snailmail_account/controllers/portal.py` (13 lines)
- `addons/snailmail_account/i18n/ar.po` (138 lines)
- `addons/snailmail_account/i18n/az.po` (129 lines)
- `addons/snailmail_account/i18n/bg.po` (127 lines)
- `addons/snailmail_account/i18n/bs.po` (129 lines)
- `addons/snailmail_account/i18n/ca.po` (138 lines)
- `addons/snailmail_account/i18n/cs.po` (135 lines)
- `addons/snailmail_account/i18n/da.po` (132 lines)
- `addons/snailmail_account/i18n/de.po` (137 lines)
- `addons/snailmail_account/i18n/el.po` (129 lines)
- `addons/snailmail_account/i18n/es.po` (138 lines)
- `addons/snailmail_account/i18n/es_419.po` (131 lines)
- `addons/snailmail_account/i18n/et.po` (136 lines)
- `addons/snailmail_account/i18n/fa.po` (136 lines)
- `addons/snailmail_account/i18n/fi.po` (138 lines)
- `addons/snailmail_account/i18n/fr.po` (135 lines)
- `addons/snailmail_account/i18n/gu.po` (127 lines)
- `addons/snailmail_account/i18n/he.po` (136 lines)
- `addons/snailmail_account/i18n/hi.po` (125 lines)
- `addons/snailmail_account/i18n/hr.po` (132 lines)
- `addons/snailmail_account/i18n/hu.po` (137 lines)
- `addons/snailmail_account/i18n/id.po` (131 lines)
- `addons/snailmail_account/i18n/is.po` (121 lines)
- `addons/snailmail_account/i18n/it.po` (134 lines)
- `addons/snailmail_account/i18n/ja.po` (134 lines)
- `addons/snailmail_account/i18n/kab.po` (125 lines)
- `addons/snailmail_account/i18n/km.po` (126 lines)
- `addons/snailmail_account/i18n/ko.po` (134 lines)
- `addons/snailmail_account/i18n/ku.po` (125 lines)
- `addons/snailmail_account/i18n/lo.po` (124 lines)
- `addons/snailmail_account/i18n/lt.po` (136 lines)
- `addons/snailmail_account/i18n/lv.po` (125 lines)
- `addons/snailmail_account/i18n/mn.po` (134 lines)
- `addons/snailmail_account/i18n/my.po` (125 lines)
- `addons/snailmail_account/i18n/nb.po` (132 lines)
- `addons/snailmail_account/i18n/nl.po` (139 lines)
- `addons/snailmail_account/i18n/pl.po` (144 lines)
- `addons/snailmail_account/i18n/pt.po` (137 lines)
- `addons/snailmail_account/i18n/pt_BR.po` (138 lines)
- `addons/snailmail_account/i18n/ro.po` (134 lines)
- `addons/snailmail_account/i18n/ru.po` (134 lines)
- `addons/snailmail_account/i18n/sk.po` (131 lines)
- `addons/snailmail_account/i18n/sl.po` (129 lines)
- `addons/snailmail_account/i18n/snailmail_account.pot` (121 lines)
- `addons/snailmail_account/i18n/sr@latin.po` (132 lines)
- `addons/snailmail_account/i18n/sv.po` (131 lines)
- `addons/snailmail_account/i18n/th.po` (133 lines)
- `addons/snailmail_account/i18n/tr.po` (143 lines)
- `addons/snailmail_account/i18n/uk.po` (135 lines)
- `addons/snailmail_account/i18n/uz.po` (146 lines)
- `addons/snailmail_account/i18n/vi.po` (133 lines)
- `addons/snailmail_account/i18n/zh_CN.po` (133 lines)
- `addons/snailmail_account/i18n/zh_TW.po` (131 lines)
- `addons/snailmail_account/models/__init__.py` (3 lines)
- `addons/snailmail_account/models/account_move.py` (13 lines)
- `addons/snailmail_account/models/account_move_send.py` (67 lines)
- `addons/snailmail_account/models/res_partner.py` (9 lines)
- `addons/snailmail_account/tests/__init__.py` (2 lines)
- `addons/snailmail_account/tests/test_pingen_send.py` (70 lines)
- `addons/snailmail_account/tests/test_snailmail_on_invoice.py` (52 lines)
- `addons/snailmail_account/views/res_config_settings_views.xml` (31 lines)
- `addons/snailmail_account/wizard/__init__.py` (1 lines)
- `addons/snailmail_account/wizard/account_move_send_batch_wizard.py` (21 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
