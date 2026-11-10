# Module: test_base

- **Module ID:** MOD-650
- **Path:** `odoo/addons/test_base`
- **Manifest:** `odoo/addons/test_base/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

A module to test the ORM.

Declared dependencies: `base`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 112 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 22 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 10 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 107 | Test files found by path/name convention. |
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
    "data/test_translated_field/test_model_data.xml",
    "data/test_access_rights_data.xml",
    "data/test_action_bindings.xml",
    "data/test_inherits.xml",
    "data/test_orm_data.xml",
    "data/test_orm_partner.xml",
    "views/test_acl.xml",
    "views/test_orm_views.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `odoo/addons/test_base/__init__.py` (1 lines)
- `odoo/addons/test_base/__manifest__.py` (22 lines)
- `odoo/addons/test_base/data/test_access_rights_data.xml` (5 lines)
- `odoo/addons/test_base/data/test_action_bindings.xml` (40 lines)
- `odoo/addons/test_base/data/test_inherits.xml` (19 lines)
- `odoo/addons/test_base/data/test_orm_data.xml` (54 lines)
- `odoo/addons/test_base/data/test_orm_partner.xml` (17 lines)
- `odoo/addons/test_base/data/test_translated_field/test_model_data.xml` (8 lines)
- `odoo/addons/test_base/data/test_translated_field/test_tools.convert.csv` (2 lines)
- `odoo/addons/test_base/i18n/fr.po` (22 lines)
- `odoo/addons/test_base/models/__init__.py` (21 lines)
- `odoo/addons/test_base/models/common.py` (192 lines)
- `odoo/addons/test_base/models/models_translation.py` (12 lines)
- `odoo/addons/test_base/models/test_access_rights.py` (83 lines)
- `odoo/addons/test_base/models/test_acl.py` (41 lines)
- `odoo/addons/test_base/models/test_action_bindings.py` (11 lines)
- `odoo/addons/test_base/models/test_config.py` (54 lines)
- `odoo/addons/test_base/models/test_convert.py` (38 lines)
- `odoo/addons/test_base/models/test_domain_expression.py` (93 lines)
- `odoo/addons/test_base/models/test_fields.py` (62 lines)
- `odoo/addons/test_base/models/test_inherits.py` (165 lines)
- `odoo/addons/test_base/models/test_ir_qweb_fields.py` (33 lines)
- `odoo/addons/test_base/models/test_orm.py` (2,462 lines)
- `odoo/addons/test_base/models/test_performance.py` (129 lines)
- `odoo/addons/test_base/models/test_properties.py` (9 lines)
- `odoo/addons/test_base/models/test_read_group.py` (282 lines)
- `odoo/addons/test_base/models/test_schema.py` (38 lines)
- `odoo/addons/test_base/models/test_search.py` (66 lines)
- `odoo/addons/test_base/models/test_tools.py` (38 lines)
- `odoo/addons/test_base/models/test_unity_read.py` (78 lines)
- `odoo/addons/test_base/security/ir.access.csv` (247 lines)
- `odoo/addons/test_base/test_file.txt` (1 lines)
- `odoo/addons/test_base/tests/__init__.py` (4 lines)
- `odoo/addons/test_base/tests/test_core/__init__.py` (8 lines)
- `odoo/addons/test_base/tests/test_core/shell_file.txt` (1 lines)
- `odoo/addons/test_base/tests/test_core/test_cli.py` (234 lines)
- `odoo/addons/test_base/tests/test_core/test_core_init.py` (60 lines)
- `odoo/addons/test_base/tests/test_core/test_monkeypatch_lxml.py` (15 lines)
- `odoo/addons/test_base/tests/test_core/test_monkeypatch_num2words.py` (35 lines)
- `odoo/addons/test_base/tests/test_core/test_monkeypatch_num2words_es.py` (84 lines)
- `odoo/addons/test_base/tests/test_core/test_monkeypatch_zoneinfo.py` (103 lines)
- `odoo/addons/test_base/tests/test_modules/__init__.py` (6 lines)
- `odoo/addons/test_base/tests/test_modules/test_install_addons/test_install_auto/__init__.py` (1 lines)
- `odoo/addons/test_base/tests/test_modules/test_install_addons/test_install_auto/__manifest__.py` (13 lines)
- `odoo/addons/test_base/tests/test_modules/test_install_addons/test_install_auto/data/ir_cron.xml` (15 lines)
- `odoo/addons/test_base/tests/test_modules/test_install_addons/test_install_auto/models/__init__.py` (1 lines)
- `odoo/addons/test_base/tests/test_modules/test_install_addons/test_install_auto/models/res_currency.py` (11 lines)
- `odoo/addons/test_base/tests/test_modules/test_install_addons/test_install_base/__init__.py` (0 lines)
- `odoo/addons/test_base/tests/test_modules/test_install_addons/test_install_base/__manifest__.py` (10 lines)
- `odoo/addons/test_base/tests/test_modules/test_install_addons/test_install_fail/__init__.py` (0 lines)
- `odoo/addons/test_base/tests/test_modules/test_install_addons/test_install_fail/__manifest__.py` (13 lines)
- `odoo/addons/test_base/tests/test_modules/test_install_addons/test_install_fail/views/res_currency_views.xml` (13 lines)
- `odoo/addons/test_base/tests/test_modules/test_install_addons/test_isolated_install.md` (19 lines)
- `odoo/addons/test_base/tests/test_modules/test_loading.py` (46 lines)
- `odoo/addons/test_base/tests/test_modules/test_manifest.py` (102 lines)
- `odoo/addons/test_base/tests/test_modules/test_module_graph.py` (135 lines)
- `odoo/addons/test_base/tests/test_modules/test_neutralize.py` (30 lines)
- `odoo/addons/test_base/tests/test_orm/__init__.py` (47 lines)
- `odoo/addons/test_base/tests/test_orm/common.py` (98 lines)
- `odoo/addons/test_base/tests/test_orm/test_access.py` (376 lines)
- `odoo/addons/test_base/tests/test_orm/test_access_feedback.py` (558 lines)
- `odoo/addons/test_base/tests/test_orm/test_access_monetary_related.py` (38 lines)
- `odoo/addons/test_base/tests/test_orm/test_acl.py` (253 lines)
- `odoo/addons/test_base/tests/test_orm/test_action_bindings.py` (97 lines)
- `odoo/addons/test_base/tests/test_orm/test_all_models.py` (102 lines)
- `odoo/addons/test_base/tests/test_orm/test_autovacuum.py` (18 lines)
- `odoo/addons/test_base/tests/test_orm/test_cache.py` (124 lines)
- `odoo/addons/test_base/tests/test_orm/test_check_access.py` (51 lines)
- `odoo/addons/test_base/tests/test_orm/test_company_checks.py` (284 lines)
- `odoo/addons/test_base/tests/test_orm/test_config_settings.py` (259 lines)
- `odoo/addons/test_base/tests/test_orm/test_copy.py` (84 lines)
- `odoo/addons/test_base/tests/test_orm/test_create.py` (23 lines)
- `odoo/addons/test_base/tests/test_orm/test_domain.py` (1,272 lines)
- `odoo/addons/test_base/tests/test_orm/test_domain_expression.py` (3,029 lines)
- `odoo/addons/test_base/tests/test_orm/test_fields.py` (5,625 lines)
- `odoo/addons/test_base/tests/test_orm/test_index_method.py` (72 lines)
- `odoo/addons/test_base/tests/test_orm/test_indexed_translation.py` (91 lines)
- `odoo/addons/test_base/tests/test_orm/test_inherits.py` (255 lines)
- `odoo/addons/test_base/tests/test_orm/test_ir_qweb_fields.py` (303 lines)
- `odoo/addons/test_base/tests/test_orm/test_ir_rules.py` (252 lines)
- `odoo/addons/test_base/tests/test_orm/test_json_field.py` (37 lines)
- `odoo/addons/test_base/tests/test_orm/test_many2many.py` (97 lines)
- `odoo/addons/test_base/tests/test_orm/test_models.py` (858 lines)
- `odoo/addons/test_base/tests/test_orm/test_modules_db.py` (170 lines)
- `odoo/addons/test_base/tests/test_orm/test_one2many.py` (469 lines)
- `odoo/addons/test_base/tests/test_orm/test_parent_store.py` (93 lines)
- `odoo/addons/test_base/tests/test_orm/test_performance.py` (855 lines)
- `odoo/addons/test_base/tests/test_orm/test_prefetch.py` (255 lines)
- `odoo/addons/test_base/tests/test_orm/test_properties.py` (2,218 lines)
- `odoo/addons/test_base/tests/test_orm/test_query.py` (188 lines)
- `odoo/addons/test_base/tests/test_orm/test_read_group_override.py` (54 lines)
- `odoo/addons/test_base/tests/test_orm/test_read_group_private.py` (1,601 lines)
- `odoo/addons/test_base/tests/test_orm/test_read_grouping_sets.py` (293 lines)
- `odoo/addons/test_base/tests/test_orm/test_registry.py` (127 lines)
- `odoo/addons/test_base/tests/test_orm/test_registry_signaling.py` (693 lines)
- `odoo/addons/test_base/tests/test_orm/test_schema.py` (508 lines)
- `odoo/addons/test_base/tests/test_orm/test_search.py` (2,470 lines)
- `odoo/addons/test_base/tests/test_orm/test_search_order.py` (277 lines)
- `odoo/addons/test_base/tests/test_orm/test_sort.py` (207 lines)
- `odoo/addons/test_base/tests/test_orm/test_timeit.py` (277 lines)
- `odoo/addons/test_base/tests/test_orm/test_transactions.py` (69 lines)
- `odoo/addons/test_base/tests/test_orm/test_uninstall.py` (85 lines)
- `odoo/addons/test_base/tests/test_orm/test_views.py` (126 lines)
- `odoo/addons/test_base/tests/test_tools/__init__.py` (24 lines)
- `odoo/addons/test_base/tests/test_tools/config/16.0.conf` (67 lines)
- `odoo/addons/test_base/tests/test_tools/config/cli` (79 lines)
- `odoo/addons/test_base/tests/test_tools/config/empty.conf` (1 lines)
- `odoo/addons/test_base/tests/test_tools/config/environ` (70 lines)
- `odoo/addons/test_base/tests/test_tools/config/multidb.conf` (2 lines)
- `odoo/addons/test_base/tests/test_tools/config/non_default.conf` (99 lines)
- `odoo/addons/test_base/tests/test_tools/config/save_posix.conf` (83 lines)
- `odoo/addons/test_base/tests/test_tools/config/sysloglogfile.conf` (3 lines)
- `odoo/addons/test_base/tests/test_tools/test_barcode.py` (27 lines)
- `odoo/addons/test_base/tests/test_tools/test_binary.py` (33 lines)
- `odoo/addons/test_base/tests/test_tools/test_cloc.py` (264 lines)
- `odoo/addons/test_base/tests/test_tools/test_config.py` (833 lines)
- `odoo/addons/test_base/tests/test_tools/test_convert.py` (481 lines)
- `odoo/addons/test_base/tests/test_tools/test_date_utils.py` (508 lines)
- `odoo/addons/test_base/tests/test_tools/test_float_utils.py` (301 lines)
- `odoo/addons/test_base/tests/test_tools/test_func.py` (210 lines)
- `odoo/addons/test_base/tests/test_tools/test_i18n.py` (36 lines)
- `odoo/addons/test_base/tests/test_tools/test_image.py` (366 lines)
- `odoo/addons/test_base/tests/test_tools/test_intervals.py` (268 lines)
- `odoo/addons/test_base/tests/test_tools/test_mail.py` (1,066 lines)
- `odoo/addons/test_base/tests/test_tools/test_mimetypes.py` (239 lines)
- `odoo/addons/test_base/tests/test_tools/test_misc.py` (857 lines)
- `odoo/addons/test_base/tests/test_tools/test_pdf.py` (598 lines)
- `odoo/addons/test_base/tests/test_tools/test_profiler.py` (832 lines)
- `odoo/addons/test_base/tests/test_tools/test_safe_eval.py` (890 lines)
- `odoo/addons/test_base/tests/test_tools/test_safe_eval_expr.py` (251 lines)
- `odoo/addons/test_base/tests/test_tools/test_set_expression.py` (474 lines)
- `odoo/addons/test_base/tests/test_tools/test_sql.py` (405 lines)
- `odoo/addons/test_base/tests/test_tools/test_translate.py` (3,097 lines)
- `odoo/addons/test_base/tests/test_tools/test_xml_utils.py` (54 lines)
- `odoo/addons/test_base/views/test_acl.xml` (18 lines)
- `odoo/addons/test_base/views/test_orm_views.xml` (524 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
