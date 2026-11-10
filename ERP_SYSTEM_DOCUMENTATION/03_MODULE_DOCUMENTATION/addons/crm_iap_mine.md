# Module: crm_iap_mine

- **Module ID:** MOD-056
- **Path:** `addons/crm_iap_mine`
- **Manifest:** `addons/crm_iap_mine/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Generate Leads/Opportunities based on country, industries, size, etc.

No manifest description declared.

Declared dependencies: `iap_crm`, `iap_mail`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 13 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 8 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 7 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
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
    "data/crm.iap.lead.industry.division.csv",
    "data/crm.iap.lead.industry.csv",
    "data/crm.iap.lead.role.csv",
    "data/crm.iap.lead.seniority.csv",
    "data/mail_template_data.xml",
    "data/ir_sequence_data.xml",
    "views/crm_iap_lead_industry_views.xml",
    "views/crm_iap_lead_mining_request_views.xml",
    "views/res_config_settings_views.xml",
    "views/mail_templates.xml",
    "views/crm_menus.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "crm_iap_mine/static/src/js/**/*",
      "crm_iap_mine/static/src/components/**/*"
    ]
  }
}
```

### Representative source files

- `addons/crm_iap_mine/__init__.py` (4 lines)
- `addons/crm_iap_mine/__manifest__.py` (36 lines)
- `addons/crm_iap_mine/data/crm.iap.lead.industry.csv` (84 lines)
- `addons/crm_iap_mine/data/crm.iap.lead.industry.division.csv` (11 lines)
- `addons/crm_iap_mine/data/crm.iap.lead.role.csv` (23 lines)
- `addons/crm_iap_mine/data/crm.iap.lead.seniority.csv` (4 lines)
- `addons/crm_iap_mine/data/ir_sequence_data.xml` (14 lines)
- `addons/crm_iap_mine/data/mail_template_data.xml` (21 lines)
- `addons/crm_iap_mine/i18n/ar.po` (1,182 lines)
- `addons/crm_iap_mine/i18n/az.po` (1,174 lines)
- `addons/crm_iap_mine/i18n/bg.po` (1,157 lines)
- `addons/crm_iap_mine/i18n/bs.po` (1,154 lines)
- `addons/crm_iap_mine/i18n/ca.po` (1,182 lines)
- `addons/crm_iap_mine/i18n/crm_iap_mine.pot` (1,148 lines)
- `addons/crm_iap_mine/i18n/cs.po` (1,187 lines)
- `addons/crm_iap_mine/i18n/da.po` (1,188 lines)
- `addons/crm_iap_mine/i18n/de.po` (1,199 lines)
- `addons/crm_iap_mine/i18n/el.po` (1,154 lines)
- `addons/crm_iap_mine/i18n/es.po` (1,186 lines)
- `addons/crm_iap_mine/i18n/es_419.po` (1,193 lines)
- `addons/crm_iap_mine/i18n/et.po` (1,179 lines)
- `addons/crm_iap_mine/i18n/fa.po` (1,157 lines)
- `addons/crm_iap_mine/i18n/fi.po` (1,181 lines)
- `addons/crm_iap_mine/i18n/fr.po` (1,202 lines)
- `addons/crm_iap_mine/i18n/he.po` (1,187 lines)
- `addons/crm_iap_mine/i18n/hi.po` (1,157 lines)
- `addons/crm_iap_mine/i18n/hr.po` (1,165 lines)
- `addons/crm_iap_mine/i18n/hu.po` (1,161 lines)
- `addons/crm_iap_mine/i18n/id.po` (1,181 lines)
- `addons/crm_iap_mine/i18n/it.po` (1,199 lines)
- `addons/crm_iap_mine/i18n/ja.po` (1,190 lines)
- `addons/crm_iap_mine/i18n/kab.po` (1,153 lines)
- `addons/crm_iap_mine/i18n/ko.po` (1,179 lines)
- `addons/crm_iap_mine/i18n/ku.po` (1,152 lines)
- `addons/crm_iap_mine/i18n/lo.po` (1,184 lines)
- `addons/crm_iap_mine/i18n/lt.po` (1,171 lines)
- `addons/crm_iap_mine/i18n/lv.po` (1,154 lines)
- `addons/crm_iap_mine/i18n/mn.po` (1,163 lines)
- `addons/crm_iap_mine/i18n/my.po` (1,153 lines)
- `addons/crm_iap_mine/i18n/nb.po` (1,159 lines)
- `addons/crm_iap_mine/i18n/nl.po` (1,196 lines)
- `addons/crm_iap_mine/i18n/pl.po` (1,207 lines)
- `addons/crm_iap_mine/i18n/pt.po` (1,169 lines)
- `addons/crm_iap_mine/i18n/pt_BR.po` (1,196 lines)
- `addons/crm_iap_mine/i18n/ro.po` (1,189 lines)
- `addons/crm_iap_mine/i18n/ru.po` (1,195 lines)
- `addons/crm_iap_mine/i18n/sk.po` (1,155 lines)
- `addons/crm_iap_mine/i18n/sl.po` (1,182 lines)
- `addons/crm_iap_mine/i18n/sr@latin.po` (1,155 lines)
- `addons/crm_iap_mine/i18n/sv.po` (1,179 lines)
- `addons/crm_iap_mine/i18n/th.po` (1,178 lines)
- `addons/crm_iap_mine/i18n/tr.po` (1,208 lines)
- `addons/crm_iap_mine/i18n/uk.po` (1,186 lines)
- `addons/crm_iap_mine/i18n/uz.po` (1,281 lines)
- `addons/crm_iap_mine/i18n/vi.po` (1,181 lines)
- `addons/crm_iap_mine/i18n/zh_CN.po` (1,188 lines)
- `addons/crm_iap_mine/i18n/zh_TW.po` (1,179 lines)
- `addons/crm_iap_mine/models/__init__.py` (10 lines)
- `addons/crm_iap_mine/models/crm_iap_lead_helpers.py` (64 lines)
- `addons/crm_iap_mine/models/crm_iap_lead_industry.py` (42 lines)
- `addons/crm_iap_mine/models/crm_iap_lead_industry_division.py` (19 lines)
- `addons/crm_iap_mine/models/crm_iap_lead_mining_request.py` (316 lines)
- `addons/crm_iap_mine/models/crm_iap_lead_role.py` (23 lines)
- `addons/crm_iap_mine/models/crm_iap_lead_seniority.py` (23 lines)
- `addons/crm_iap_mine/models/crm_lead.py` (24 lines)
- `addons/crm_iap_mine/security/ir.access.csv` (6 lines)
- `addons/crm_iap_mine/static/img/crunchbase.ico` (61 lines)
- `addons/crm_iap_mine/static/src/components/lead_generation_dropdown/crm_lead_gen_element.js` (28 lines)
- `addons/crm_iap_mine/static/src/js/tours/crm_iap_lead.js` (45 lines)
- `addons/crm_iap_mine/tests/__init__.py` (4 lines)
- `addons/crm_iap_mine/tests/common.py` (70 lines)
- `addons/crm_iap_mine/tests/test_lead_mine.py` (92 lines)
- `addons/crm_iap_mine/views/crm_iap_lead_industry_views.xml` (25 lines)
- `addons/crm_iap_mine/views/crm_iap_lead_mining_request_views.xml` (159 lines)
- `addons/crm_iap_mine/views/crm_menus.xml` (15 lines)
- `addons/crm_iap_mine/views/mail_templates.xml` (50 lines)
- `addons/crm_iap_mine/views/res_config_settings_views.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
