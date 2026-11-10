# Module: crm_iap_enrich

- **Module ID:** MOD-055
- **Path:** `addons/crm_iap_enrich`
- **Manifest:** `addons/crm_iap_enrich/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Enrich Leads/Opportunities using email address domain

No manifest description declared.

Declared dependencies: `iap_crm`, `iap_mail`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "iap_crm",
    "iap_mail"
  ],
  "data": [
    "data/ir_cron.xml",
    "data/ir_action.xml",
    "data/mail_templates.xml",
    "views/crm_lead_views.xml",
    "views/res_config_settings_view.xml"
  ]
}
```

### Representative source files

- `addons/crm_iap_enrich/__init__.py` (11 lines)
- `addons/crm_iap_enrich/__manifest__.py` (24 lines)
- `addons/crm_iap_enrich/data/ir_action.xml` (16 lines)
- `addons/crm_iap_enrich/data/ir_cron.xml` (13 lines)
- `addons/crm_iap_enrich/data/mail_templates.xml` (18 lines)
- `addons/crm_iap_enrich/i18n/ar.po` (151 lines)
- `addons/crm_iap_enrich/i18n/az.po` (139 lines)
- `addons/crm_iap_enrich/i18n/bg.po` (139 lines)
- `addons/crm_iap_enrich/i18n/bs.po` (141 lines)
- `addons/crm_iap_enrich/i18n/ca.po` (148 lines)
- `addons/crm_iap_enrich/i18n/crm_iap_enrich.pot` (135 lines)
- `addons/crm_iap_enrich/i18n/cs.po` (151 lines)
- `addons/crm_iap_enrich/i18n/da.po` (150 lines)
- `addons/crm_iap_enrich/i18n/de.po` (153 lines)
- `addons/crm_iap_enrich/i18n/el.po` (140 lines)
- `addons/crm_iap_enrich/i18n/es.po` (152 lines)
- `addons/crm_iap_enrich/i18n/es_419.po` (148 lines)
- `addons/crm_iap_enrich/i18n/et.po` (144 lines)
- `addons/crm_iap_enrich/i18n/fa.po` (144 lines)
- `addons/crm_iap_enrich/i18n/fi.po` (147 lines)
- `addons/crm_iap_enrich/i18n/fr.po` (153 lines)
- `addons/crm_iap_enrich/i18n/he.po` (149 lines)
- `addons/crm_iap_enrich/i18n/hi.po` (141 lines)
- `addons/crm_iap_enrich/i18n/hr.po` (144 lines)
- `addons/crm_iap_enrich/i18n/hu.po` (143 lines)
- `addons/crm_iap_enrich/i18n/id.po` (148 lines)
- `addons/crm_iap_enrich/i18n/it.po` (151 lines)
- `addons/crm_iap_enrich/i18n/ja.po` (145 lines)
- `addons/crm_iap_enrich/i18n/kab.po` (140 lines)
- `addons/crm_iap_enrich/i18n/ko.po` (145 lines)
- `addons/crm_iap_enrich/i18n/ku.po` (139 lines)
- `addons/crm_iap_enrich/i18n/lo.po` (143 lines)
- `addons/crm_iap_enrich/i18n/lt.po` (145 lines)
- `addons/crm_iap_enrich/i18n/lv.po` (141 lines)
- `addons/crm_iap_enrich/i18n/mn.po` (142 lines)
- `addons/crm_iap_enrich/i18n/my.po` (139 lines)
- `addons/crm_iap_enrich/i18n/nb.po` (141 lines)
- `addons/crm_iap_enrich/i18n/nl.po` (150 lines)
- `addons/crm_iap_enrich/i18n/pl.po` (152 lines)
- `addons/crm_iap_enrich/i18n/pt.po` (152 lines)
- `addons/crm_iap_enrich/i18n/pt_BR.po` (152 lines)
- `addons/crm_iap_enrich/i18n/ro.po` (152 lines)
- `addons/crm_iap_enrich/i18n/ru.po` (150 lines)
- `addons/crm_iap_enrich/i18n/sk.po` (140 lines)
- `addons/crm_iap_enrich/i18n/sl.po` (148 lines)
- `addons/crm_iap_enrich/i18n/sr@latin.po` (140 lines)
- `addons/crm_iap_enrich/i18n/sv.po` (148 lines)
- `addons/crm_iap_enrich/i18n/th.po` (143 lines)
- `addons/crm_iap_enrich/i18n/tr.po` (150 lines)
- `addons/crm_iap_enrich/i18n/uk.po` (152 lines)
- `addons/crm_iap_enrich/i18n/uz.po` (172 lines)
- `addons/crm_iap_enrich/i18n/vi.po` (148 lines)
- `addons/crm_iap_enrich/i18n/zh_CN.po` (146 lines)
- `addons/crm_iap_enrich/i18n/zh_TW.po` (144 lines)
- `addons/crm_iap_enrich/models/__init__.py` (5 lines)
- `addons/crm_iap_enrich/models/crm_lead.py` (213 lines)
- `addons/crm_iap_enrich/models/res_config_settings.py` (21 lines)
- `addons/crm_iap_enrich/tests/__init__.py` (5 lines)
- `addons/crm_iap_enrich/tests/test_crm_lead_merge.py` (27 lines)
- `addons/crm_iap_enrich/tests/test_lead_enrich.py` (61 lines)
- `addons/crm_iap_enrich/views/crm_lead_views.xml` (20 lines)
- `addons/crm_iap_enrich/views/res_config_settings_view.xml` (15 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
