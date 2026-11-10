# Module: test_sale_product_configurators

- **Module ID:** MOD-581
- **Path:** `addons/test_sale_product_configurators`
- **Manifest:** `addons/test_sale_product_configurators/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Test Suite for Sale Product Configurator

No manifest description declared.

Declared dependencies: `event_sale`, `sale_management`, `sale_product_matrix`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 12 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "event_sale",
    "sale_management",
    "sale_product_matrix"
  ],
  "assets": {
    "web.assets_tests": [
      "test_sale_product_configurators/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/test_sale_product_configurators/__init__.py` (0 lines)
- `addons/test_sale_product_configurators/__manifest__.py` (19 lines)
- `addons/test_sale_product_configurators/static/tests/tours/event_sale_with_product_configurator_ui.js` (137 lines)
- `addons/test_sale_product_configurators/static/tests/tours/product_attribute_with_multi_type.js` (16 lines)
- `addons/test_sale_product_configurators/static/tests/tours/product_configurator_advanced_ui.js` (52 lines)
- `addons/test_sale_product_configurators/static/tests/tours/product_configurator_custom_value_update_tour.js` (25 lines)
- `addons/test_sale_product_configurators/static/tests/tours/product_configurator_edition_ui.js` (72 lines)
- `addons/test_sale_product_configurators/static/tests/tours/product_configurator_optional_products_ui.js` (67 lines)
- `addons/test_sale_product_configurators/static/tests/tours/product_configurator_pricelist_ui.js` (42 lines)
- `addons/test_sale_product_configurators/static/tests/tours/product_configurator_recursive_optional_products.js` (20 lines)
- `addons/test_sale_product_configurators/static/tests/tours/product_configurator_single_custom_attribute_ui.js` (34 lines)
- `addons/test_sale_product_configurators/static/tests/tours/product_configurator_ui.js` (75 lines)
- `addons/test_sale_product_configurators/static/tests/tours/product_configurator_uom_choice.js` (43 lines)
- `addons/test_sale_product_configurators/static/tests/tours/product_matrix_tour.js` (154 lines)
- `addons/test_sale_product_configurators/tests/__init__.py` (5 lines)
- `addons/test_sale_product_configurators/tests/test_event_sale_with_product_configurator.py` (126 lines)
- `addons/test_sale_product_configurators/tests/test_sale_product_configurator.py` (337 lines)
- `addons/test_sale_product_configurators/tests/test_sale_product_matrix.py` (77 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
