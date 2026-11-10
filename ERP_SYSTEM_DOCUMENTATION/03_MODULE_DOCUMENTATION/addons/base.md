# Module: base

- **Module ID:** MOD-648
- **Path:** `odoo/addons/base`
- **Manifest:** `odoo/addons/base/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


The kernel of Odoo, needed for all installation.
===================================================


Declared dependencies: None declared.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 107 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 52 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 88 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 42 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "data": [
    "data/res.lang.csv",
    "data/res_lang_data.xml",
    "data/res_partner_data.xml",
    "data/res_currency_data.xml",
    "data/res_company_data.xml",
    "data/res_users_data.xml",
    "data/report_paperformat_data.xml",
    "data/res_country_data.xml",
    "data/clearing_label_data.xml",
    "data/ir_demo_data.xml",
    "security/base_groups.xml",
    "wizard/wizard_ir_model_menu_create_views.xml",
    "views/decimal_precision_views.xml",
    "views/res_config_views.xml",
    "data/res.country.state.csv",
    "views/ir_actions_views.xml",
    "views/ir_asset_views.xml",
    "views/ir_config_parameter_views.xml",
    "views/ir_cron_views.xml",
    "views/ir_cron_trigger_views.xml",
    "views/ir_filters_views.xml",
    "views/ir_mail_server_views.xml",
    "views/ir_model_views.xml",
    "views/ir_attachment_views.xml",
    "views/ir_access_views.xml",
    "views/ir_sequence_views.xml",
    "views/ir_ui_menu_views.xml",
    "views/ir_ui_view_views.xml",
    "views/ir_default_views.xml",
    "data/ir_config_parameter_data.xml",
    "data/ir_cron_data.xml",
    "report/ir_model_report.xml",
    "report/ir_model_templates.xml",
    "views/ir_logging_views.xml",
    "views/ir_qweb_widget_templates.xml",
    "views/ir_module_views.xml",
    "data/ir_module_category_data.xml",
    "data/ir_module_module.xml",
    "report/ir_module_reports.xml",
    "report/ir_module_report_templates.xml",
    "wizard/base_module_update_views.xml",
    "wizard/base_language_install_views.xml",
    "wizard/base_import_language_views.xml",
    "wizard/base_module_upgrade_views.xml",
    "wizard/base_module_uninstall_views.xml",
    "wizard/base_export_language_views.xml",
    "wizard/base_partner_merge_views.xml",
    "data/ir_demo_failure_data.xml",
    "views/ir_profile_views.xml",
    "views/res_company_views.xml",
    "views/res_lang_views.xml",
    "views/res_partner_views.xml",
    "views/clearing_label_views.xml",
    "views/res_partner_bank_views.xml",
    "views/res_country_views.xml",
    "views/res_country_group_views.xml",
    "views/res_country_state_views.xml",
    "views/res_currency_views.xml",
    "views/res_groups_views.xml",
    "views/res_users_views.xml",
    "views/res_users_apikeys_views.xml",
    "views/res_device_views.xml",
    "views/res_users_identitycheck_views.xml",
    "views/res_config_settings_views.xml",
    "views/report_paperformat_views.xml",
    "data/ir_action_data.xml",
    "data/website.xml",
    "views/base_menus.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/res_users_demo.xml",
    "data/res_partner_bank_demo.xml",
    "data/res_currency_demo.xml",
    "data/res_currency_rate_demo.xml",
    "data/res_partner_demo.xml",
    "data/res_partner_image_demo.xml"
  ],
  "assets": {
    "web.assets_tests": [
      "base/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `odoo/addons/base/__init__.py` (11 lines)
- `odoo/addons/base/__manifest__.py` (100 lines)
- `odoo/addons/base/data/base_data.sql` (141 lines)
- `odoo/addons/base/data/base_data_test.sql` (21 lines)
- `odoo/addons/base/data/clearing_label_data.xml` (66 lines)
- `odoo/addons/base/data/ir_action_data.xml` (13 lines)
- `odoo/addons/base/data/ir_config_parameter_data.xml` (9 lines)
- `odoo/addons/base/data/ir_cron_data.xml` (22 lines)
- `odoo/addons/base/data/ir_demo_data.xml` (27 lines)
- `odoo/addons/base/data/ir_demo_failure_data.xml` (71 lines)
- `odoo/addons/base/data/ir_module_category_data.xml` (152 lines)
- `odoo/addons/base/data/ir_module_module.xml` (282 lines)
- `odoo/addons/base/data/neutralize.sql` (33 lines)
- `odoo/addons/base/data/report_paperformat_data.xml` (54 lines)
- `odoo/addons/base/data/res.country.state.csv` (2,131 lines)
- `odoo/addons/base/data/res.lang.csv` (94 lines)
- `odoo/addons/base/data/res_company_data.xml` (10 lines)
- `odoo/addons/base/data/res_country_data.xml` (1,790 lines)
- `odoo/addons/base/data/res_currency_data.xml` (1,900 lines)
- `odoo/addons/base/data/res_currency_demo.xml` (22 lines)
- `odoo/addons/base/data/res_currency_rate_demo.xml` (982 lines)
- `odoo/addons/base/data/res_lang_data.xml` (28 lines)
- `odoo/addons/base/data/res_partner_bank_demo.xml` (9 lines)
- `odoo/addons/base/data/res_partner_data.xml` (137 lines)
- `odoo/addons/base/data/res_partner_demo.xml` (369 lines)
- `odoo/addons/base/data/res_partner_image_demo.xml` (106 lines)
- `odoo/addons/base/data/res_users_data.xml` (39 lines)
- `odoo/addons/base/data/res_users_demo.xml` (121 lines)
- `odoo/addons/base/data/rtlcss.json` (21 lines)
- `odoo/addons/base/data/website.xml` (11 lines)
- `odoo/addons/base/i18n/af.po` (21,617 lines)
- `odoo/addons/base/i18n/am.po` (21,613 lines)
- `odoo/addons/base/i18n/ar.po` (22,468 lines)
- `odoo/addons/base/i18n/az.po` (21,991 lines)
- `odoo/addons/base/i18n/base.pot` (21,499 lines)
- `odoo/addons/base/i18n/bg.po` (21,920 lines)
- `odoo/addons/base/i18n/bs.po` (21,727 lines)
- `odoo/addons/base/i18n/ca.po` (22,197 lines)
- `odoo/addons/base/i18n/cs.po` (22,486 lines)
- `odoo/addons/base/i18n/da.po` (22,714 lines)
- `odoo/addons/base/i18n/de.po` (22,869 lines)
- `odoo/addons/base/i18n/el.po` (21,769 lines)
- `odoo/addons/base/i18n/es.po` (22,638 lines)
- `odoo/addons/base/i18n/es_419.po` (23,000 lines)
- `odoo/addons/base/i18n/es_CL.po` (763 lines)
- `odoo/addons/base/i18n/et.po` (22,102 lines)
- `odoo/addons/base/i18n/eu.po` (21,616 lines)
- `odoo/addons/base/i18n/fa.po` (21,907 lines)
- `odoo/addons/base/i18n/fi.po` (22,630 lines)
- `odoo/addons/base/i18n/fo.po` (21,616 lines)
- `odoo/addons/base/i18n/fr.po` (22,838 lines)
- `odoo/addons/base/i18n/fr_BE.po` (21,612 lines)
- `odoo/addons/base/i18n/fr_CA.po` (715 lines)
- `odoo/addons/base/i18n/gl.po` (21,616 lines)
- `odoo/addons/base/i18n/gu.po` (21,633 lines)
- `odoo/addons/base/i18n/he.po` (21,911 lines)
- `odoo/addons/base/i18n/hi.po` (21,644 lines)
- `odoo/addons/base/i18n/hr.po` (21,815 lines)
- `odoo/addons/base/i18n/hu.po` (21,927 lines)
- `odoo/addons/base/i18n/id.po` (22,912 lines)
- `odoo/addons/base/i18n/is.po` (21,832 lines)
- `odoo/addons/base/i18n/it.po` (23,025 lines)
- `odoo/addons/base/i18n/ja.po` (22,751 lines)
- `odoo/addons/base/i18n/ka.po` (21,616 lines)
- `odoo/addons/base/i18n/kab.po` (21,619 lines)
- `odoo/addons/base/i18n/km.po` (21,621 lines)
- `odoo/addons/base/i18n/ko.po` (22,272 lines)
- `odoo/addons/base/i18n/ku.po` (21,647 lines)
- `odoo/addons/base/i18n/lb.po` (21,618 lines)
- `odoo/addons/base/i18n/lo.po` (22,543 lines)
- `odoo/addons/base/i18n/lt.po` (21,809 lines)
- `odoo/addons/base/i18n/lv.po` (21,956 lines)
- `odoo/addons/base/i18n/mk.po` (21,616 lines)
- `odoo/addons/base/i18n/mn.po` (22,805 lines)
- `odoo/addons/base/i18n/my.po` (21,623 lines)
- `odoo/addons/base/i18n/nb.po` (21,733 lines)
- `odoo/addons/base/i18n/nl.po` (22,774 lines)
- `odoo/addons/base/i18n/pl.po` (22,678 lines)
- `odoo/addons/base/i18n/pt.po` (22,233 lines)
- `odoo/addons/base/i18n/pt_BR.po` (22,950 lines)
- `odoo/addons/base/i18n/ro.po` (22,463 lines)
- `odoo/addons/base/i18n/ru.po` (22,551 lines)
- `odoo/addons/base/i18n/sk.po` (21,949 lines)
- `odoo/addons/base/i18n/sl.po` (22,334 lines)
- `odoo/addons/base/i18n/sq.po` (21,616 lines)
- `odoo/addons/base/i18n/sr@latin.po` (21,652 lines)
- `odoo/addons/base/i18n/sv.po` (22,464 lines)
- `odoo/addons/base/i18n/th.po` (22,226 lines)
- `odoo/addons/base/i18n/tr.po` (22,761 lines)
- `odoo/addons/base/i18n/uk.po` (22,199 lines)
- `odoo/addons/base/i18n/uz.po` (25,547 lines)
- `odoo/addons/base/i18n/vi.po` (22,689 lines)
- `odoo/addons/base/i18n/zh_CN.po` (22,218 lines)
- `odoo/addons/base/i18n/zh_TW.po` (22,066 lines)
- `odoo/addons/base/models/__init__.py` (57 lines)
- `odoo/addons/base/models/assetsbundle.py` (1,189 lines)
- `odoo/addons/base/models/avatar_mixin.py` (104 lines)
- `odoo/addons/base/models/clearing_label.py` (21 lines)
- `odoo/addons/base/models/decimal_precision.py` (45 lines)
- `odoo/addons/base/models/image_mixin.py` (18 lines)
- `odoo/addons/base/models/ir_access.py` (540 lines)
- `odoo/addons/base/models/ir_actions.py` (1,498 lines)
- `odoo/addons/base/models/ir_actions_report.py` (926 lines)
- `odoo/addons/base/models/ir_asset.py` (423 lines)
- `odoo/addons/base/models/ir_attachment.py` (1,237 lines)
- `odoo/addons/base/models/ir_autovacuum.py` (75 lines)
- `odoo/addons/base/models/ir_binary.py` (298 lines)
- `odoo/addons/base/models/ir_config_parameter.py` (173 lines)
- `odoo/addons/base/models/ir_cron.py` (966 lines)
- `odoo/addons/base/models/ir_default.py` (250 lines)
- `odoo/addons/base/models/ir_demo.py` (19 lines)
- `odoo/addons/base/models/ir_demo_failure.py` (32 lines)
- `odoo/addons/base/models/ir_embedded_actions.py` (111 lines)
- `odoo/addons/base/models/ir_exports.py` (167 lines)
- `odoo/addons/base/models/ir_fields.py` (753 lines)
- `odoo/addons/base/models/ir_filters.py` (127 lines)
- `odoo/addons/base/models/ir_http.py` (691 lines)
- `odoo/addons/base/models/ir_logging.py` (45 lines)
- `odoo/addons/base/models/ir_mail_server.py` (965 lines)
- `odoo/addons/base/models/ir_model.py` (2,823 lines)
- `odoo/addons/base/models/ir_module.py` (1,149 lines)
- `odoo/addons/base/models/ir_profile.py` (279 lines)
- `odoo/addons/base/models/ir_profile_query.py` (68 lines)
- `odoo/addons/base/models/ir_qweb.py` (3,216 lines)
- `odoo/addons/base/models/ir_qweb_fields.py` (920 lines)
- `odoo/addons/base/models/ir_sequence.py` (394 lines)
- `odoo/addons/base/models/ir_ui_menu.py` (322 lines)
- `odoo/addons/base/models/ir_ui_view.py` (3,699 lines)
- `odoo/addons/base/models/properties_base_definition.py` (66 lines)
- `odoo/addons/base/models/properties_base_definition_mixin.py` (54 lines)
- `odoo/addons/base/models/report_layout.py` (17 lines)
- `odoo/addons/base/models/report_paperformat.py` (213 lines)
- `odoo/addons/base/models/res_company.py` (589 lines)
- `odoo/addons/base/models/res_config.py` (560 lines)
- `odoo/addons/base/models/res_country.py` (298 lines)
- `odoo/addons/base/models/res_currency.py` (546 lines)
- `odoo/addons/base/models/res_device.py` (376 lines)
- `odoo/addons/base/models/res_groups.py` (649 lines)
- `odoo/addons/base/models/res_groups_privilege.py` (15 lines)
- `odoo/addons/base/models/res_lang.py` (544 lines)
- `odoo/addons/base/models/res_partner.py` (2,463 lines)
- `odoo/addons/base/models/res_partner_bank.py` (254 lines)
- `odoo/addons/base/models/res_users.py` (1,963 lines)
- `odoo/addons/base/models/res_users_deletion.py` (100 lines)
- `odoo/addons/base/models/res_users_settings.py` (55 lines)
- `odoo/addons/base/models/website.py` (66 lines)
- `odoo/addons/base/populate/common.xml` (32 lines)
- `odoo/addons/base/report/__init__.py` (4 lines)
- `odoo/addons/base/report/corporate_defaults.xsl` (94 lines)
- `odoo/addons/base/report/custom_default_printscreen.xsl` (20 lines)
- `odoo/addons/base/report/custom_new.xsl` (177 lines)
- `odoo/addons/base/report/custom_rml_printscreen.xsl` (29 lines)
- `odoo/addons/base/report/ir_model_report.xml` (12 lines)
- `odoo/addons/base/report/ir_model_templates.xml` (103 lines)
- `odoo/addons/base/report/ir_module_report_templates.xml` (68 lines)
- `odoo/addons/base/report/ir_module_reports.xml` (15 lines)
- `odoo/addons/base/report/mako_footer.html` (23 lines)
- `odoo/addons/base/report/mako_header.html` (62 lines)
- `odoo/addons/base/report/mako_template.css` (16 lines)
- `odoo/addons/base/report/report_base_report_irmodulereference.py` (46 lines)

Additional files not expanded here: 501. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
