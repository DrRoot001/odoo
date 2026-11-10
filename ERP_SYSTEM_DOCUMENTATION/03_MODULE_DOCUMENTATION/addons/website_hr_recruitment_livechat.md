# Module: website_hr_recruitment_livechat

- **Module ID:** MOD-621
- **Path:** `addons/website_hr_recruitment_livechat`
- **Manifest:** `addons/website_hr_recruitment_livechat/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Chatbot for the HR Recruitment


A chatbot to help the user be guided through recruitment process on the website and land on the right jobs position.
    

Declared dependencies: `website_hr_recruitment`, `im_livechat`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 2 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website_hr_recruitment",
    "im_livechat"
  ],
  "demo": [
    "data/website_hr_recruitment_livechat_chatbot_demo.xml"
  ]
}
```

### Representative source files

- `addons/website_hr_recruitment_livechat/__init__.py` (0 lines)
- `addons/website_hr_recruitment_livechat/__manifest__.py` (17 lines)
- `addons/website_hr_recruitment_livechat/data/website_hr_recruitment_livechat_chatbot_demo.xml` (409 lines)
- `addons/website_hr_recruitment_livechat/i18n/ar.po` (170 lines)
- `addons/website_hr_recruitment_livechat/i18n/az.po` (166 lines)
- `addons/website_hr_recruitment_livechat/i18n/bg.po` (166 lines)
- `addons/website_hr_recruitment_livechat/i18n/bs.po` (167 lines)
- `addons/website_hr_recruitment_livechat/i18n/ca.po` (169 lines)
- `addons/website_hr_recruitment_livechat/i18n/cs.po` (169 lines)
- `addons/website_hr_recruitment_livechat/i18n/da.po` (167 lines)
- `addons/website_hr_recruitment_livechat/i18n/de.po` (182 lines)
- `addons/website_hr_recruitment_livechat/i18n/el.po` (166 lines)
- `addons/website_hr_recruitment_livechat/i18n/es.po` (181 lines)
- `addons/website_hr_recruitment_livechat/i18n/es_419.po` (171 lines)
- `addons/website_hr_recruitment_livechat/i18n/et.po` (166 lines)
- `addons/website_hr_recruitment_livechat/i18n/fa.po` (166 lines)
- `addons/website_hr_recruitment_livechat/i18n/fi.po` (172 lines)
- `addons/website_hr_recruitment_livechat/i18n/fr.po` (176 lines)
- `addons/website_hr_recruitment_livechat/i18n/he.po` (167 lines)
- `addons/website_hr_recruitment_livechat/i18n/hi.po` (166 lines)
- `addons/website_hr_recruitment_livechat/i18n/hr.po` (167 lines)
- `addons/website_hr_recruitment_livechat/i18n/hu.po` (166 lines)
- `addons/website_hr_recruitment_livechat/i18n/id.po` (171 lines)
- `addons/website_hr_recruitment_livechat/i18n/it.po` (178 lines)
- `addons/website_hr_recruitment_livechat/i18n/ja.po` (170 lines)
- `addons/website_hr_recruitment_livechat/i18n/kab.po` (166 lines)
- `addons/website_hr_recruitment_livechat/i18n/ko.po` (167 lines)
- `addons/website_hr_recruitment_livechat/i18n/ku.po` (166 lines)
- `addons/website_hr_recruitment_livechat/i18n/lo.po` (171 lines)
- `addons/website_hr_recruitment_livechat/i18n/lt.po` (168 lines)
- `addons/website_hr_recruitment_livechat/i18n/lv.po` (166 lines)
- `addons/website_hr_recruitment_livechat/i18n/mn.po` (166 lines)
- `addons/website_hr_recruitment_livechat/i18n/my.po` (167 lines)
- `addons/website_hr_recruitment_livechat/i18n/nb.po` (166 lines)
- `addons/website_hr_recruitment_livechat/i18n/nl.po` (172 lines)
- `addons/website_hr_recruitment_livechat/i18n/pl.po` (178 lines)
- `addons/website_hr_recruitment_livechat/i18n/pt.po` (168 lines)
- `addons/website_hr_recruitment_livechat/i18n/pt_BR.po` (179 lines)
- `addons/website_hr_recruitment_livechat/i18n/ro.po` (167 lines)
- `addons/website_hr_recruitment_livechat/i18n/ru.po` (173 lines)
- `addons/website_hr_recruitment_livechat/i18n/sk.po` (165 lines)
- `addons/website_hr_recruitment_livechat/i18n/sl.po` (168 lines)
- `addons/website_hr_recruitment_livechat/i18n/sr@latin.po` (169 lines)
- `addons/website_hr_recruitment_livechat/i18n/sv.po` (166 lines)
- `addons/website_hr_recruitment_livechat/i18n/th.po` (167 lines)
- `addons/website_hr_recruitment_livechat/i18n/tr.po` (173 lines)
- `addons/website_hr_recruitment_livechat/i18n/uk.po` (168 lines)
- `addons/website_hr_recruitment_livechat/i18n/uz.po` (202 lines)
- `addons/website_hr_recruitment_livechat/i18n/vi.po` (169 lines)
- `addons/website_hr_recruitment_livechat/i18n/website_hr_recruitment_livechat.pot` (162 lines)
- `addons/website_hr_recruitment_livechat/i18n/zh_CN.po` (170 lines)
- `addons/website_hr_recruitment_livechat/i18n/zh_TW.po` (167 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
