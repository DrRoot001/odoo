# Module: link_tracker

- **Module ID:** MOD-348
- **Path:** `addons/link_tracker`
- **Manifest:** `addons/link_tracker/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Shorten URLs and use them to track clicks and UTMs


Declared dependencies: `utm`, `mail`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 15 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "utm",
    "mail"
  ],
  "data": [
    "views/link_tracker_views.xml",
    "views/utm_campaign_views.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/link_tracker/__init__.py` (6 lines)
- `addons/link_tracker/__manifest__.py` (18 lines)
- `addons/link_tracker/controller/__init__.py` (4 lines)
- `addons/link_tracker/controller/main.py` (25 lines)
- `addons/link_tracker/i18n/af.po` (382 lines)
- `addons/link_tracker/i18n/ar.po` (403 lines)
- `addons/link_tracker/i18n/az.po` (392 lines)
- `addons/link_tracker/i18n/bg.po` (390 lines)
- `addons/link_tracker/i18n/bs.po` (387 lines)
- `addons/link_tracker/i18n/ca.po` (408 lines)
- `addons/link_tracker/i18n/cs.po` (398 lines)
- `addons/link_tracker/i18n/da.po` (399 lines)
- `addons/link_tracker/i18n/de.po` (412 lines)
- `addons/link_tracker/i18n/el.po` (387 lines)
- `addons/link_tracker/i18n/es.po` (406 lines)
- `addons/link_tracker/i18n/es_419.po` (408 lines)
- `addons/link_tracker/i18n/es_CL.po` (66 lines)
- `addons/link_tracker/i18n/et.po` (397 lines)
- `addons/link_tracker/i18n/eu.po` (381 lines)
- `addons/link_tracker/i18n/fa.po` (390 lines)
- `addons/link_tracker/i18n/fi.po` (413 lines)
- `addons/link_tracker/i18n/fo.po` (381 lines)
- `addons/link_tracker/i18n/fr.po` (407 lines)
- `addons/link_tracker/i18n/fr_BE.po` (56 lines)
- `addons/link_tracker/i18n/fr_CA.po` (66 lines)
- `addons/link_tracker/i18n/gl.po` (381 lines)
- `addons/link_tracker/i18n/gu.po` (382 lines)
- `addons/link_tracker/i18n/he.po` (395 lines)
- `addons/link_tracker/i18n/hi.po` (381 lines)
- `addons/link_tracker/i18n/hr.po` (393 lines)
- `addons/link_tracker/i18n/hu.po` (395 lines)
- `addons/link_tracker/i18n/id.po` (403 lines)
- `addons/link_tracker/i18n/is.po` (378 lines)
- `addons/link_tracker/i18n/it.po` (407 lines)
- `addons/link_tracker/i18n/ja.po` (405 lines)
- `addons/link_tracker/i18n/ka.po` (381 lines)
- `addons/link_tracker/i18n/kab.po` (383 lines)
- `addons/link_tracker/i18n/km.po` (382 lines)
- `addons/link_tracker/i18n/ko.po` (399 lines)
- `addons/link_tracker/i18n/ku.po` (381 lines)
- `addons/link_tracker/i18n/link_tracker.pot` (377 lines)
- `addons/link_tracker/i18n/lo.po` (393 lines)
- `addons/link_tracker/i18n/lt.po` (398 lines)
- `addons/link_tracker/i18n/lv.po` (388 lines)
- `addons/link_tracker/i18n/mk.po` (381 lines)
- `addons/link_tracker/i18n/ml_IN.po` (381 lines)
- `addons/link_tracker/i18n/mn.po` (395 lines)
- `addons/link_tracker/i18n/my.po` (382 lines)
- `addons/link_tracker/i18n/nb.po` (393 lines)
- `addons/link_tracker/i18n/nl.po` (405 lines)
- `addons/link_tracker/i18n/pl.po` (410 lines)
- `addons/link_tracker/i18n/pt.po` (406 lines)
- `addons/link_tracker/i18n/pt_BR.po` (412 lines)
- `addons/link_tracker/i18n/ro.po` (395 lines)
- `addons/link_tracker/i18n/ru.po` (402 lines)
- `addons/link_tracker/i18n/sk.po` (398 lines)
- `addons/link_tracker/i18n/sl.po` (406 lines)
- `addons/link_tracker/i18n/sq.po` (381 lines)
- `addons/link_tracker/i18n/sr@latin.po` (390 lines)
- `addons/link_tracker/i18n/sv.po` (408 lines)
- `addons/link_tracker/i18n/ta.po` (382 lines)
- `addons/link_tracker/i18n/th.po` (395 lines)
- `addons/link_tracker/i18n/tr.po` (414 lines)
- `addons/link_tracker/i18n/uk.po` (395 lines)
- `addons/link_tracker/i18n/uz.po` (452 lines)
- `addons/link_tracker/i18n/vi.po` (403 lines)
- `addons/link_tracker/i18n/zh_CN.po` (401 lines)
- `addons/link_tracker/i18n/zh_TW.po` (394 lines)
- `addons/link_tracker/models/__init__.py` (6 lines)
- `addons/link_tracker/models/link_tracker.py` (403 lines)
- `addons/link_tracker/models/mail_render_mixin.py` (102 lines)
- `addons/link_tracker/models/utm.py` (21 lines)
- `addons/link_tracker/security/ir.access.csv` (7 lines)
- `addons/link_tracker/tests/__init__.py` (7 lines)
- `addons/link_tracker/tests/common.py` (92 lines)
- `addons/link_tracker/tests/test_link_tracker.py` (364 lines)
- `addons/link_tracker/tests/test_mail_render_mixin.py` (287 lines)
- `addons/link_tracker/tests/test_tracker_http_requests.py` (47 lines)
- `addons/link_tracker/tools/__init__.py` (3 lines)
- `addons/link_tracker/tools/html.py` (64 lines)
- `addons/link_tracker/views/link_tracker_views.xml` (207 lines)
- `addons/link_tracker/views/utm_campaign_views.xml` (34 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
