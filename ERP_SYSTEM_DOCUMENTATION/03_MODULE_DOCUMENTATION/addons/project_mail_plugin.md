# Module: project_mail_plugin

- **Module ID:** MOD-479
- **Path:** `addons/project_mail_plugin`
- **Manifest:** `addons/project_mail_plugin/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Integrate your inbox with projects

Turn emails received in your mailbox into tasks and log their content as internal notes.

Declared dependencies: `project`, `mail_plugin`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 3 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "project",
    "mail_plugin"
  ]
}
```

### Representative source files

- `addons/project_mail_plugin/__init__.py` (3 lines)
- `addons/project_mail_plugin/__manifest__.py` (17 lines)
- `addons/project_mail_plugin/controllers/__init__.py` (3 lines)
- `addons/project_mail_plugin/controllers/mail_plugin.py` (192 lines)
- `addons/project_mail_plugin/i18n/ar.po` (190 lines)
- `addons/project_mail_plugin/i18n/az.po` (188 lines)
- `addons/project_mail_plugin/i18n/bg.po` (188 lines)
- `addons/project_mail_plugin/i18n/bs.po` (190 lines)
- `addons/project_mail_plugin/i18n/ca.po` (191 lines)
- `addons/project_mail_plugin/i18n/cs.po` (189 lines)
- `addons/project_mail_plugin/i18n/da.po` (190 lines)
- `addons/project_mail_plugin/i18n/de.po` (194 lines)
- `addons/project_mail_plugin/i18n/el.po` (189 lines)
- `addons/project_mail_plugin/i18n/es.po` (194 lines)
- `addons/project_mail_plugin/i18n/es_419.po` (192 lines)
- `addons/project_mail_plugin/i18n/et.po` (191 lines)
- `addons/project_mail_plugin/i18n/fa.po` (188 lines)
- `addons/project_mail_plugin/i18n/fi.po` (191 lines)
- `addons/project_mail_plugin/i18n/fr.po` (192 lines)
- `addons/project_mail_plugin/i18n/he.po` (189 lines)
- `addons/project_mail_plugin/i18n/hi.po` (188 lines)
- `addons/project_mail_plugin/i18n/hr.po` (189 lines)
- `addons/project_mail_plugin/i18n/hu.po` (189 lines)
- `addons/project_mail_plugin/i18n/id.po` (192 lines)
- `addons/project_mail_plugin/i18n/it.po` (192 lines)
- `addons/project_mail_plugin/i18n/ja.po` (192 lines)
- `addons/project_mail_plugin/i18n/kab.po` (189 lines)
- `addons/project_mail_plugin/i18n/ko.po` (192 lines)
- `addons/project_mail_plugin/i18n/ku.po` (188 lines)
- `addons/project_mail_plugin/i18n/lo.po` (191 lines)
- `addons/project_mail_plugin/i18n/lt.po` (190 lines)
- `addons/project_mail_plugin/i18n/lv.po` (189 lines)
- `addons/project_mail_plugin/i18n/mn.po` (188 lines)
- `addons/project_mail_plugin/i18n/my.po` (188 lines)
- `addons/project_mail_plugin/i18n/nb.po` (189 lines)
- `addons/project_mail_plugin/i18n/nl.po` (192 lines)
- `addons/project_mail_plugin/i18n/pl.po` (192 lines)
- `addons/project_mail_plugin/i18n/project_mail_plugin.pot` (185 lines)
- `addons/project_mail_plugin/i18n/pt.po` (191 lines)
- `addons/project_mail_plugin/i18n/pt_BR.po` (196 lines)
- `addons/project_mail_plugin/i18n/ro.po` (192 lines)
- `addons/project_mail_plugin/i18n/ru.po` (193 lines)
- `addons/project_mail_plugin/i18n/sk.po` (188 lines)
- `addons/project_mail_plugin/i18n/sl.po` (191 lines)
- `addons/project_mail_plugin/i18n/sr@latin.po` (189 lines)
- `addons/project_mail_plugin/i18n/sv.po` (191 lines)
- `addons/project_mail_plugin/i18n/th.po` (190 lines)
- `addons/project_mail_plugin/i18n/tr.po` (191 lines)
- `addons/project_mail_plugin/i18n/uk.po` (189 lines)
- `addons/project_mail_plugin/i18n/uz.po` (215 lines)
- `addons/project_mail_plugin/i18n/vi.po` (191 lines)
- `addons/project_mail_plugin/i18n/zh_CN.po` (190 lines)
- `addons/project_mail_plugin/i18n/zh_TW.po` (191 lines)
- `addons/project_mail_plugin/static/src/to_translate/translations_gmail.xml` (26 lines)
- `addons/project_mail_plugin/static/src/to_translate/translations_outlook.xml` (26 lines)
- `addons/project_mail_plugin/tests/__init__.py` (3 lines)
- `addons/project_mail_plugin/tests/test_controller.py` (53 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
