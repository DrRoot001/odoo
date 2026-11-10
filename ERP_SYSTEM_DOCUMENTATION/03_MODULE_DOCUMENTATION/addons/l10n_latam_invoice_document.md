# Module: l10n_latam_invoice_document

- **Module ID:** MOD-260
- **Path:** `addons/l10n_latam_invoice_document`
- **Manifest:** `addons/l10n_latam_invoice_document/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

LATAM Document Types


Functional
----------

In some Latinamerica countries, including Argentina and Chile, some accounting transactions like invoices and vendor bills are classified by a document types defined by the government fiscal authorities (In Argentina case ARCA, Chile case SII).

This module is intended to be extended by localizations in order to manage these document types and is an essential information that needs to be displayed in the printed reports and that needs to be easily identified, within the set of invoices as well of account moves.

Each document type have their own rules and sequence number, this last one is integrated with the invoice number and journal sequence in order to be easy for the localization user. In order to support or not this document types a Journal has a new option that lets to use document or not.

Technical
---------

If your localization needs this logic will then need to add this module as dependency and in your localization module extend:

* extend company's _localization_use_documents() method.
* create the data of the document types that exists for the specific country. The document type has a country field



Declared dependencies: `account`, `account_debit_note`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 15 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 7 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 7 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account",
    "account_debit_note"
  ],
  "data": [
    "views/account_journal_view.xml",
    "views/account_move_line_view.xml",
    "views/account_move_view.xml",
    "views/l10n_latam_document_type_view.xml",
    "views/report_templates.xml",
    "report/invoice_report_view.xml",
    "wizards/account_move_reversal_view.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/l10n_latam_invoice_document/__init__.py` (4 lines)
- `addons/l10n_latam_invoice_document/__manifest__.py` (42 lines)
- `addons/l10n_latam_invoice_document/i18n/es_419.po` (466 lines)
- `addons/l10n_latam_invoice_document/i18n/l10n_latam_invoice_document.pot` (400 lines)
- `addons/l10n_latam_invoice_document/i18n/pt_BR.po` (465 lines)
- `addons/l10n_latam_invoice_document/migrations/1.1/post-migration.py` (8 lines)
- `addons/l10n_latam_invoice_document/models/__init__.py` (8 lines)
- `addons/l10n_latam_invoice_document/models/account_chart_template.py` (16 lines)
- `addons/l10n_latam_invoice_document/models/account_journal.py` (51 lines)
- `addons/l10n_latam_invoice_document/models/account_move.py` (249 lines)
- `addons/l10n_latam_invoice_document/models/account_move_line.py` (13 lines)
- `addons/l10n_latam_invoice_document/models/l10n_latam_document_type.py` (43 lines)
- `addons/l10n_latam_invoice_document/models/res_company.py` (11 lines)
- `addons/l10n_latam_invoice_document/report/__init__.py` (3 lines)
- `addons/l10n_latam_invoice_document/report/invoice_report.py` (11 lines)
- `addons/l10n_latam_invoice_document/report/invoice_report_view.xml` (18 lines)
- `addons/l10n_latam_invoice_document/security/ir.access.csv` (3 lines)
- `addons/l10n_latam_invoice_document/views/account_journal_view.xml` (22 lines)
- `addons/l10n_latam_invoice_document/views/account_move_line_view.xml` (18 lines)
- `addons/l10n_latam_invoice_document/views/account_move_view.xml` (64 lines)
- `addons/l10n_latam_invoice_document/views/l10n_latam_document_type_view.xml` (65 lines)
- `addons/l10n_latam_invoice_document/views/report_templates.xml` (113 lines)
- `addons/l10n_latam_invoice_document/wizards/__init__.py` (4 lines)
- `addons/l10n_latam_invoice_document/wizards/account_debit_note.py` (21 lines)
- `addons/l10n_latam_invoice_document/wizards/account_move_reversal.py` (86 lines)
- `addons/l10n_latam_invoice_document/wizards/account_move_reversal_view.xml` (21 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
