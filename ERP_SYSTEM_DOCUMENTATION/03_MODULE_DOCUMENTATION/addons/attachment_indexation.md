# Module: attachment_indexation

- **Module ID:** MOD-019
- **Path:** `addons/attachment_indexation`
- **Manifest:** `addons/attachment_indexation/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Attachments list and document indexation
========================================
* Show attachment on the top of the forms
* Document Indexation: odt, pdf, xlsx, docx

The `pdfminer.six` Python library has to be installed in order to index PDF files


Declared dependencies: `web`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
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
    "web"
  ]
}
```

### Representative source files

- `addons/attachment_indexation/__init__.py` (4 lines)
- `addons/attachment_indexation/__manifest__.py` (17 lines)
- `addons/attachment_indexation/i18n/ar.po` (57 lines)
- `addons/attachment_indexation/i18n/attachment_indexation.pot` (48 lines)
- `addons/attachment_indexation/i18n/az.po` (53 lines)
- `addons/attachment_indexation/i18n/bg.po` (53 lines)
- `addons/attachment_indexation/i18n/bs.po` (55 lines)
- `addons/attachment_indexation/i18n/ca.po` (54 lines)
- `addons/attachment_indexation/i18n/cs.po` (56 lines)
- `addons/attachment_indexation/i18n/da.po` (56 lines)
- `addons/attachment_indexation/i18n/de.po` (66 lines)
- `addons/attachment_indexation/i18n/el.po` (54 lines)
- `addons/attachment_indexation/i18n/es.po` (65 lines)
- `addons/attachment_indexation/i18n/es_419.po` (62 lines)
- `addons/attachment_indexation/i18n/et.po` (53 lines)
- `addons/attachment_indexation/i18n/fa.po` (53 lines)
- `addons/attachment_indexation/i18n/fi.po` (62 lines)
- `addons/attachment_indexation/i18n/fr.po` (65 lines)
- `addons/attachment_indexation/i18n/he.po` (57 lines)
- `addons/attachment_indexation/i18n/hi.po` (53 lines)
- `addons/attachment_indexation/i18n/hr.po` (57 lines)
- `addons/attachment_indexation/i18n/hu.po` (56 lines)
- `addons/attachment_indexation/i18n/id.po` (53 lines)
- `addons/attachment_indexation/i18n/it.po` (64 lines)
- `addons/attachment_indexation/i18n/ja.po` (62 lines)
- `addons/attachment_indexation/i18n/kab.po` (54 lines)
- `addons/attachment_indexation/i18n/ko.po` (53 lines)
- `addons/attachment_indexation/i18n/ku.po` (53 lines)
- `addons/attachment_indexation/i18n/lo.po` (52 lines)
- `addons/attachment_indexation/i18n/lt.po` (57 lines)
- `addons/attachment_indexation/i18n/lv.po` (55 lines)
- `addons/attachment_indexation/i18n/mn.po` (56 lines)
- `addons/attachment_indexation/i18n/my.po` (53 lines)
- `addons/attachment_indexation/i18n/nb.po` (56 lines)
- `addons/attachment_indexation/i18n/nl.po` (65 lines)
- `addons/attachment_indexation/i18n/pl.po` (59 lines)
- `addons/attachment_indexation/i18n/pt.po` (55 lines)
- `addons/attachment_indexation/i18n/pt_BR.po` (64 lines)
- `addons/attachment_indexation/i18n/ro.po` (56 lines)
- `addons/attachment_indexation/i18n/ru.po` (56 lines)
- `addons/attachment_indexation/i18n/sk.po` (54 lines)
- `addons/attachment_indexation/i18n/sl.po` (54 lines)
- `addons/attachment_indexation/i18n/sr@latin.po` (54 lines)
- `addons/attachment_indexation/i18n/sv.po` (54 lines)
- `addons/attachment_indexation/i18n/th.po` (53 lines)
- `addons/attachment_indexation/i18n/tr.po` (56 lines)
- `addons/attachment_indexation/i18n/uk.po` (58 lines)
- `addons/attachment_indexation/i18n/uz.po` (63 lines)
- `addons/attachment_indexation/i18n/vi.po` (56 lines)
- `addons/attachment_indexation/i18n/zh_CN.po` (56 lines)
- `addons/attachment_indexation/i18n/zh_TW.po` (55 lines)
- `addons/attachment_indexation/models/__init__.py` (4 lines)
- `addons/attachment_indexation/models/ir_attachment.py` (277 lines)
- `addons/attachment_indexation/tests/__init__.py` (3 lines)
- `addons/attachment_indexation/tests/files/test_content.pdf` (155 lines)
- `addons/attachment_indexation/tests/test_indexation.py` (72 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
