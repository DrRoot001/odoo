# Module: pos_glory_cash

- **Module ID:** MOD-432
- **Path:** `addons/pos_glory_cash`
- **Manifest:** `addons/pos_glory_cash/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Integrate your POS with a Glory automatic cash payment device

No manifest description declared.

Declared dependencies: `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 13 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "point_of_sale"
  ],
  "data": [
    "views/pos_payment_method_views.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "pos_glory_cash/static/src/**/*",
      [
        "remove",
        "pos_glory_cash/static/src/app/**/*"
      ]
    ],
    "point_of_sale.payment_terminals": [
      "pos_glory_cash/static/src/**/*",
      [
        "remove",
        "pos_glory_cash/static/src/backend/**/*"
      ],
      [
        "remove",
        "pos_glory_cash/static/src/app/screens/**/*"
      ]
    ],
    "point_of_sale._assets_pos": [
      "pos_glory_cash/static/src/**/*",
      [
        "remove",
        "pos_glory_cash/static/src/backend/**/*"
      ]
    ],
    "web.assets_unit_tests": [
      "pos_glory_cash/static/tests/**/*",
      "pos_glory_cash/static/src/utils/*.js"
    ]
  }
}
```

### Representative source files

- `addons/pos_glory_cash/__init__.py` (1 lines)
- `addons/pos_glory_cash/__manifest__.py` (30 lines)
- `addons/pos_glory_cash/data/neutralize.sql` (2 lines)
- `addons/pos_glory_cash/i18n/ar.po` (448 lines)
- `addons/pos_glory_cash/i18n/az.po` (440 lines)
- `addons/pos_glory_cash/i18n/bg.po` (440 lines)
- `addons/pos_glory_cash/i18n/bs.po` (447 lines)
- `addons/pos_glory_cash/i18n/ca.po` (443 lines)
- `addons/pos_glory_cash/i18n/cs.po` (442 lines)
- `addons/pos_glory_cash/i18n/da.po` (441 lines)
- `addons/pos_glory_cash/i18n/de.po` (474 lines)
- `addons/pos_glory_cash/i18n/el.po` (441 lines)
- `addons/pos_glory_cash/i18n/es.po` (469 lines)
- `addons/pos_glory_cash/i18n/es_419.po` (461 lines)
- `addons/pos_glory_cash/i18n/et.po` (442 lines)
- `addons/pos_glory_cash/i18n/fa.po` (440 lines)
- `addons/pos_glory_cash/i18n/fi.po` (455 lines)
- `addons/pos_glory_cash/i18n/fr.po` (463 lines)
- `addons/pos_glory_cash/i18n/he.po` (442 lines)
- `addons/pos_glory_cash/i18n/hi.po` (442 lines)
- `addons/pos_glory_cash/i18n/hr.po` (443 lines)
- `addons/pos_glory_cash/i18n/hu.po` (440 lines)
- `addons/pos_glory_cash/i18n/id.po` (465 lines)
- `addons/pos_glory_cash/i18n/it.po` (456 lines)
- `addons/pos_glory_cash/i18n/ja.po` (455 lines)
- `addons/pos_glory_cash/i18n/kab.po` (444 lines)
- `addons/pos_glory_cash/i18n/ko.po` (445 lines)
- `addons/pos_glory_cash/i18n/ku.po` (440 lines)
- `addons/pos_glory_cash/i18n/lo.po` (448 lines)
- `addons/pos_glory_cash/i18n/lt.po` (442 lines)
- `addons/pos_glory_cash/i18n/lv.po` (446 lines)
- `addons/pos_glory_cash/i18n/mn.po` (441 lines)
- `addons/pos_glory_cash/i18n/my.po` (440 lines)
- `addons/pos_glory_cash/i18n/nb.po` (440 lines)
- `addons/pos_glory_cash/i18n/nl.po` (467 lines)
- `addons/pos_glory_cash/i18n/pl.po` (468 lines)
- `addons/pos_glory_cash/i18n/pos_glory_cash.pot` (435 lines)
- `addons/pos_glory_cash/i18n/pt.po` (442 lines)
- `addons/pos_glory_cash/i18n/pt_BR.po` (473 lines)
- `addons/pos_glory_cash/i18n/ro.po` (464 lines)
- `addons/pos_glory_cash/i18n/ru.po` (460 lines)
- `addons/pos_glory_cash/i18n/sk.po` (445 lines)
- `addons/pos_glory_cash/i18n/sl.po` (442 lines)
- `addons/pos_glory_cash/i18n/sr@latin.po` (441 lines)
- `addons/pos_glory_cash/i18n/sv.po` (442 lines)
- `addons/pos_glory_cash/i18n/th.po` (443 lines)
- `addons/pos_glory_cash/i18n/tr.po` (458 lines)
- `addons/pos_glory_cash/i18n/uk.po` (443 lines)
- `addons/pos_glory_cash/i18n/uz.po` (488 lines)
- `addons/pos_glory_cash/i18n/vi.po` (451 lines)
- `addons/pos_glory_cash/i18n/zh_CN.po` (449 lines)
- `addons/pos_glory_cash/i18n/zh_TW.po` (443 lines)
- `addons/pos_glory_cash/models/__init__.py` (1 lines)
- `addons/pos_glory_cash/models/pos_payment_method.py` (16 lines)
- `addons/pos_glory_cash/static/description/icon.png` (97 lines)
- `addons/pos_glory_cash/static/src/@types/models.ts` (58 lines)
- `addons/pos_glory_cash/static/src/app/components/cancel_dialog.js` (12 lines)
- `addons/pos_glory_cash/static/src/app/components/cancel_dialog.xml` (18 lines)
- `addons/pos_glory_cash/static/src/app/components/glory_error_dialog.js` (14 lines)
- `addons/pos_glory_cash/static/src/app/components/glory_error_dialog.xml` (21 lines)
- `addons/pos_glory_cash/static/src/app/models/pos_payment.js` (11 lines)
- `addons/pos_glory_cash/static/src/app/payment_glory.js` (373 lines)
- `addons/pos_glory_cash/static/src/app/screens/payment_screen/payment_lines/payment_lines.xml` (58 lines)
- `addons/pos_glory_cash/static/src/backend/glory_admin_buttons/glory_admin_buttons.js` (103 lines)
- `addons/pos_glory_cash/static/src/backend/glory_admin_buttons/glory_admin_buttons.xml` (29 lines)
- `addons/pos_glory_cash/static/src/glory_service.js` (562 lines)
- `addons/pos_glory_cash/static/src/utils/constants.js` (175 lines)
- `addons/pos_glory_cash/static/src/utils/glory_xml.js` (133 lines)
- `addons/pos_glory_cash/static/src/utils/socket_io.js` (187 lines)
- `addons/pos_glory_cash/static/tests/glory_service.test.js` (156 lines)
- `addons/pos_glory_cash/static/tests/glory_xml.test.js` (110 lines)
- `addons/pos_glory_cash/static/tests/socket_io.test.js` (211 lines)
- `addons/pos_glory_cash/views/pos_payment_method_views.xml` (25 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
