# Module: l10n_do

- **Module ID:** MOD-166
- **Path:** `addons/l10n_do`
- **Manifest:** `addons/l10n_do/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.



Localization Module for Dominican Republic
===========================================

Catálogo de Cuentas e Impuestos para República Dominicana, Compatible para
**Internacionalización** con **NIIF** y alineado a las normas y regulaciones
de la Dirección General de Impuestos Internos (**DGII**).

**Este módulo consiste de:**

- Catálogo de Cuentas Estándar (alineado a DGII y NIIF)
- Catálogo de Impuestos con la mayoría de Impuestos Preconfigurados
        - ITBIS para compras y ventas
        - Retenciones de ITBIS
        - Retenciones de ISR
        - Grupos de Impuestos y Retenciones:
                - Telecomunicaiones
                - Proveedores de Materiales de Construcción
                - Personas Físicas Proveedoras de Servicios
        - Otros impuestos
- Secuencias Preconfiguradas para manejo de todos los NCF
        - Facturas con Valor Fiscal (para Ventas)
        - Facturas para Consumidores Finales
        - Notas de Débito y Crédito
        - Registro de Proveedores Informales
        - Registro de Ingreso Único
        - Registro de Gastos Menores
        - Gubernamentales
- Posiciones Fiscales para automatización de impuestos y retenciones
        - Cambios de Impuestos a Exenciones (Ej. Ventas al Estado)
        - Cambios de Impuestos a Retenciones (Ej. Compra Servicios al Exterior)
        - Entre otros

**Nota:**
Esta localización, aunque posee las secuencias para NCF, las mismas no pueden
ser utilizadas sin la instalación de módulos de terceros o desarrollo
adicional.

Estructura de Codificación del Catálogo de Cuentas:
===================================================

**Un dígito** representa la categoría/tipo de cuenta del del estado financiero.
**1** - Activo        **4** - Cuentas de Ingresos y Ganancias
**2** - Pasivo        **5** - Costos, Gastos y Pérdidas
**3** - Capital       **6** - Cuentas Liquidadoras de Resultados

**Dos dígitos** representan los rubros de agrupación:
11- Activo Corriente
21- Pasivo Corriente
31- Capital Contable

**Cuatro dígitos** se asignan a las cuentas de mayor: cuentas de primer orden
1101- Efectivo y Equivalentes de Efectivo
2101- Cuentas y Documentos por pagar
3101- Capital Social

**Seis dígitos** se asignan a las sub-cuentas: cuentas de segundo orden
110101 - Caja
210101 - Proveedores locales

**Ocho dígitos** son para las cuentas de tercer orden (las visualizadas
en Odoo):
1101- Efectivo y Equivalentes
110101- Caja
11010101 Caja General
    

Declared dependencies: `account`, `l10n_latam_invoice_document`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 8 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account",
    "l10n_latam_invoice_document"
  ],
  "data": [
    "data/account_account_tag_data.xml",
    "data/account_tax_report_data.xml",
    "data/l10n_latam_document_type_data.xml",
    "views/account_move_views.xml",
    "views/account_tax_views.xml"
  ],
  "demo": [
    "demo/demo_company.xml",
    "demo/demo_res_partner.xml",
    "demo/demo_account_journal.xml"
  ]
}
```

### Representative source files

- `addons/l10n_do/__init__.py` (4 lines)
- `addons/l10n_do/__manifest__.py` (95 lines)
- `addons/l10n_do/data/account_account_tag_data.xml` (17 lines)
- `addons/l10n_do/data/account_tax_report_data.xml` (291 lines)
- `addons/l10n_do/data/l10n_latam_document_type_data.xml` (48 lines)
- `addons/l10n_do/data/template/account.account-do.csv` (378 lines)
- `addons/l10n_do/data/template/account.fiscal.position-do.csv` (15 lines)
- `addons/l10n_do/data/template/account.tax-do.csv` (164 lines)
- `addons/l10n_do/data/template/account.tax.group-do.csv` (16 lines)
- `addons/l10n_do/demo/demo_account_journal.xml` (10 lines)
- `addons/l10n_do/demo/demo_company.xml` (36 lines)
- `addons/l10n_do/demo/demo_res_partner.xml` (15 lines)
- `addons/l10n_do/i18n/es_419.po` (418 lines)
- `addons/l10n_do/i18n/l10n_do.pot` (335 lines)
- `addons/l10n_do/models/__init__.py` (5 lines)
- `addons/l10n_do/models/account_move.py` (58 lines)
- `addons/l10n_do/models/account_tax.py` (22 lines)
- `addons/l10n_do/models/res_partner.py` (26 lines)
- `addons/l10n_do/models/template_do.py` (44 lines)
- `addons/l10n_do/tools/__init__.py` (1 lines)
- `addons/l10n_do/tools/partner_identifiers.py` (18 lines)
- `addons/l10n_do/views/account_move_views.xml` (14 lines)
- `addons/l10n_do/views/account_tax_views.xml` (14 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
