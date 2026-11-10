# Module: payment_aps

- **Module ID:** MOD-394
- **Path:** `addons/payment_aps`
- **Manifest:** `addons/payment_aps/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

An Amazon payment provider covering the MENA region.

 

Declared dependencies: `payment`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 2 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "payment"
  ],
  "data": [
    "views/payment_provider_views.xml",
    "data/payment_method_data.xml",
    "data/payment_provider_data.xml"
  ]
}
```

### Representative source files

- `addons/payment_aps/README.md` (34 lines)
- `addons/payment_aps/__init__.py` (12 lines)
- `addons/payment_aps/__manifest__.py` (19 lines)
- `addons/payment_aps/const.py` (8 lines)
- `addons/payment_aps/controllers/__init__.py` (3 lines)
- `addons/payment_aps/controllers/main.py` (61 lines)
- `addons/payment_aps/data/neutralize.sql` (6 lines)
- `addons/payment_aps/data/payment_method_data.xml` (84 lines)
- `addons/payment_aps/data/payment_provider_data.xml` (9 lines)
- `addons/payment_aps/i18n/ar.po` (176 lines)
- `addons/payment_aps/i18n/az.po` (173 lines)
- `addons/payment_aps/i18n/bg.po` (173 lines)
- `addons/payment_aps/i18n/bs.po` (175 lines)
- `addons/payment_aps/i18n/ca.po` (174 lines)
- `addons/payment_aps/i18n/cs.po` (175 lines)
- `addons/payment_aps/i18n/da.po` (175 lines)
- `addons/payment_aps/i18n/de.po` (177 lines)
- `addons/payment_aps/i18n/el.po` (174 lines)
- `addons/payment_aps/i18n/es.po` (181 lines)
- `addons/payment_aps/i18n/es_419.po` (178 lines)
- `addons/payment_aps/i18n/et.po` (173 lines)
- `addons/payment_aps/i18n/fa.po` (173 lines)
- `addons/payment_aps/i18n/fi.po` (175 lines)
- `addons/payment_aps/i18n/fr.po` (177 lines)
- `addons/payment_aps/i18n/he.po` (174 lines)
- `addons/payment_aps/i18n/hi.po` (173 lines)
- `addons/payment_aps/i18n/hr.po` (174 lines)
- `addons/payment_aps/i18n/hu.po` (174 lines)
- `addons/payment_aps/i18n/id.po` (175 lines)
- `addons/payment_aps/i18n/it.po` (177 lines)
- `addons/payment_aps/i18n/ja.po` (175 lines)
- `addons/payment_aps/i18n/kab.po` (174 lines)
- `addons/payment_aps/i18n/ko.po` (175 lines)
- `addons/payment_aps/i18n/ku.po` (173 lines)
- `addons/payment_aps/i18n/lo.po` (174 lines)
- `addons/payment_aps/i18n/lt.po` (175 lines)
- `addons/payment_aps/i18n/lv.po` (174 lines)
- `addons/payment_aps/i18n/mn.po` (173 lines)
- `addons/payment_aps/i18n/my.po` (173 lines)
- `addons/payment_aps/i18n/nb.po` (174 lines)
- `addons/payment_aps/i18n/nl.po` (177 lines)
- `addons/payment_aps/i18n/payment_aps.pot` (171 lines)
- `addons/payment_aps/i18n/pl.po` (179 lines)
- `addons/payment_aps/i18n/pt.po` (175 lines)
- `addons/payment_aps/i18n/pt_BR.po` (178 lines)
- `addons/payment_aps/i18n/ro.po` (176 lines)
- `addons/payment_aps/i18n/ru.po` (178 lines)
- `addons/payment_aps/i18n/sk.po` (173 lines)
- `addons/payment_aps/i18n/sl.po` (175 lines)
- `addons/payment_aps/i18n/sr@latin.po` (174 lines)
- `addons/payment_aps/i18n/sv.po` (178 lines)
- `addons/payment_aps/i18n/th.po` (175 lines)
- `addons/payment_aps/i18n/tr.po` (177 lines)
- `addons/payment_aps/i18n/uk.po` (174 lines)
- `addons/payment_aps/i18n/uz.po` (201 lines)
- `addons/payment_aps/i18n/vi.po` (176 lines)
- `addons/payment_aps/i18n/zh_CN.po` (176 lines)
- `addons/payment_aps/i18n/zh_TW.po` (177 lines)
- `addons/payment_aps/models/__init__.py` (3 lines)
- `addons/payment_aps/models/payment_provider.py` (75 lines)
- `addons/payment_aps/models/payment_transaction.py` (122 lines)
- `addons/payment_aps/static/description/icon.png` (11 lines)
- `addons/payment_aps/static/description/icon.svg` (1 lines)
- `addons/payment_aps/static/description/icon_hi.png` (86 lines)
- `addons/payment_aps/tests/__init__.py` (3 lines)
- `addons/payment_aps/tests/common.py` (50 lines)
- `addons/payment_aps/tests/test_payment_transaction.py` (73 lines)
- `addons/payment_aps/tests/test_processing_flows.py` (82 lines)
- `addons/payment_aps/views/payment_provider_views.xml` (41 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
