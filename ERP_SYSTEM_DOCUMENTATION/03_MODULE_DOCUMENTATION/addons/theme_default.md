# Module: theme_default

- **Module ID:** MOD-589
- **Path:** `addons/theme_default`
- **Manifest:** `addons/theme_default/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Default website theme

Declared dependencies: `website`.

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
    "website"
  ],
  "data": [
    "data/generate_primary_template.xml"
  ]
}
```

### Representative source files

- `addons/theme_default/__init__.py` (2 lines)
- `addons/theme_default/__manifest__.py` (18 lines)
- `addons/theme_default/data/generate_primary_template.xml` (9 lines)
- `addons/theme_default/i18n/ar.po` (26 lines)
- `addons/theme_default/i18n/az.po` (26 lines)
- `addons/theme_default/i18n/bg.po` (26 lines)
- `addons/theme_default/i18n/bs.po` (26 lines)
- `addons/theme_default/i18n/ca.po` (26 lines)
- `addons/theme_default/i18n/cs.po` (26 lines)
- `addons/theme_default/i18n/da.po` (26 lines)
- `addons/theme_default/i18n/de.po` (30 lines)
- `addons/theme_default/i18n/el.po` (26 lines)
- `addons/theme_default/i18n/es.po` (30 lines)
- `addons/theme_default/i18n/es_419.po` (26 lines)
- `addons/theme_default/i18n/et.po` (26 lines)
- `addons/theme_default/i18n/fa.po` (26 lines)
- `addons/theme_default/i18n/fi.po` (26 lines)
- `addons/theme_default/i18n/fr.po` (26 lines)
- `addons/theme_default/i18n/he.po` (26 lines)
- `addons/theme_default/i18n/hi.po` (26 lines)
- `addons/theme_default/i18n/hr.po` (26 lines)
- `addons/theme_default/i18n/hu.po` (26 lines)
- `addons/theme_default/i18n/id.po` (26 lines)
- `addons/theme_default/i18n/it.po` (26 lines)
- `addons/theme_default/i18n/ja.po` (26 lines)
- `addons/theme_default/i18n/kab.po` (26 lines)
- `addons/theme_default/i18n/ko.po` (26 lines)
- `addons/theme_default/i18n/ku.po` (26 lines)
- `addons/theme_default/i18n/lo.po` (26 lines)
- `addons/theme_default/i18n/lt.po` (26 lines)
- `addons/theme_default/i18n/lv.po` (26 lines)
- `addons/theme_default/i18n/mn.po` (26 lines)
- `addons/theme_default/i18n/my.po` (26 lines)
- `addons/theme_default/i18n/nb.po` (26 lines)
- `addons/theme_default/i18n/nl.po` (26 lines)
- `addons/theme_default/i18n/pl.po` (26 lines)
- `addons/theme_default/i18n/pt.po` (26 lines)
- `addons/theme_default/i18n/pt_BR.po` (30 lines)
- `addons/theme_default/i18n/ro.po` (26 lines)
- `addons/theme_default/i18n/ru.po` (26 lines)
- `addons/theme_default/i18n/sk.po` (26 lines)
- `addons/theme_default/i18n/sl.po` (26 lines)
- `addons/theme_default/i18n/sr@latin.po` (26 lines)
- `addons/theme_default/i18n/sv.po` (30 lines)
- `addons/theme_default/i18n/th.po` (26 lines)
- `addons/theme_default/i18n/theme_default.pot` (26 lines)
- `addons/theme_default/i18n/tr.po` (26 lines)
- `addons/theme_default/i18n/uk.po` (26 lines)
- `addons/theme_default/i18n/uz.po` (26 lines)
- `addons/theme_default/i18n/vi.po` (26 lines)
- `addons/theme_default/i18n/zh_CN.po` (30 lines)
- `addons/theme_default/i18n/zh_TW.po` (26 lines)
- `addons/theme_default/static/description/cover.png` (86 lines)
- `addons/theme_default/static/description/icon.png` (14 lines)
- `addons/theme_default/static/description/theme_default_screenshot.jpg` (718 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
