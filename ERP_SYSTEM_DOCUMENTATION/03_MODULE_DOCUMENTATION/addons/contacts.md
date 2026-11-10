# Module: contacts

- **Module ID:** MOD-053
- **Path:** `addons/contacts`
- **Manifest:** `addons/contacts/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Centralize your address book


This module gives you a quick view of your contacts directory, accessible from your home page.
You can track your vendors, customers and other contacts.


Declared dependencies: `base_address_extended`, `mail`, `web_hierarchy`.

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
    "base_address_extended",
    "mail",
    "web_hierarchy"
  ],
  "data": [
    "views/contact_views.xml"
  ],
  "demo": [
    "data/mail_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "contacts/static/src/views/contacts_hierarchy/contacts_hierarchy_card.scss"
    ],
    "web.assets_tests": [
      "contacts/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/contacts/__init__.py` (4 lines)
- `addons/contacts/__manifest__.py` (31 lines)
- `addons/contacts/data/mail_demo.xml` (19 lines)
- `addons/contacts/i18n/af.po` (140 lines)
- `addons/contacts/i18n/ar.po` (150 lines)
- `addons/contacts/i18n/az.po` (147 lines)
- `addons/contacts/i18n/bg.po` (153 lines)
- `addons/contacts/i18n/bs.po` (149 lines)
- `addons/contacts/i18n/ca.po` (152 lines)
- `addons/contacts/i18n/contacts.pot` (139 lines)
- `addons/contacts/i18n/cs.po` (151 lines)
- `addons/contacts/i18n/da.po` (151 lines)
- `addons/contacts/i18n/de.po` (161 lines)
- `addons/contacts/i18n/el.po` (151 lines)
- `addons/contacts/i18n/es.po` (156 lines)
- `addons/contacts/i18n/es_419.po` (157 lines)
- `addons/contacts/i18n/et.po` (151 lines)
- `addons/contacts/i18n/fa.po` (152 lines)
- `addons/contacts/i18n/fi.po` (162 lines)
- `addons/contacts/i18n/fr.po` (159 lines)
- `addons/contacts/i18n/gu.po` (140 lines)
- `addons/contacts/i18n/he.po` (151 lines)
- `addons/contacts/i18n/hi.po` (145 lines)
- `addons/contacts/i18n/hr.po` (153 lines)
- `addons/contacts/i18n/hu.po` (155 lines)
- `addons/contacts/i18n/id.po` (152 lines)
- `addons/contacts/i18n/is.po` (136 lines)
- `addons/contacts/i18n/it.po` (160 lines)
- `addons/contacts/i18n/ja.po` (155 lines)
- `addons/contacts/i18n/kab.po` (145 lines)
- `addons/contacts/i18n/km.po` (139 lines)
- `addons/contacts/i18n/ko.po` (151 lines)
- `addons/contacts/i18n/ku.po` (147 lines)
- `addons/contacts/i18n/lb.po` (141 lines)
- `addons/contacts/i18n/lo.po` (153 lines)
- `addons/contacts/i18n/lt.po` (153 lines)
- `addons/contacts/i18n/lv.po` (151 lines)
- `addons/contacts/i18n/mn.po` (163 lines)
- `addons/contacts/i18n/my.po` (145 lines)
- `addons/contacts/i18n/nb.po` (149 lines)
- `addons/contacts/i18n/nl.po` (151 lines)
- `addons/contacts/i18n/pl.po` (155 lines)
- `addons/contacts/i18n/pt.po` (158 lines)
- `addons/contacts/i18n/pt_BR.po` (162 lines)
- `addons/contacts/i18n/ro.po` (161 lines)
- `addons/contacts/i18n/ru.po` (149 lines)
- `addons/contacts/i18n/sk.po` (149 lines)
- `addons/contacts/i18n/sl.po` (152 lines)
- `addons/contacts/i18n/sr@latin.po` (150 lines)
- `addons/contacts/i18n/sv.po` (156 lines)
- `addons/contacts/i18n/th.po` (151 lines)
- `addons/contacts/i18n/tr.po` (155 lines)
- `addons/contacts/i18n/uk.po` (151 lines)
- `addons/contacts/i18n/uz.po` (170 lines)
- `addons/contacts/i18n/vi.po` (150 lines)
- `addons/contacts/i18n/zh_CN.po` (158 lines)
- `addons/contacts/i18n/zh_TW.po` (148 lines)
- `addons/contacts/models/__init__.py` (5 lines)
- `addons/contacts/models/res_partner.py` (10 lines)
- `addons/contacts/models/res_users.py` (18 lines)
- `addons/contacts/static/description/icon.png` (18 lines)
- `addons/contacts/static/description/icon.svg` (1 lines)
- `addons/contacts/static/description/icon_hi.png` (44 lines)
- `addons/contacts/static/src/views/contacts_hierarchy/contacts_hierarchy_card.scss` (3 lines)
- `addons/contacts/static/tests/tours/debug_menu_set_defaults.js` (87 lines)
- `addons/contacts/tests/__init__.py` (4 lines)
- `addons/contacts/tests/test_ui.py` (37 lines)
- `addons/contacts/views/contact_views.xml` (150 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
