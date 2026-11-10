# Module: portal_discuss

- **Module ID:** MOD-420
- **Path:** `addons/portal_discuss`
- **Manifest:** `addons/portal_discuss/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Bridge module adding Discuss access from portal.

Declared dependencies: `mail`, `portal`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
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
    "mail",
    "portal"
  ],
  "data": [
    "data/portal_entry_data.xml",
    "views/portal_templates.xml"
  ],
  "assets": {
    "mail.assets_public": [
      "portal_discuss/static/src/core/common/**/*"
    ]
  }
}
```

### Representative source files

- `addons/portal_discuss/__init__.py` (4 lines)
- `addons/portal_discuss/__manifest__.py` (20 lines)
- `addons/portal_discuss/controllers/__init__.py` (4 lines)
- `addons/portal_discuss/controllers/portal.py` (17 lines)
- `addons/portal_discuss/controllers/public_page.py` (29 lines)
- `addons/portal_discuss/data/portal_entry_data.xml` (11 lines)
- `addons/portal_discuss/i18n/ar.po` (58 lines)
- `addons/portal_discuss/i18n/az.po` (58 lines)
- `addons/portal_discuss/i18n/bg.po` (58 lines)
- `addons/portal_discuss/i18n/bs.po` (58 lines)
- `addons/portal_discuss/i18n/ca.po` (58 lines)
- `addons/portal_discuss/i18n/cs.po` (58 lines)
- `addons/portal_discuss/i18n/da.po` (58 lines)
- `addons/portal_discuss/i18n/de.po` (63 lines)
- `addons/portal_discuss/i18n/el.po` (58 lines)
- `addons/portal_discuss/i18n/es.po` (62 lines)
- `addons/portal_discuss/i18n/es_419.po` (62 lines)
- `addons/portal_discuss/i18n/et.po` (58 lines)
- `addons/portal_discuss/i18n/fa.po` (58 lines)
- `addons/portal_discuss/i18n/fi.po` (62 lines)
- `addons/portal_discuss/i18n/fr.po` (58 lines)
- `addons/portal_discuss/i18n/he.po` (58 lines)
- `addons/portal_discuss/i18n/hi.po` (58 lines)
- `addons/portal_discuss/i18n/hr.po` (58 lines)
- `addons/portal_discuss/i18n/hu.po` (58 lines)
- `addons/portal_discuss/i18n/id.po` (62 lines)
- `addons/portal_discuss/i18n/it.po` (63 lines)
- `addons/portal_discuss/i18n/ja.po` (58 lines)
- `addons/portal_discuss/i18n/kab.po` (58 lines)
- `addons/portal_discuss/i18n/ko.po` (58 lines)
- `addons/portal_discuss/i18n/ku.po` (58 lines)
- `addons/portal_discuss/i18n/lo.po` (58 lines)
- `addons/portal_discuss/i18n/lt.po` (58 lines)
- `addons/portal_discuss/i18n/lv.po` (58 lines)
- `addons/portal_discuss/i18n/mn.po` (58 lines)
- `addons/portal_discuss/i18n/my.po` (58 lines)
- `addons/portal_discuss/i18n/nb.po` (58 lines)
- `addons/portal_discuss/i18n/nl.po` (62 lines)
- `addons/portal_discuss/i18n/pl.po` (58 lines)
- `addons/portal_discuss/i18n/portal_discuss.pot` (58 lines)
- `addons/portal_discuss/i18n/pt.po` (58 lines)
- `addons/portal_discuss/i18n/pt_BR.po` (68 lines)
- `addons/portal_discuss/i18n/ro.po` (58 lines)
- `addons/portal_discuss/i18n/ru.po` (58 lines)
- `addons/portal_discuss/i18n/sk.po` (58 lines)
- `addons/portal_discuss/i18n/sl.po` (58 lines)
- `addons/portal_discuss/i18n/sr@latin.po` (58 lines)
- `addons/portal_discuss/i18n/sv.po` (62 lines)
- `addons/portal_discuss/i18n/th.po` (58 lines)
- `addons/portal_discuss/i18n/tr.po` (58 lines)
- `addons/portal_discuss/i18n/uk.po` (58 lines)
- `addons/portal_discuss/i18n/uz.po` (58 lines)
- `addons/portal_discuss/i18n/vi.po` (58 lines)
- `addons/portal_discuss/i18n/zh_CN.po` (63 lines)
- `addons/portal_discuss/i18n/zh_TW.po` (58 lines)
- `addons/portal_discuss/models/__init__.py` (4 lines)
- `addons/portal_discuss/models/discuss_channel.py` (18 lines)
- `addons/portal_discuss/models/portal_entry.py` (23 lines)
- `addons/portal_discuss/static/src/core/common/discuss_client_action_patch.js` (16 lines)
- `addons/portal_discuss/static/src/img/portal-discuss.png` (229 lines)
- `addons/portal_discuss/tests/__init__.py` (3 lines)
- `addons/portal_discuss/tests/test_portal_discuss.py` (18 lines)
- `addons/portal_discuss/views/portal_templates.xml` (8 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
