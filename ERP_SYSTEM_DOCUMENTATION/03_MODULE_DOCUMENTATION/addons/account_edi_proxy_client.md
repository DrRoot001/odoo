# Module: account_edi_proxy_client

- **Module ID:** MOD-005
- **Path:** `addons/account_edi_proxy_client`
- **Manifest:** `addons/account_edi_proxy_client/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This module adds generic features to register an Odoo DB on the proxy responsible for receiving data (via requests from web-services).
- An edi_proxy_user has a unique identification on a specific proxy type (e.g. l10n_it_edi, peppol) which
allows to identify him when receiving a document addressed to him. It is linked to a specific company on a specific
Odoo database.
- Encryption features allows to decrypt all the user's data when receiving it from the proxy.
- Authentication offers an additionnal level of security to avoid impersonification, in case someone gains to the user's database.
    

Declared dependencies: `account`, `certificate`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account",
    "certificate"
  ],
  "data": [
    "views/account_edi_proxy_user_views.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/account_edi_proxy_client/__init__.py` (4 lines)
- `addons/account_edi_proxy_client/__manifest__.py` (20 lines)
- `addons/account_edi_proxy_client/data/neutralize.sql` (10 lines)
- `addons/account_edi_proxy_client/i18n/account_edi_proxy_client.pot` (230 lines)
- `addons/account_edi_proxy_client/i18n/ar.po` (269 lines)
- `addons/account_edi_proxy_client/i18n/az.po` (241 lines)
- `addons/account_edi_proxy_client/i18n/bg.po` (241 lines)
- `addons/account_edi_proxy_client/i18n/bs.po` (243 lines)
- `addons/account_edi_proxy_client/i18n/ca.po` (248 lines)
- `addons/account_edi_proxy_client/i18n/cs.po` (253 lines)
- `addons/account_edi_proxy_client/i18n/da.po` (259 lines)
- `addons/account_edi_proxy_client/i18n/de.po` (278 lines)
- `addons/account_edi_proxy_client/i18n/el.po` (241 lines)
- `addons/account_edi_proxy_client/i18n/es.po` (273 lines)
- `addons/account_edi_proxy_client/i18n/es_419.po` (271 lines)
- `addons/account_edi_proxy_client/i18n/et.po` (249 lines)
- `addons/account_edi_proxy_client/i18n/fa.po` (248 lines)
- `addons/account_edi_proxy_client/i18n/fi.po` (268 lines)
- `addons/account_edi_proxy_client/i18n/fr.po` (274 lines)
- `addons/account_edi_proxy_client/i18n/he.po` (242 lines)
- `addons/account_edi_proxy_client/i18n/hi.po` (245 lines)
- `addons/account_edi_proxy_client/i18n/hr.po` (243 lines)
- `addons/account_edi_proxy_client/i18n/hu.po` (241 lines)
- `addons/account_edi_proxy_client/i18n/id.po` (260 lines)
- `addons/account_edi_proxy_client/i18n/it.po` (271 lines)
- `addons/account_edi_proxy_client/i18n/ja.po` (267 lines)
- `addons/account_edi_proxy_client/i18n/kab.po` (243 lines)
- `addons/account_edi_proxy_client/i18n/ko.po` (247 lines)
- `addons/account_edi_proxy_client/i18n/ku.po` (243 lines)
- `addons/account_edi_proxy_client/i18n/lo.po` (262 lines)
- `addons/account_edi_proxy_client/i18n/lt.po` (243 lines)
- `addons/account_edi_proxy_client/i18n/lv.po` (243 lines)
- `addons/account_edi_proxy_client/i18n/mn.po` (241 lines)
- `addons/account_edi_proxy_client/i18n/my.po` (243 lines)
- `addons/account_edi_proxy_client/i18n/nb.po` (241 lines)
- `addons/account_edi_proxy_client/i18n/nl.po` (273 lines)
- `addons/account_edi_proxy_client/i18n/pl.po` (271 lines)
- `addons/account_edi_proxy_client/i18n/pt.po` (248 lines)
- `addons/account_edi_proxy_client/i18n/pt_BR.po` (271 lines)
- `addons/account_edi_proxy_client/i18n/ro.po` (260 lines)
- `addons/account_edi_proxy_client/i18n/ru.po` (265 lines)
- `addons/account_edi_proxy_client/i18n/sk.po` (284 lines)
- `addons/account_edi_proxy_client/i18n/sl.po` (250 lines)
- `addons/account_edi_proxy_client/i18n/sr@latin.po` (245 lines)
- `addons/account_edi_proxy_client/i18n/sv.po` (277 lines)
- `addons/account_edi_proxy_client/i18n/th.po` (242 lines)
- `addons/account_edi_proxy_client/i18n/tr.po` (272 lines)
- `addons/account_edi_proxy_client/i18n/uk.po` (273 lines)
- `addons/account_edi_proxy_client/i18n/uz.po` (269 lines)
- `addons/account_edi_proxy_client/i18n/vi.po` (254 lines)
- `addons/account_edi_proxy_client/i18n/zh_CN.po` (257 lines)
- `addons/account_edi_proxy_client/i18n/zh_TW.po` (243 lines)
- `addons/account_edi_proxy_client/models/__init__.py` (2 lines)
- `addons/account_edi_proxy_client/models/account_edi_proxy_auth.py` (74 lines)
- `addons/account_edi_proxy_client/models/account_edi_proxy_user.py` (246 lines)
- `addons/account_edi_proxy_client/models/res_company.py` (9 lines)
- `addons/account_edi_proxy_client/security/ir.access.csv` (4 lines)
- `addons/account_edi_proxy_client/tests/__init__.py` (2 lines)
- `addons/account_edi_proxy_client/tests/test_account_edi_proxy_client.py` (71 lines)
- `addons/account_edi_proxy_client/tests/test_neutralize.py` (30 lines)
- `addons/account_edi_proxy_client/views/account_edi_proxy_user_views.xml` (58 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
