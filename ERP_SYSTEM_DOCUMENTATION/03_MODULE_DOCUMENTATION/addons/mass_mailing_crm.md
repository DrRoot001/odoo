# Module: mass_mailing_crm

- **Module ID:** MOD-363
- **Path:** `addons/mass_mailing_crm`
- **Manifest:** `addons/mass_mailing_crm/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Add lead / opportunities UTM info on mass mailing

UTM and mass mailing on lead / opportunities

Declared dependencies: `crm`, `mass_mailing`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "crm",
    "mass_mailing"
  ],
  "data": [
    "views/mailing_mailing_views.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "mass_mailing_crm/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/mass_mailing_crm/__init__.py` (4 lines)
- `addons/mass_mailing_crm/__manifest__.py` (20 lines)
- `addons/mass_mailing_crm/i18n/ar.po` (166 lines)
- `addons/mass_mailing_crm/i18n/az.po` (158 lines)
- `addons/mass_mailing_crm/i18n/bg.po` (155 lines)
- `addons/mass_mailing_crm/i18n/bs.po` (158 lines)
- `addons/mass_mailing_crm/i18n/ca.po` (169 lines)
- `addons/mass_mailing_crm/i18n/cs.po` (165 lines)
- `addons/mass_mailing_crm/i18n/da.po` (163 lines)
- `addons/mass_mailing_crm/i18n/de.po` (169 lines)
- `addons/mass_mailing_crm/i18n/el.po` (158 lines)
- `addons/mass_mailing_crm/i18n/es.po` (168 lines)
- `addons/mass_mailing_crm/i18n/es_419.po` (164 lines)
- `addons/mass_mailing_crm/i18n/et.po` (165 lines)
- `addons/mass_mailing_crm/i18n/fa.po` (160 lines)
- `addons/mass_mailing_crm/i18n/fi.po` (168 lines)
- `addons/mass_mailing_crm/i18n/fr.po` (169 lines)
- `addons/mass_mailing_crm/i18n/gu.po` (155 lines)
- `addons/mass_mailing_crm/i18n/he.po` (161 lines)
- `addons/mass_mailing_crm/i18n/hi.po` (155 lines)
- `addons/mass_mailing_crm/i18n/hr.po` (162 lines)
- `addons/mass_mailing_crm/i18n/hu.po` (164 lines)
- `addons/mass_mailing_crm/i18n/id.po` (162 lines)
- `addons/mass_mailing_crm/i18n/is.po` (152 lines)
- `addons/mass_mailing_crm/i18n/it.po` (168 lines)
- `addons/mass_mailing_crm/i18n/ja.po` (167 lines)
- `addons/mass_mailing_crm/i18n/kab.po` (156 lines)
- `addons/mass_mailing_crm/i18n/km.po` (155 lines)
- `addons/mass_mailing_crm/i18n/ko.po` (164 lines)
- `addons/mass_mailing_crm/i18n/ku.po` (155 lines)
- `addons/mass_mailing_crm/i18n/lo.po` (162 lines)
- `addons/mass_mailing_crm/i18n/lt.po` (163 lines)
- `addons/mass_mailing_crm/i18n/lv.po` (156 lines)
- `addons/mass_mailing_crm/i18n/mass_mailing_crm.pot` (151 lines)
- `addons/mass_mailing_crm/i18n/mn.po` (161 lines)
- `addons/mass_mailing_crm/i18n/my.po` (155 lines)
- `addons/mass_mailing_crm/i18n/nb.po` (159 lines)
- `addons/mass_mailing_crm/i18n/nl.po` (169 lines)
- `addons/mass_mailing_crm/i18n/pl.po` (170 lines)
- `addons/mass_mailing_crm/i18n/pt.po` (163 lines)
- `addons/mass_mailing_crm/i18n/pt_BR.po` (170 lines)
- `addons/mass_mailing_crm/i18n/ro.po` (162 lines)
- `addons/mass_mailing_crm/i18n/ru.po` (166 lines)
- `addons/mass_mailing_crm/i18n/sk.po` (161 lines)
- `addons/mass_mailing_crm/i18n/sl.po` (161 lines)
- `addons/mass_mailing_crm/i18n/sr@latin.po` (160 lines)
- `addons/mass_mailing_crm/i18n/sv.po` (162 lines)
- `addons/mass_mailing_crm/i18n/th.po` (165 lines)
- `addons/mass_mailing_crm/i18n/tr.po` (168 lines)
- `addons/mass_mailing_crm/i18n/uk.po` (164 lines)
- `addons/mass_mailing_crm/i18n/uz.po` (184 lines)
- `addons/mass_mailing_crm/i18n/vi.po` (165 lines)
- `addons/mass_mailing_crm/i18n/zh_CN.po` (165 lines)
- `addons/mass_mailing_crm/i18n/zh_TW.po` (162 lines)
- `addons/mass_mailing_crm/models/__init__.py` (6 lines)
- `addons/mass_mailing_crm/models/crm_lead.py` (9 lines)
- `addons/mass_mailing_crm/models/mailing_mailing.py` (85 lines)
- `addons/mass_mailing_crm/models/utm.py` (10 lines)
- `addons/mass_mailing_crm/static/src/components/lead_generation_dropdown/crm_lead_gen_element.js` (33 lines)
- `addons/mass_mailing_crm/views/mailing_mailing_views.xml` (25 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
