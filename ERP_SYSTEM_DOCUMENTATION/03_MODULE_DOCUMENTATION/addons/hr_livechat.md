# Module: hr_livechat

- **Module ID:** MOD-091
- **Path:** `addons/hr_livechat`
- **Manifest:** `addons/hr_livechat/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Bridge between HR and Livechat.

Declared dependencies: `hr`, `im_livechat`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 2 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "hr",
    "im_livechat"
  ],
  "data": [
    "views/discuss_channel_views.xml",
    "views/im_livechat_channel_member_history_views.xml",
    "views/im_livechat_report_channel_views.xml"
  ]
}
```

### Representative source files

- `addons/hr_livechat/__init__.py` (0 lines)
- `addons/hr_livechat/__manifest__.py` (15 lines)
- `addons/hr_livechat/i18n/ar.po` (40 lines)
- `addons/hr_livechat/i18n/az.po` (38 lines)
- `addons/hr_livechat/i18n/bg.po` (38 lines)
- `addons/hr_livechat/i18n/bs.po` (40 lines)
- `addons/hr_livechat/i18n/ca.po` (39 lines)
- `addons/hr_livechat/i18n/cs.po` (39 lines)
- `addons/hr_livechat/i18n/da.po` (39 lines)
- `addons/hr_livechat/i18n/de.po` (42 lines)
- `addons/hr_livechat/i18n/el.po` (39 lines)
- `addons/hr_livechat/i18n/es.po` (42 lines)
- `addons/hr_livechat/i18n/es_419.po` (42 lines)
- `addons/hr_livechat/i18n/et.po` (38 lines)
- `addons/hr_livechat/i18n/fa.po` (38 lines)
- `addons/hr_livechat/i18n/fi.po` (42 lines)
- `addons/hr_livechat/i18n/fr.po` (39 lines)
- `addons/hr_livechat/i18n/he.po` (39 lines)
- `addons/hr_livechat/i18n/hi.po` (38 lines)
- `addons/hr_livechat/i18n/hr.po` (39 lines)
- `addons/hr_livechat/i18n/hr_livechat.pot` (35 lines)
- `addons/hr_livechat/i18n/hu.po` (39 lines)
- `addons/hr_livechat/i18n/id.po` (39 lines)
- `addons/hr_livechat/i18n/it.po` (42 lines)
- `addons/hr_livechat/i18n/ja.po` (39 lines)
- `addons/hr_livechat/i18n/kab.po` (39 lines)
- `addons/hr_livechat/i18n/ko.po` (39 lines)
- `addons/hr_livechat/i18n/ku.po` (38 lines)
- `addons/hr_livechat/i18n/lo.po` (38 lines)
- `addons/hr_livechat/i18n/lt.po` (40 lines)
- `addons/hr_livechat/i18n/lv.po` (39 lines)
- `addons/hr_livechat/i18n/mn.po` (38 lines)
- `addons/hr_livechat/i18n/my.po` (38 lines)
- `addons/hr_livechat/i18n/nb.po` (39 lines)
- `addons/hr_livechat/i18n/nl.po` (39 lines)
- `addons/hr_livechat/i18n/pl.po` (40 lines)
- `addons/hr_livechat/i18n/pt.po` (39 lines)
- `addons/hr_livechat/i18n/pt_BR.po` (42 lines)
- `addons/hr_livechat/i18n/ro.po` (40 lines)
- `addons/hr_livechat/i18n/ru.po` (41 lines)
- `addons/hr_livechat/i18n/sk.po` (38 lines)
- `addons/hr_livechat/i18n/sl.po` (40 lines)
- `addons/hr_livechat/i18n/sr@latin.po` (39 lines)
- `addons/hr_livechat/i18n/sv.po` (42 lines)
- `addons/hr_livechat/i18n/th.po` (39 lines)
- `addons/hr_livechat/i18n/tr.po` (39 lines)
- `addons/hr_livechat/i18n/uk.po` (39 lines)
- `addons/hr_livechat/i18n/uz.po` (47 lines)
- `addons/hr_livechat/i18n/vi.po` (39 lines)
- `addons/hr_livechat/i18n/zh_CN.po` (39 lines)
- `addons/hr_livechat/i18n/zh_TW.po` (41 lines)
- `addons/hr_livechat/views/discuss_channel_views.xml` (19 lines)
- `addons/hr_livechat/views/im_livechat_channel_member_history_views.xml` (13 lines)
- `addons/hr_livechat/views/im_livechat_report_channel_views.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
