# Module: website_crm_iap_reveal

- **Module ID:** MOD-601
- **Path:** `addons/website_crm_iap_reveal`
- **Manifest:** `addons/website_crm_iap_reveal/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Generate Leads/Opportunities from your website's traffic

No manifest description declared.

Declared dependencies: `iap_crm`, `iap_mail`, `crm_iap_mine`, `website_crm`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 7 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "iap_crm",
    "iap_mail",
    "crm_iap_mine",
    "website_crm"
  ],
  "data": [
    "data/ir_cron_data.xml",
    "data/ir_model_data.xml",
    "data/mail_templates.xml",
    "views/crm_lead_views.xml",
    "views/crm_reveal_views.xml",
    "views/res_config_settings_views.xml",
    "views/crm_menus.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/website_crm_iap_reveal/__init__.py` (5 lines)
- `addons/website_crm_iap_reveal/__manifest__.py` (27 lines)
- `addons/website_crm_iap_reveal/controllers/__init__.py` (4 lines)
- `addons/website_crm_iap_reveal/controllers/website_form.py` (18 lines)
- `addons/website_crm_iap_reveal/data/ir_cron_data.xml` (15 lines)
- `addons/website_crm_iap_reveal/data/ir_model_data.xml` (7 lines)
- `addons/website_crm_iap_reveal/data/mail_templates.xml` (59 lines)
- `addons/website_crm_iap_reveal/i18n/ar.po` (563 lines)
- `addons/website_crm_iap_reveal/i18n/az.po` (575 lines)
- `addons/website_crm_iap_reveal/i18n/bg.po` (587 lines)
- `addons/website_crm_iap_reveal/i18n/bs.po` (576 lines)
- `addons/website_crm_iap_reveal/i18n/ca.po` (564 lines)
- `addons/website_crm_iap_reveal/i18n/cs.po` (573 lines)
- `addons/website_crm_iap_reveal/i18n/da.po` (563 lines)
- `addons/website_crm_iap_reveal/i18n/de.po` (568 lines)
- `addons/website_crm_iap_reveal/i18n/el.po` (538 lines)
- `addons/website_crm_iap_reveal/i18n/es.po` (564 lines)
- `addons/website_crm_iap_reveal/i18n/es_419.po` (562 lines)
- `addons/website_crm_iap_reveal/i18n/et.po` (646 lines)
- `addons/website_crm_iap_reveal/i18n/fa.po` (585 lines)
- `addons/website_crm_iap_reveal/i18n/fi.po` (561 lines)
- `addons/website_crm_iap_reveal/i18n/fr.po` (568 lines)
- `addons/website_crm_iap_reveal/i18n/he.po` (562 lines)
- `addons/website_crm_iap_reveal/i18n/hi.po` (585 lines)
- `addons/website_crm_iap_reveal/i18n/hr.po` (555 lines)
- `addons/website_crm_iap_reveal/i18n/hu.po` (546 lines)
- `addons/website_crm_iap_reveal/i18n/id.po` (560 lines)
- `addons/website_crm_iap_reveal/i18n/it.po` (563 lines)
- `addons/website_crm_iap_reveal/i18n/ja.po` (553 lines)
- `addons/website_crm_iap_reveal/i18n/kab.po` (558 lines)
- `addons/website_crm_iap_reveal/i18n/ko.po` (551 lines)
- `addons/website_crm_iap_reveal/i18n/ku.po` (556 lines)
- `addons/website_crm_iap_reveal/i18n/lo.po` (546 lines)
- `addons/website_crm_iap_reveal/i18n/lt.po` (552 lines)
- `addons/website_crm_iap_reveal/i18n/lv.po` (577 lines)
- `addons/website_crm_iap_reveal/i18n/mn.po` (545 lines)
- `addons/website_crm_iap_reveal/i18n/my.po` (559 lines)
- `addons/website_crm_iap_reveal/i18n/nb.po` (542 lines)
- `addons/website_crm_iap_reveal/i18n/nl.po` (564 lines)
- `addons/website_crm_iap_reveal/i18n/pl.po` (575 lines)
- `addons/website_crm_iap_reveal/i18n/pt.po` (573 lines)
- `addons/website_crm_iap_reveal/i18n/pt_BR.po` (568 lines)
- `addons/website_crm_iap_reveal/i18n/ro.po` (593 lines)
- `addons/website_crm_iap_reveal/i18n/ru.po` (565 lines)
- `addons/website_crm_iap_reveal/i18n/sk.po` (652 lines)
- `addons/website_crm_iap_reveal/i18n/sl.po` (538 lines)
- `addons/website_crm_iap_reveal/i18n/sr@latin.po` (571 lines)
- `addons/website_crm_iap_reveal/i18n/sv.po` (559 lines)
- `addons/website_crm_iap_reveal/i18n/th.po` (545 lines)
- `addons/website_crm_iap_reveal/i18n/tr.po` (569 lines)
- `addons/website_crm_iap_reveal/i18n/uk.po` (567 lines)
- `addons/website_crm_iap_reveal/i18n/uz.po` (659 lines)
- `addons/website_crm_iap_reveal/i18n/vi.po` (559 lines)
- `addons/website_crm_iap_reveal/i18n/website_crm_iap_reveal.pot` (532 lines)
- `addons/website_crm_iap_reveal/i18n/zh_CN.po` (547 lines)
- `addons/website_crm_iap_reveal/i18n/zh_TW.po` (544 lines)
- `addons/website_crm_iap_reveal/models/__init__.py` (7 lines)
- `addons/website_crm_iap_reveal/models/crm_lead.py` (15 lines)
- `addons/website_crm_iap_reveal/models/crm_reveal_rule.py` (387 lines)
- `addons/website_crm_iap_reveal/models/crm_reveal_view.py` (49 lines)
- `addons/website_crm_iap_reveal/models/ir_http.py` (45 lines)
- `addons/website_crm_iap_reveal/security/ir.access.csv` (7 lines)
- `addons/website_crm_iap_reveal/tests/__init__.py` (4 lines)
- `addons/website_crm_iap_reveal/tests/common.py` (83 lines)
- `addons/website_crm_iap_reveal/tests/test_lead_reveal.py` (190 lines)
- `addons/website_crm_iap_reveal/views/crm_lead_views.xml` (96 lines)
- `addons/website_crm_iap_reveal/views/crm_menus.xml` (14 lines)
- `addons/website_crm_iap_reveal/views/crm_reveal_views.xml` (166 lines)
- `addons/website_crm_iap_reveal/views/res_config_settings_views.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
