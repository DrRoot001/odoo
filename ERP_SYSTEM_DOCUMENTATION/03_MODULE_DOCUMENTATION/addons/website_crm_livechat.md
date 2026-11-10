# Module: website_crm_livechat

- **Module ID:** MOD-602
- **Path:** `addons/website_crm_livechat`
- **Manifest:** `addons/website_crm_livechat/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

View livechat sessions for leads

 Adds a stat button on lead form view to access their livechat sessions.

Declared dependencies: `website_crm`, `website_livechat`, `crm_livechat`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website_crm",
    "website_livechat",
    "crm_livechat"
  ],
  "data": [
    "views/website_crm_lead_views.xml"
  ]
}
```

### Representative source files

- `addons/website_crm_livechat/__init__.py` (4 lines)
- `addons/website_crm_livechat/__manifest__.py` (14 lines)
- `addons/website_crm_livechat/i18n/ar.po` (86 lines)
- `addons/website_crm_livechat/i18n/az.po` (84 lines)
- `addons/website_crm_livechat/i18n/bg.po` (84 lines)
- `addons/website_crm_livechat/i18n/bs.po` (86 lines)
- `addons/website_crm_livechat/i18n/ca.po` (85 lines)
- `addons/website_crm_livechat/i18n/cs.po` (85 lines)
- `addons/website_crm_livechat/i18n/da.po` (86 lines)
- `addons/website_crm_livechat/i18n/de.po` (88 lines)
- `addons/website_crm_livechat/i18n/el.po` (85 lines)
- `addons/website_crm_livechat/i18n/es.po` (88 lines)
- `addons/website_crm_livechat/i18n/es_419.po` (85 lines)
- `addons/website_crm_livechat/i18n/et.po` (84 lines)
- `addons/website_crm_livechat/i18n/fa.po` (84 lines)
- `addons/website_crm_livechat/i18n/fi.po` (86 lines)
- `addons/website_crm_livechat/i18n/fr.po` (85 lines)
- `addons/website_crm_livechat/i18n/he.po` (85 lines)
- `addons/website_crm_livechat/i18n/hi.po` (84 lines)
- `addons/website_crm_livechat/i18n/hr.po` (85 lines)
- `addons/website_crm_livechat/i18n/hu.po` (85 lines)
- `addons/website_crm_livechat/i18n/id.po` (86 lines)
- `addons/website_crm_livechat/i18n/it.po` (85 lines)
- `addons/website_crm_livechat/i18n/ja.po` (85 lines)
- `addons/website_crm_livechat/i18n/kab.po` (85 lines)
- `addons/website_crm_livechat/i18n/ko.po` (85 lines)
- `addons/website_crm_livechat/i18n/ku.po` (84 lines)
- `addons/website_crm_livechat/i18n/lo.po` (84 lines)
- `addons/website_crm_livechat/i18n/lt.po` (86 lines)
- `addons/website_crm_livechat/i18n/lv.po` (85 lines)
- `addons/website_crm_livechat/i18n/mn.po` (84 lines)
- `addons/website_crm_livechat/i18n/my.po` (84 lines)
- `addons/website_crm_livechat/i18n/nb.po` (85 lines)
- `addons/website_crm_livechat/i18n/nl.po` (85 lines)
- `addons/website_crm_livechat/i18n/pl.po` (86 lines)
- `addons/website_crm_livechat/i18n/pt.po` (86 lines)
- `addons/website_crm_livechat/i18n/pt_BR.po` (88 lines)
- `addons/website_crm_livechat/i18n/ro.po` (86 lines)
- `addons/website_crm_livechat/i18n/ru.po` (90 lines)
- `addons/website_crm_livechat/i18n/sk.po` (84 lines)
- `addons/website_crm_livechat/i18n/sl.po` (86 lines)
- `addons/website_crm_livechat/i18n/sr@latin.po` (85 lines)
- `addons/website_crm_livechat/i18n/sv.po` (86 lines)
- `addons/website_crm_livechat/i18n/th.po` (85 lines)
- `addons/website_crm_livechat/i18n/tr.po` (86 lines)
- `addons/website_crm_livechat/i18n/uk.po` (85 lines)
- `addons/website_crm_livechat/i18n/uz.po` (101 lines)
- `addons/website_crm_livechat/i18n/vi.po` (85 lines)
- `addons/website_crm_livechat/i18n/website_crm_livechat.pot` (82 lines)
- `addons/website_crm_livechat/i18n/zh_CN.po` (85 lines)
- `addons/website_crm_livechat/i18n/zh_TW.po` (88 lines)
- `addons/website_crm_livechat/models/__init__.py` (6 lines)
- `addons/website_crm_livechat/models/chatbot_script_step.py` (17 lines)
- `addons/website_crm_livechat/models/crm_lead.py` (21 lines)
- `addons/website_crm_livechat/models/discuss_channel.py` (19 lines)
- `addons/website_crm_livechat/tests/__init__.py` (3 lines)
- `addons/website_crm_livechat/tests/test_chatbot_lead_website.py` (24 lines)
- `addons/website_crm_livechat/views/website_crm_lead_views.xml` (16 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
