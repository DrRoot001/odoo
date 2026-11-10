# Module: mass_mailing_sale

- **Module ID:** MOD-369
- **Path:** `addons/mass_mailing_sale`
- **Manifest:** `addons/mass_mailing_sale/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Add sale order UTM info on mass mailing

UTM and mass mailing on sale orders

Declared dependencies: `sale`, `mass_mailing`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sale",
    "mass_mailing"
  ],
  "data": [
    "views/mailing_mailing_views.xml"
  ],
  "demo": [
    "demo/mailing_mailing.xml"
  ],
  "assets": {
    "mass_mailing.assets_builder": [
      "mass_mailing_sale/static/src/builder/**/*",
      "mass_mailing_sale/static/src/snippets/**/*"
    ]
  }
}
```

### Representative source files

- `addons/mass_mailing_sale/__init__.py` (4 lines)
- `addons/mass_mailing_sale/__manifest__.py` (24 lines)
- `addons/mass_mailing_sale/demo/mailing_mailing.xml` (8 lines)
- `addons/mass_mailing_sale/i18n/ar.po` (191 lines)
- `addons/mass_mailing_sale/i18n/az.po` (188 lines)
- `addons/mass_mailing_sale/i18n/bg.po` (185 lines)
- `addons/mass_mailing_sale/i18n/bs.po` (187 lines)
- `addons/mass_mailing_sale/i18n/ca.po` (202 lines)
- `addons/mass_mailing_sale/i18n/cs.po` (190 lines)
- `addons/mass_mailing_sale/i18n/da.po` (189 lines)
- `addons/mass_mailing_sale/i18n/de.po` (197 lines)
- `addons/mass_mailing_sale/i18n/el.po` (189 lines)
- `addons/mass_mailing_sale/i18n/es.po` (195 lines)
- `addons/mass_mailing_sale/i18n/es_419.po` (193 lines)
- `addons/mass_mailing_sale/i18n/et.po` (195 lines)
- `addons/mass_mailing_sale/i18n/fa.po` (191 lines)
- `addons/mass_mailing_sale/i18n/fi.po` (194 lines)
- `addons/mass_mailing_sale/i18n/fr.po` (199 lines)
- `addons/mass_mailing_sale/i18n/gu.po` (185 lines)
- `addons/mass_mailing_sale/i18n/he.po` (193 lines)
- `addons/mass_mailing_sale/i18n/hi.po` (185 lines)
- `addons/mass_mailing_sale/i18n/hr.po` (190 lines)
- `addons/mass_mailing_sale/i18n/hu.po` (193 lines)
- `addons/mass_mailing_sale/i18n/id.po` (192 lines)
- `addons/mass_mailing_sale/i18n/is.po` (181 lines)
- `addons/mass_mailing_sale/i18n/it.po` (198 lines)
- `addons/mass_mailing_sale/i18n/ja.po` (194 lines)
- `addons/mass_mailing_sale/i18n/kab.po` (185 lines)
- `addons/mass_mailing_sale/i18n/ko.po` (192 lines)
- `addons/mass_mailing_sale/i18n/ku.po` (185 lines)
- `addons/mass_mailing_sale/i18n/lo.po` (187 lines)
- `addons/mass_mailing_sale/i18n/lt.po` (191 lines)
- `addons/mass_mailing_sale/i18n/lv.po` (185 lines)
- `addons/mass_mailing_sale/i18n/mass_mailing_sale.pot` (181 lines)
- `addons/mass_mailing_sale/i18n/mn.po` (190 lines)
- `addons/mass_mailing_sale/i18n/my.po` (185 lines)
- `addons/mass_mailing_sale/i18n/nb.po` (189 lines)
- `addons/mass_mailing_sale/i18n/nl.po` (195 lines)
- `addons/mass_mailing_sale/i18n/pl.po` (197 lines)
- `addons/mass_mailing_sale/i18n/pt.po` (197 lines)
- `addons/mass_mailing_sale/i18n/pt_BR.po` (200 lines)
- `addons/mass_mailing_sale/i18n/ro.po` (195 lines)
- `addons/mass_mailing_sale/i18n/ru.po` (192 lines)
- `addons/mass_mailing_sale/i18n/sk.po` (189 lines)
- `addons/mass_mailing_sale/i18n/sl.po` (187 lines)
- `addons/mass_mailing_sale/i18n/sr@latin.po` (189 lines)
- `addons/mass_mailing_sale/i18n/sv.po` (189 lines)
- `addons/mass_mailing_sale/i18n/th.po` (192 lines)
- `addons/mass_mailing_sale/i18n/tr.po` (196 lines)
- `addons/mass_mailing_sale/i18n/uk.po` (194 lines)
- `addons/mass_mailing_sale/i18n/uz.po` (215 lines)
- `addons/mass_mailing_sale/i18n/vi.po` (190 lines)
- `addons/mass_mailing_sale/i18n/zh_CN.po` (193 lines)
- `addons/mass_mailing_sale/i18n/zh_TW.po` (190 lines)
- `addons/mass_mailing_sale/models/__init__.py` (6 lines)
- `addons/mass_mailing_sale/models/mailing_mailing.py` (137 lines)
- `addons/mass_mailing_sale/models/sale_order.py` (13 lines)
- `addons/mass_mailing_sale/models/utm.py` (13 lines)
- `addons/mass_mailing_sale/static/src/builder/options/product_snapshot_fragments.xml` (80 lines)
- `addons/mass_mailing_sale/static/src/builder/options/product_snapshot_snippet_info.js` (31 lines)
- `addons/mass_mailing_sale/static/src/snippets/s_product_snapshot.xml` (65 lines)
- `addons/mass_mailing_sale/static/src/snippets/snippet_categories.xml` (9 lines)
- `addons/mass_mailing_sale/views/mailing_mailing_views.xml` (32 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
