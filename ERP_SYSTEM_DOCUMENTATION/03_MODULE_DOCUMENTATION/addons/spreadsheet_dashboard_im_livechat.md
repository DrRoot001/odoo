# Module: spreadsheet_dashboard_im_livechat

- **Module ID:** MOD-551
- **Path:** `addons/spreadsheet_dashboard_im_livechat`
- **Manifest:** `addons/spreadsheet_dashboard_im_livechat/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['im_livechat']`
- **License:** `LGPL-3`

## Purpose and dependencies

Spreadsheet

Spreadsheet

Declared dependencies: `spreadsheet_dashboard`, `im_livechat`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 2 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "spreadsheet_dashboard",
    "im_livechat"
  ],
  "data": [
    "data/livechat_ongoing_sessions_actions.xml",
    "data/dashboards.xml"
  ]
}
```

### Representative source files

- `addons/spreadsheet_dashboard_im_livechat/__init__.py` (1 lines)
- `addons/spreadsheet_dashboard_im_livechat/__manifest__.py` (15 lines)
- `addons/spreadsheet_dashboard_im_livechat/data/dashboards.xml` (25 lines)
- `addons/spreadsheet_dashboard_im_livechat/data/files/livechat_dashboard.json` (2,443 lines)
- `addons/spreadsheet_dashboard_im_livechat/data/files/livechat_ongoing_dashboard.json` (1,444 lines)
- `addons/spreadsheet_dashboard_im_livechat/data/files/livechat_sample_dashboard.json` (1,903 lines)
- `addons/spreadsheet_dashboard_im_livechat/data/files/livechat_sample_ongoing_dashboard.json` (939 lines)
- `addons/spreadsheet_dashboard_im_livechat/data/livechat_ongoing_sessions_actions.xml` (90 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/ar.po` (411 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/az.po` (407 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/bg.po` (407 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/bs.po` (409 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/ca.po` (408 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/cs.po` (408 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/da.po` (409 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/de.po` (409 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/el.po` (408 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/es.po` (413 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/es_419.po` (410 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/et.po` (407 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/fa.po` (407 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/fi.po` (409 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/fr.po` (410 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/he.po` (408 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/hi.po` (407 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/hr.po` (408 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/hu.po` (408 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/id.po` (410 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/it.po` (410 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/ja.po` (410 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/kab.po` (408 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/ko.po` (409 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/ku.po` (407 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/lo.po` (407 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/lt.po` (409 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/lv.po` (408 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/mn.po` (407 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/my.po` (407 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/nb.po` (408 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/nl.po` (411 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/pl.po` (410 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/pt.po` (408 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/pt_BR.po` (411 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/ro.po` (408 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/ru.po` (411 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/sk.po` (407 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/sl.po` (409 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/spreadsheet_dashboard_im_livechat.pot` (404 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/sr@latin.po` (408 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/sv.po` (409 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/th.po` (409 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/tr.po` (411 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/uk.po` (408 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/uz.po` (467 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/vi.po` (409 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/zh_CN.po` (410 lines)
- `addons/spreadsheet_dashboard_im_livechat/i18n/zh_TW.po` (413 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
