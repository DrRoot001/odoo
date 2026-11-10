# Module: sales_team

- **Module ID:** MOD-538
- **Path:** `addons/sales_team`
- **Manifest:** `addons/sales_team/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Sales Teams


Using this application you can manage Sales Teams with CRM and/or Sales
=======================================================================
 

Declared dependencies: `base`, `mail`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 8 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 4 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base",
    "mail"
  ],
  "data": [
    "security/sales_team_security.xml",
    "data/crm_team_data.xml",
    "views/crm_tag_views.xml",
    "views/crm_team_views.xml",
    "views/crm_team_member_views.xml",
    "views/mail_activity_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/crm_team_demo.xml",
    "data/crm_tag_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "sales_team/static/src/**/*"
    ],
    "web.assets_unit_tests": [
      "sales_team/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/sales_team/__init__.py` (4 lines)
- `addons/sales_team/__manifest__.py` (37 lines)
- `addons/sales_team/data/crm_tag_demo.xml` (38 lines)
- `addons/sales_team/data/crm_team_data.xml` (34 lines)
- `addons/sales_team/data/crm_team_demo.xml` (29 lines)
- `addons/sales_team/i18n/af.po` (770 lines)
- `addons/sales_team/i18n/am.po` (766 lines)
- `addons/sales_team/i18n/ar.po` (795 lines)
- `addons/sales_team/i18n/az.po` (775 lines)
- `addons/sales_team/i18n/bg.po` (796 lines)
- `addons/sales_team/i18n/bs.po` (775 lines)
- `addons/sales_team/i18n/ca.po` (817 lines)
- `addons/sales_team/i18n/cs.po` (810 lines)
- `addons/sales_team/i18n/da.po` (788 lines)
- `addons/sales_team/i18n/de.po` (827 lines)
- `addons/sales_team/i18n/el.po` (808 lines)
- `addons/sales_team/i18n/es.po` (818 lines)
- `addons/sales_team/i18n/es_419.po` (821 lines)
- `addons/sales_team/i18n/es_CL.po` (102 lines)
- `addons/sales_team/i18n/et.po` (810 lines)
- `addons/sales_team/i18n/eu.po` (768 lines)
- `addons/sales_team/i18n/fa.po` (800 lines)
- `addons/sales_team/i18n/fi.po` (832 lines)
- `addons/sales_team/i18n/fo.po` (768 lines)
- `addons/sales_team/i18n/fr.po` (815 lines)
- `addons/sales_team/i18n/fr_BE.po` (73 lines)
- `addons/sales_team/i18n/fr_CA.po` (79 lines)
- `addons/sales_team/i18n/gl.po` (768 lines)
- `addons/sales_team/i18n/gu.po` (770 lines)
- `addons/sales_team/i18n/he.po` (803 lines)
- `addons/sales_team/i18n/hi.po` (771 lines)
- `addons/sales_team/i18n/hr.po` (788 lines)
- `addons/sales_team/i18n/hu.po` (812 lines)
- `addons/sales_team/i18n/id.po` (806 lines)
- `addons/sales_team/i18n/is.po` (770 lines)
- `addons/sales_team/i18n/it.po` (811 lines)
- `addons/sales_team/i18n/ja.po` (808 lines)
- `addons/sales_team/i18n/ka.po` (768 lines)
- `addons/sales_team/i18n/kab.po` (770 lines)
- `addons/sales_team/i18n/km.po` (771 lines)
- `addons/sales_team/i18n/ko.po` (789 lines)
- `addons/sales_team/i18n/ku.po` (770 lines)
- `addons/sales_team/i18n/lb.po` (771 lines)
- `addons/sales_team/i18n/lo.po` (797 lines)
- `addons/sales_team/i18n/lt.po` (797 lines)
- `addons/sales_team/i18n/lv.po` (777 lines)
- `addons/sales_team/i18n/mk.po` (770 lines)
- `addons/sales_team/i18n/mn.po` (788 lines)
- `addons/sales_team/i18n/my.po` (771 lines)
- `addons/sales_team/i18n/nb.po` (798 lines)
- `addons/sales_team/i18n/nl.po` (822 lines)
- `addons/sales_team/i18n/pl.po` (830 lines)
- `addons/sales_team/i18n/pt.po` (813 lines)
- `addons/sales_team/i18n/pt_BR.po` (824 lines)
- `addons/sales_team/i18n/ro.po` (808 lines)
- `addons/sales_team/i18n/ru.po` (822 lines)
- `addons/sales_team/i18n/sales_team.pot` (765 lines)
- `addons/sales_team/i18n/sk.po` (787 lines)
- `addons/sales_team/i18n/sl.po` (801 lines)
- `addons/sales_team/i18n/sq.po` (768 lines)
- `addons/sales_team/i18n/sr@latin.po` (775 lines)
- `addons/sales_team/i18n/sv.po` (815 lines)
- `addons/sales_team/i18n/ta.po` (770 lines)
- `addons/sales_team/i18n/th.po` (783 lines)
- `addons/sales_team/i18n/tr.po` (817 lines)
- `addons/sales_team/i18n/uk.po` (803 lines)
- `addons/sales_team/i18n/uz.po` (927 lines)
- `addons/sales_team/i18n/vi.po` (802 lines)
- `addons/sales_team/i18n/zh_CN.po` (797 lines)
- `addons/sales_team/i18n/zh_TW.po` (779 lines)
- `addons/sales_team/models/__init__.py` (7 lines)
- `addons/sales_team/models/crm_tag.py` (21 lines)
- `addons/sales_team/models/crm_team.py` (266 lines)
- `addons/sales_team/models/crm_team_member.py` (213 lines)
- `addons/sales_team/models/res_users.py` (50 lines)
- `addons/sales_team/security/ir.access.csv` (8 lines)
- `addons/sales_team/security/sales_team_security.xml` (33 lines)
- `addons/sales_team/static/src/js/crm_team_form.js` (54 lines)
- `addons/sales_team/static/src/scss/crm_team_views.scss` (20 lines)
- `addons/sales_team/static/tests/crm_team_form.test.js` (79 lines)
- `addons/sales_team/static/tests/crm_team_test_helpers.js` (9 lines)
- `addons/sales_team/static/tests/mock_server/mock_models/crm_team.js` (21 lines)
- `addons/sales_team/tests/__init__.py` (7 lines)
- `addons/sales_team/tests/common.py` (149 lines)
- `addons/sales_team/tests/test_sales_team.py` (280 lines)
- `addons/sales_team/tests/test_sales_team_internals.py` (97 lines)
- `addons/sales_team/tests/test_sales_team_membership.py` (323 lines)
- `addons/sales_team/views/crm_tag_views.xml` (52 lines)
- `addons/sales_team/views/crm_team_member_views.xml` (170 lines)
- `addons/sales_team/views/crm_team_views.xml` (210 lines)
- `addons/sales_team/views/mail_activity_views.xml` (16 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
