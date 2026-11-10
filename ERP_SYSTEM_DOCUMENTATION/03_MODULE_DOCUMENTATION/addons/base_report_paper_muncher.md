# Module: base_report_paper_muncher

- **Module ID:** MOD-040
- **Path:** `addons/base_report_paper_muncher`
- **Manifest:** `addons/base_report_paper_muncher/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Paper Muncher Engine


This module is the implementation of the odoo's
in house rendering engine called Paper Muncher.

learn more about it here:
https://odoo.github.io/paper-muncher/
    

Declared dependencies: `base_setup`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base_setup"
  ]
}
```

### Representative source files

- `addons/base_report_paper_muncher/README.md` (8 lines)
- `addons/base_report_paper_muncher/__init__.py` (3 lines)
- `addons/base_report_paper_muncher/__manifest__.py` (19 lines)
- `addons/base_report_paper_muncher/i18n/ar.po` (74 lines)
- `addons/base_report_paper_muncher/i18n/az.po` (73 lines)
- `addons/base_report_paper_muncher/i18n/base_report_paper_muncher.pot` (70 lines)
- `addons/base_report_paper_muncher/i18n/bg.po` (73 lines)
- `addons/base_report_paper_muncher/i18n/bs.po` (74 lines)
- `addons/base_report_paper_muncher/i18n/ca.po` (73 lines)
- `addons/base_report_paper_muncher/i18n/cs.po` (73 lines)
- `addons/base_report_paper_muncher/i18n/da.po` (77 lines)
- `addons/base_report_paper_muncher/i18n/de.po` (85 lines)
- `addons/base_report_paper_muncher/i18n/el.po` (73 lines)
- `addons/base_report_paper_muncher/i18n/es.po` (74 lines)
- `addons/base_report_paper_muncher/i18n/es_419.po` (84 lines)
- `addons/base_report_paper_muncher/i18n/et.po` (73 lines)
- `addons/base_report_paper_muncher/i18n/fa.po` (73 lines)
- `addons/base_report_paper_muncher/i18n/fi.po` (80 lines)
- `addons/base_report_paper_muncher/i18n/fr.po` (83 lines)
- `addons/base_report_paper_muncher/i18n/he.po` (74 lines)
- `addons/base_report_paper_muncher/i18n/hi.po` (73 lines)
- `addons/base_report_paper_muncher/i18n/hr.po` (74 lines)
- `addons/base_report_paper_muncher/i18n/hu.po` (73 lines)
- `addons/base_report_paper_muncher/i18n/id.po` (73 lines)
- `addons/base_report_paper_muncher/i18n/it.po` (84 lines)
- `addons/base_report_paper_muncher/i18n/ja.po` (83 lines)
- `addons/base_report_paper_muncher/i18n/kab.po` (73 lines)
- `addons/base_report_paper_muncher/i18n/ko.po` (73 lines)
- `addons/base_report_paper_muncher/i18n/ku.po` (73 lines)
- `addons/base_report_paper_muncher/i18n/lo.po` (73 lines)
- `addons/base_report_paper_muncher/i18n/lt.po` (75 lines)
- `addons/base_report_paper_muncher/i18n/lv.po` (74 lines)
- `addons/base_report_paper_muncher/i18n/mn.po` (73 lines)
- `addons/base_report_paper_muncher/i18n/my.po` (73 lines)
- `addons/base_report_paper_muncher/i18n/nb.po` (73 lines)
- `addons/base_report_paper_muncher/i18n/nl.po` (78 lines)
- `addons/base_report_paper_muncher/i18n/pl.po` (74 lines)
- `addons/base_report_paper_muncher/i18n/pt.po` (73 lines)
- `addons/base_report_paper_muncher/i18n/pt_BR.po` (83 lines)
- `addons/base_report_paper_muncher/i18n/ro.po` (74 lines)
- `addons/base_report_paper_muncher/i18n/ru.po` (74 lines)
- `addons/base_report_paper_muncher/i18n/sk.po` (73 lines)
- `addons/base_report_paper_muncher/i18n/sl.po` (74 lines)
- `addons/base_report_paper_muncher/i18n/sr@latin.po` (74 lines)
- `addons/base_report_paper_muncher/i18n/sv.po` (74 lines)
- `addons/base_report_paper_muncher/i18n/th.po` (73 lines)
- `addons/base_report_paper_muncher/i18n/tr.po` (83 lines)
- `addons/base_report_paper_muncher/i18n/uk.po` (74 lines)
- `addons/base_report_paper_muncher/i18n/uz.po` (73 lines)
- `addons/base_report_paper_muncher/i18n/vi.po` (73 lines)
- `addons/base_report_paper_muncher/i18n/zh_CN.po` (83 lines)
- `addons/base_report_paper_muncher/i18n/zh_TW.po` (74 lines)
- `addons/base_report_paper_muncher/models/__init__.py` (3 lines)
- `addons/base_report_paper_muncher/models/ir_actions_report.py` (187 lines)
- `addons/base_report_paper_muncher/paper_muncher.py` (408 lines)
- `addons/base_report_paper_muncher/static/description/icon.png` (99 lines)
- `addons/base_report_paper_muncher/static/description/icon.svg` (17 lines)
- `addons/base_report_paper_muncher/tests/__init__.py` (3 lines)
- `addons/base_report_paper_muncher/tests/test_report.py` (89 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
