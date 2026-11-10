# Module: product_email_template

- **Module ID:** MOD-471
- **Path:** `addons/product_email_template`
- **Manifest:** `addons/product_email_template/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Add email templates to products to be sent on invoice confirmation
==================================================================

With this module, link your products to a template to send complete information and tools to your customer.
For instance when invoicing a training, the training agenda and materials will automatically be sent to your customers.'
    

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account"
  ],
  "data": [
    "views/product_views.xml",
    "views/mail_template_views.xml"
  ]
}
```

### Representative source files

- `addons/product_email_template/__init__.py` (3 lines)
- `addons/product_email_template/__manifest__.py` (19 lines)
- `addons/product_email_template/i18n/af.po` (88 lines)
- `addons/product_email_template/i18n/ar.po` (98 lines)
- `addons/product_email_template/i18n/az.po` (95 lines)
- `addons/product_email_template/i18n/bg.po` (100 lines)
- `addons/product_email_template/i18n/bs.po` (95 lines)
- `addons/product_email_template/i18n/ca.po` (102 lines)
- `addons/product_email_template/i18n/cs.po` (99 lines)
- `addons/product_email_template/i18n/da.po` (99 lines)
- `addons/product_email_template/i18n/de.po` (111 lines)
- `addons/product_email_template/i18n/el.po` (100 lines)
- `addons/product_email_template/i18n/es.po` (111 lines)
- `addons/product_email_template/i18n/es_419.po` (106 lines)
- `addons/product_email_template/i18n/es_CL.po` (24 lines)
- `addons/product_email_template/i18n/et.po` (101 lines)
- `addons/product_email_template/i18n/eu.po` (90 lines)
- `addons/product_email_template/i18n/fa.po` (97 lines)
- `addons/product_email_template/i18n/fi.po` (104 lines)
- `addons/product_email_template/i18n/fr.po` (101 lines)
- `addons/product_email_template/i18n/gl.po` (90 lines)
- `addons/product_email_template/i18n/gu.po` (92 lines)
- `addons/product_email_template/i18n/he.po` (100 lines)
- `addons/product_email_template/i18n/hi.po` (93 lines)
- `addons/product_email_template/i18n/hr.po` (100 lines)
- `addons/product_email_template/i18n/hu.po` (100 lines)
- `addons/product_email_template/i18n/id.po` (98 lines)
- `addons/product_email_template/i18n/is.po` (92 lines)
- `addons/product_email_template/i18n/it.po` (110 lines)
- `addons/product_email_template/i18n/ja.po` (99 lines)
- `addons/product_email_template/i18n/ka.po` (90 lines)
- `addons/product_email_template/i18n/kab.po` (92 lines)
- `addons/product_email_template/i18n/kk.po` (90 lines)
- `addons/product_email_template/i18n/ko.po` (98 lines)
- `addons/product_email_template/i18n/ku.po` (92 lines)
- `addons/product_email_template/i18n/lo.po` (91 lines)
- `addons/product_email_template/i18n/lt.po` (104 lines)
- `addons/product_email_template/i18n/lv.po` (97 lines)
- `addons/product_email_template/i18n/mk.po` (91 lines)
- `addons/product_email_template/i18n/mn.po` (100 lines)
- `addons/product_email_template/i18n/my.po` (92 lines)
- `addons/product_email_template/i18n/nb.po` (95 lines)
- `addons/product_email_template/i18n/nl.po` (112 lines)
- `addons/product_email_template/i18n/pl.po` (103 lines)
- `addons/product_email_template/i18n/product_email_template.pot` (86 lines)
- `addons/product_email_template/i18n/pt.po` (105 lines)
- `addons/product_email_template/i18n/pt_BR.po` (110 lines)
- `addons/product_email_template/i18n/ro.po` (111 lines)
- `addons/product_email_template/i18n/ru.po` (110 lines)
- `addons/product_email_template/i18n/sk.po` (100 lines)
- `addons/product_email_template/i18n/sl.po` (97 lines)
- `addons/product_email_template/i18n/sr@latin.po` (96 lines)
- `addons/product_email_template/i18n/sv.po` (103 lines)
- `addons/product_email_template/i18n/th.po` (98 lines)
- `addons/product_email_template/i18n/tr.po` (103 lines)
- `addons/product_email_template/i18n/uk.po` (103 lines)
- `addons/product_email_template/i18n/uz.po` (113 lines)
- `addons/product_email_template/i18n/vi.po` (98 lines)
- `addons/product_email_template/i18n/zh_CN.po` (104 lines)
- `addons/product_email_template/i18n/zh_TW.po` (97 lines)
- `addons/product_email_template/models/__init__.py` (4 lines)
- `addons/product_email_template/models/account_move.py` (29 lines)
- `addons/product_email_template/models/product.py` (16 lines)
- `addons/product_email_template/static/img/online_training.png` (90 lines)
- `addons/product_email_template/tests/__init__.py` (3 lines)
- `addons/product_email_template/tests/test_account_move.py` (64 lines)
- `addons/product_email_template/views/mail_template_views.xml` (21 lines)
- `addons/product_email_template/views/product_views.xml` (25 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
