# Module: payment_custom

- **Module ID:** MOD-398
- **Path:** `addons/payment_custom`
- **Manifest:** `addons/payment_custom/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

A payment provider for custom flows like wire transfers.

 

Declared dependencies: `payment`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "payment"
  ],
  "data": [
    "views/payment_custom_templates.xml",
    "views/payment_provider_views.xml",
    "data/payment_method_data.xml",
    "data/payment_provider_data.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "payment_custom/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/payment_custom/README.md` (29 lines)
- `addons/payment_custom/__init__.py` (14 lines)
- `addons/payment_custom/__manifest__.py` (22 lines)
- `addons/payment_custom/const.py` (7 lines)
- `addons/payment_custom/controllers/__init__.py` (3 lines)
- `addons/payment_custom/controllers/main.py` (26 lines)
- `addons/payment_custom/data/payment_method_data.xml` (25 lines)
- `addons/payment_custom/data/payment_provider_data.xml` (25 lines)
- `addons/payment_custom/i18n/af.po` (165 lines)
- `addons/payment_custom/i18n/ar.po` (165 lines)
- `addons/payment_custom/i18n/az.po` (167 lines)
- `addons/payment_custom/i18n/bg.po` (167 lines)
- `addons/payment_custom/i18n/bs.po` (168 lines)
- `addons/payment_custom/i18n/ca.po` (168 lines)
- `addons/payment_custom/i18n/cs.po` (163 lines)
- `addons/payment_custom/i18n/da.po` (166 lines)
- `addons/payment_custom/i18n/de.po` (172 lines)
- `addons/payment_custom/i18n/el.po` (165 lines)
- `addons/payment_custom/i18n/es.po` (166 lines)
- `addons/payment_custom/i18n/es_419.po` (169 lines)
- `addons/payment_custom/i18n/es_CL.po` (24 lines)
- `addons/payment_custom/i18n/et.po` (175 lines)
- `addons/payment_custom/i18n/fa.po` (178 lines)
- `addons/payment_custom/i18n/fi.po` (169 lines)
- `addons/payment_custom/i18n/fo.po` (164 lines)
- `addons/payment_custom/i18n/fr.po` (164 lines)
- `addons/payment_custom/i18n/fr_BE.po` (24 lines)
- `addons/payment_custom/i18n/gl.po` (164 lines)
- `addons/payment_custom/i18n/gu.po` (165 lines)
- `addons/payment_custom/i18n/he.po` (174 lines)
- `addons/payment_custom/i18n/hi.po` (169 lines)
- `addons/payment_custom/i18n/hr.po` (166 lines)
- `addons/payment_custom/i18n/hu.po` (167 lines)
- `addons/payment_custom/i18n/hy.po` (164 lines)
- `addons/payment_custom/i18n/id.po` (163 lines)
- `addons/payment_custom/i18n/is.po` (166 lines)
- `addons/payment_custom/i18n/it.po` (167 lines)
- `addons/payment_custom/i18n/ja.po` (165 lines)
- `addons/payment_custom/i18n/ka.po` (164 lines)
- `addons/payment_custom/i18n/kab.po` (163 lines)
- `addons/payment_custom/i18n/km.po` (165 lines)
- `addons/payment_custom/i18n/ko.po` (162 lines)
- `addons/payment_custom/i18n/ku.po` (164 lines)
- `addons/payment_custom/i18n/lo.po` (163 lines)
- `addons/payment_custom/i18n/lt.po` (166 lines)
- `addons/payment_custom/i18n/lv.po` (171 lines)
- `addons/payment_custom/i18n/mk.po` (166 lines)
- `addons/payment_custom/i18n/mn.po` (168 lines)
- `addons/payment_custom/i18n/my.po` (166 lines)
- `addons/payment_custom/i18n/nb.po` (162 lines)
- `addons/payment_custom/i18n/nl.po` (168 lines)
- `addons/payment_custom/i18n/payment_custom.pot` (155 lines)
- `addons/payment_custom/i18n/pl.po` (167 lines)
- `addons/payment_custom/i18n/pt.po` (169 lines)
- `addons/payment_custom/i18n/pt_BR.po` (170 lines)
- `addons/payment_custom/i18n/ro.po` (162 lines)
- `addons/payment_custom/i18n/ru.po` (165 lines)
- `addons/payment_custom/i18n/sk.po` (178 lines)
- `addons/payment_custom/i18n/sl.po` (160 lines)
- `addons/payment_custom/i18n/sr@latin.po` (170 lines)
- `addons/payment_custom/i18n/sv.po` (168 lines)
- `addons/payment_custom/i18n/te.po` (164 lines)
- `addons/payment_custom/i18n/th.po` (163 lines)
- `addons/payment_custom/i18n/tr.po` (169 lines)
- `addons/payment_custom/i18n/uk.po` (180 lines)
- `addons/payment_custom/i18n/uz.po` (182 lines)
- `addons/payment_custom/i18n/vi.po` (163 lines)
- `addons/payment_custom/i18n/zh_CN.po` (166 lines)
- `addons/payment_custom/i18n/zh_TW.po` (164 lines)
- `addons/payment_custom/models/__init__.py` (3 lines)
- `addons/payment_custom/models/payment_provider.py` (93 lines)
- `addons/payment_custom/models/payment_transaction.py` (126 lines)
- `addons/payment_custom/static/description/icon.png` (13 lines)
- `addons/payment_custom/static/description/icon.svg` (1 lines)
- `addons/payment_custom/static/description/icon_hi.png` (71 lines)
- `addons/payment_custom/static/description/icon_invoice.png` (27 lines)
- `addons/payment_custom/static/description/icon_invoice.svg` (13 lines)
- `addons/payment_custom/static/img/pay_on_invoice.png` (17 lines)
- `addons/payment_custom/static/img/wire_transfer.png` (13 lines)
- `addons/payment_custom/static/src/interactions/payment_form.js` (19 lines)
- `addons/payment_custom/static/src/interactions/payment_status.js` (21 lines)
- `addons/payment_custom/tests/__init__.py` (3 lines)
- `addons/payment_custom/tests/common.py` (22 lines)
- `addons/payment_custom/tests/test_payment_transaction.py` (77 lines)
- `addons/payment_custom/tests/test_processing_flows.py` (33 lines)
- `addons/payment_custom/views/payment_custom_templates.xml` (94 lines)
- `addons/payment_custom/views/payment_provider_views.xml` (78 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
