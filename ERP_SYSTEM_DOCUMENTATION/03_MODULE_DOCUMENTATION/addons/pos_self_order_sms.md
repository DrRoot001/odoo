# Module: pos_self_order_sms

- **Module ID:** MOD-462
- **Path:** `addons/pos_self_order_sms`
- **Manifest:** `addons/pos_self_order_sms/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Integrates POS Self Order with SMS to send customers order confirmation via SMS.

Declared dependencies: `pos_self_order`, `pos_sms`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "pos_self_order",
    "pos_sms"
  ],
  "data": [
    "data/preset_data.xml",
    "views/pos_preset_views.xml"
  ],
  "assets": {
    "pos_self_order.assets": [
      "pos_self_order_sms/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_self_order_sms/__init__.py` (3 lines)
- `addons/pos_self_order_sms/__manifest__.py` (20 lines)
- `addons/pos_self_order_sms/data/preset_data.xml` (10 lines)
- `addons/pos_self_order_sms/i18n/ar.po` (76 lines)
- `addons/pos_self_order_sms/i18n/az.po` (75 lines)
- `addons/pos_self_order_sms/i18n/bg.po` (75 lines)
- `addons/pos_self_order_sms/i18n/bs.po` (76 lines)
- `addons/pos_self_order_sms/i18n/ca.po` (75 lines)
- `addons/pos_self_order_sms/i18n/cs.po` (75 lines)
- `addons/pos_self_order_sms/i18n/da.po` (75 lines)
- `addons/pos_self_order_sms/i18n/de.po` (80 lines)
- `addons/pos_self_order_sms/i18n/el.po` (75 lines)
- `addons/pos_self_order_sms/i18n/es.po` (80 lines)
- `addons/pos_self_order_sms/i18n/es_419.po` (78 lines)
- `addons/pos_self_order_sms/i18n/et.po` (75 lines)
- `addons/pos_self_order_sms/i18n/fa.po` (75 lines)
- `addons/pos_self_order_sms/i18n/fi.po` (76 lines)
- `addons/pos_self_order_sms/i18n/fr.po` (78 lines)
- `addons/pos_self_order_sms/i18n/he.po` (76 lines)
- `addons/pos_self_order_sms/i18n/hi.po` (75 lines)
- `addons/pos_self_order_sms/i18n/hr.po` (76 lines)
- `addons/pos_self_order_sms/i18n/hu.po` (75 lines)
- `addons/pos_self_order_sms/i18n/id.po` (75 lines)
- `addons/pos_self_order_sms/i18n/it.po` (78 lines)
- `addons/pos_self_order_sms/i18n/ja.po` (75 lines)
- `addons/pos_self_order_sms/i18n/kab.po` (75 lines)
- `addons/pos_self_order_sms/i18n/ko.po` (75 lines)
- `addons/pos_self_order_sms/i18n/ku.po` (75 lines)
- `addons/pos_self_order_sms/i18n/lo.po` (75 lines)
- `addons/pos_self_order_sms/i18n/lt.po` (77 lines)
- `addons/pos_self_order_sms/i18n/lv.po` (76 lines)
- `addons/pos_self_order_sms/i18n/mn.po` (75 lines)
- `addons/pos_self_order_sms/i18n/my.po` (75 lines)
- `addons/pos_self_order_sms/i18n/nb.po` (75 lines)
- `addons/pos_self_order_sms/i18n/nl.po` (78 lines)
- `addons/pos_self_order_sms/i18n/pl.po` (76 lines)
- `addons/pos_self_order_sms/i18n/pos_self_order_sms.pot` (72 lines)
- `addons/pos_self_order_sms/i18n/pt.po` (75 lines)
- `addons/pos_self_order_sms/i18n/pt_BR.po` (81 lines)
- `addons/pos_self_order_sms/i18n/ro.po` (76 lines)
- `addons/pos_self_order_sms/i18n/ru.po` (76 lines)
- `addons/pos_self_order_sms/i18n/sk.po` (75 lines)
- `addons/pos_self_order_sms/i18n/sl.po` (76 lines)
- `addons/pos_self_order_sms/i18n/sr@latin.po` (76 lines)
- `addons/pos_self_order_sms/i18n/sv.po` (76 lines)
- `addons/pos_self_order_sms/i18n/th.po` (75 lines)
- `addons/pos_self_order_sms/i18n/tr.po` (75 lines)
- `addons/pos_self_order_sms/i18n/uk.po` (76 lines)
- `addons/pos_self_order_sms/i18n/uz.po` (75 lines)
- `addons/pos_self_order_sms/i18n/vi.po` (75 lines)
- `addons/pos_self_order_sms/i18n/zh_CN.po` (77 lines)
- `addons/pos_self_order_sms/i18n/zh_TW.po` (75 lines)
- `addons/pos_self_order_sms/models/__init__.py` (4 lines)
- `addons/pos_self_order_sms/models/pos_order.py` (21 lines)
- `addons/pos_self_order_sms/models/pos_preset.py` (18 lines)
- `addons/pos_self_order_sms/static/src/app/models/pos_preset.js` (11 lines)
- `addons/pos_self_order_sms/tests/__init__.py` (3 lines)
- `addons/pos_self_order_sms/tests/test_self_order_sms_receipt.py` (49 lines)
- `addons/pos_self_order_sms/views/pos_preset_views.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
