# Module: populate

- **Module ID:** MOD-418
- **Path:** `addons/populate`
- **Manifest:** `addons/populate/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Generate synthetic data for an Odoo database

Generate synthetic data for an Odoo database, following a predefined blueprint. Used for performance testing.

Declared dependencies: `base`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 30 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base"
  ],
  "data": [
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/populate/README.md` (788 lines)
- `addons/populate/__init__.py` (6 lines)
- `addons/populate/__manifest__.py` (13 lines)
- `addons/populate/cli/populate.py` (231 lines)
- `addons/populate/generators/__init__.py` (72 lines)
- `addons/populate/generators/binary.py` (81 lines)
- `addons/populate/generators/choice.py` (60 lines)
- `addons/populate/generators/fake.py` (208 lines)
- `addons/populate/generators/generator.py` (524 lines)
- `addons/populate/generators/misc.py` (181 lines)
- `addons/populate/generators/properties.py` (285 lines)
- `addons/populate/generators/reference.py` (116 lines)
- `addons/populate/generators/relation.py` (149 lines)
- `addons/populate/generators/scalar.py` (137 lines)
- `addons/populate/generators/temporal.py` (70 lines)
- `addons/populate/generators/textual.py` (38 lines)
- `addons/populate/i18n/ar.po` (868 lines)
- `addons/populate/i18n/az.po` (867 lines)
- `addons/populate/i18n/bg.po` (867 lines)
- `addons/populate/i18n/bs.po` (868 lines)
- `addons/populate/i18n/ca.po` (867 lines)
- `addons/populate/i18n/cs.po` (867 lines)
- `addons/populate/i18n/da.po` (867 lines)
- `addons/populate/i18n/de.po` (958 lines)
- `addons/populate/i18n/el.po` (867 lines)
- `addons/populate/i18n/es.po` (868 lines)
- `addons/populate/i18n/es_419.po` (920 lines)
- `addons/populate/i18n/et.po` (867 lines)
- `addons/populate/i18n/fa.po` (867 lines)
- `addons/populate/i18n/fi.po` (868 lines)
- `addons/populate/i18n/fr.po` (923 lines)
- `addons/populate/i18n/he.po` (868 lines)
- `addons/populate/i18n/hi.po` (867 lines)
- `addons/populate/i18n/hr.po` (868 lines)
- `addons/populate/i18n/hu.po` (867 lines)
- `addons/populate/i18n/id.po` (867 lines)
- `addons/populate/i18n/it.po` (931 lines)
- `addons/populate/i18n/ja.po` (868 lines)
- `addons/populate/i18n/kab.po` (867 lines)
- `addons/populate/i18n/ko.po` (867 lines)
- `addons/populate/i18n/ku.po` (867 lines)
- `addons/populate/i18n/lo.po` (922 lines)
- `addons/populate/i18n/lt.po` (869 lines)
- `addons/populate/i18n/lv.po` (868 lines)
- `addons/populate/i18n/mn.po` (867 lines)
- `addons/populate/i18n/my.po` (868 lines)
- `addons/populate/i18n/nb.po` (867 lines)
- `addons/populate/i18n/nl.po` (905 lines)
- `addons/populate/i18n/pl.po` (868 lines)
- `addons/populate/i18n/populate.pot` (862 lines)
- `addons/populate/i18n/pt.po` (867 lines)
- `addons/populate/i18n/pt_BR.po` (950 lines)
- `addons/populate/i18n/ro.po` (868 lines)
- `addons/populate/i18n/ru.po` (868 lines)
- `addons/populate/i18n/sk.po` (867 lines)
- `addons/populate/i18n/sl.po` (868 lines)
- `addons/populate/i18n/sr@latin.po` (868 lines)
- `addons/populate/i18n/sv.po` (868 lines)
- `addons/populate/i18n/th.po` (867 lines)
- `addons/populate/i18n/tr.po` (867 lines)
- `addons/populate/i18n/uk.po` (868 lines)
- `addons/populate/i18n/uz.po` (867 lines)
- `addons/populate/i18n/vi.po` (867 lines)
- `addons/populate/i18n/zh_CN.po` (904 lines)
- `addons/populate/i18n/zh_TW.po` (867 lines)
- `addons/populate/models/__init__.py` (6 lines)
- `addons/populate/models/blueprint.py` (313 lines)
- `addons/populate/models/job.py` (538 lines)
- `addons/populate/models/model_data.py` (22 lines)
- `addons/populate/models/session.py` (541 lines)
- `addons/populate/requirements.txt` (5 lines)
- `addons/populate/scripts/distributions.webp` (1,205 lines)
- `addons/populate/scripts/plot_distributions.py` (402 lines)
- `addons/populate/security/ir.access.csv` (5 lines)
- `addons/populate/utils/__init__.py` (10 lines)
- `addons/populate/utils/distributions.py` (519 lines)
- `addons/populate/utils/expression.py` (187 lines)
- `addons/populate/utils/loading.py` (72 lines)
- `addons/populate/utils/orm.py` (193 lines)
- `addons/populate/utils/populate_worker.py` (52 lines)
- `addons/populate/utils/profiling.py` (48 lines)
- `addons/populate/utils/seed.py` (19 lines)
- `addons/populate/utils/xml.py` (230 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
