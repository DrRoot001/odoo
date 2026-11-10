# Module: payment_adyen

- **Module ID:** MOD-393
- **Path:** `addons/payment_adyen`
- **Manifest:** `addons/payment_adyen/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

A Dutch payment provider covering Europe and the US.

 

Declared dependencies: `payment`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 16 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 5 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "payment"
  ],
  "data": [
    "views/payment_adyen_templates.xml",
    "views/payment_form_templates.xml",
    "views/payment_provider_views.xml",
    "data/payment_method_data.xml",
    "data/payment_provider_data.xml",
    "wizards/payment_capture_wizard_views.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "payment_adyen/static/src/interactions/payment_form.js"
    ]
  }
}
```

### Representative source files

- `addons/payment_adyen/README.md` (87 lines)
- `addons/payment_adyen/__init__.py` (12 lines)
- `addons/payment_adyen/__manifest__.py` (24 lines)
- `addons/payment_adyen/const.py` (69 lines)
- `addons/payment_adyen/controllers/__init__.py` (3 lines)
- `addons/payment_adyen/controllers/main.py` (336 lines)
- `addons/payment_adyen/data/neutralize.sql` (5 lines)
- `addons/payment_adyen/data/payment_method_data.xml` (1,241 lines)
- `addons/payment_adyen/data/payment_provider_data.xml` (10 lines)
- `addons/payment_adyen/i18n/ar.po` (637 lines)
- `addons/payment_adyen/i18n/az.po` (621 lines)
- `addons/payment_adyen/i18n/bg.po` (621 lines)
- `addons/payment_adyen/i18n/bs.po` (624 lines)
- `addons/payment_adyen/i18n/ca.po` (635 lines)
- `addons/payment_adyen/i18n/cs.po` (639 lines)
- `addons/payment_adyen/i18n/da.po` (627 lines)
- `addons/payment_adyen/i18n/de.po` (643 lines)
- `addons/payment_adyen/i18n/el.po` (625 lines)
- `addons/payment_adyen/i18n/es.po` (640 lines)
- `addons/payment_adyen/i18n/es_419.po` (637 lines)
- `addons/payment_adyen/i18n/et.po` (626 lines)
- `addons/payment_adyen/i18n/fa.po` (624 lines)
- `addons/payment_adyen/i18n/fi.po` (639 lines)
- `addons/payment_adyen/i18n/fr.po` (641 lines)
- `addons/payment_adyen/i18n/he.po` (627 lines)
- `addons/payment_adyen/i18n/hi.po` (621 lines)
- `addons/payment_adyen/i18n/hr.po` (627 lines)
- `addons/payment_adyen/i18n/hu.po` (626 lines)
- `addons/payment_adyen/i18n/id.po` (638 lines)
- `addons/payment_adyen/i18n/it.po` (644 lines)
- `addons/payment_adyen/i18n/ja.po` (637 lines)
- `addons/payment_adyen/i18n/kab.po` (621 lines)
- `addons/payment_adyen/i18n/ko.po` (635 lines)
- `addons/payment_adyen/i18n/ku.po` (621 lines)
- `addons/payment_adyen/i18n/lo.po` (628 lines)
- `addons/payment_adyen/i18n/lt.po` (628 lines)
- `addons/payment_adyen/i18n/lv.po` (621 lines)
- `addons/payment_adyen/i18n/mn.po` (625 lines)
- `addons/payment_adyen/i18n/my.po` (621 lines)
- `addons/payment_adyen/i18n/nb.po` (625 lines)
- `addons/payment_adyen/i18n/nl.po` (642 lines)
- `addons/payment_adyen/i18n/payment_adyen.pot` (616 lines)
- `addons/payment_adyen/i18n/pl.po` (643 lines)
- `addons/payment_adyen/i18n/pt.po` (633 lines)
- `addons/payment_adyen/i18n/pt_BR.po` (645 lines)
- `addons/payment_adyen/i18n/ro.po` (626 lines)
- `addons/payment_adyen/i18n/ru.po` (637 lines)
- `addons/payment_adyen/i18n/sk.po` (626 lines)
- `addons/payment_adyen/i18n/sl.po` (623 lines)
- `addons/payment_adyen/i18n/sr@latin.po` (622 lines)
- `addons/payment_adyen/i18n/sv.po` (641 lines)
- `addons/payment_adyen/i18n/th.po` (634 lines)
- `addons/payment_adyen/i18n/tr.po` (643 lines)
- `addons/payment_adyen/i18n/uk.po` (628 lines)
- `addons/payment_adyen/i18n/uz.po` (678 lines)
- `addons/payment_adyen/i18n/vi.po` (637 lines)
- `addons/payment_adyen/i18n/zh_CN.po` (635 lines)
- `addons/payment_adyen/i18n/zh_TW.po` (633 lines)
- `addons/payment_adyen/models/__init__.py` (3 lines)
- `addons/payment_adyen/models/payment_provider.py` (181 lines)
- `addons/payment_adyen/models/payment_token.py` (13 lines)
- `addons/payment_adyen/models/payment_transaction.py` (450 lines)
- `addons/payment_adyen/static/description/icon.png` (4 lines)
- `addons/payment_adyen/static/description/icon.svg` (1 lines)
- `addons/payment_adyen/static/description/icon_hi.png` (33 lines)
- `addons/payment_adyen/static/src/interactions/payment_form.js` (284 lines)
- `addons/payment_adyen/tests/__init__.py` (3 lines)
- `addons/payment_adyen/tests/common.py` (49 lines)
- `addons/payment_adyen/tests/test_adyen.py` (576 lines)
- `addons/payment_adyen/tests/test_processing_flows.py` (46 lines)
- `addons/payment_adyen/utils.py` (61 lines)
- `addons/payment_adyen/views/payment_adyen_templates.xml` (8 lines)
- `addons/payment_adyen/views/payment_form_templates.xml` (27 lines)
- `addons/payment_adyen/views/payment_provider_views.xml` (56 lines)
- `addons/payment_adyen/wizards/__init__.py` (3 lines)
- `addons/payment_adyen/wizards/payment_capture_wizard.py` (14 lines)
- `addons/payment_adyen/wizards/payment_capture_wizard_views.xml` (22 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
