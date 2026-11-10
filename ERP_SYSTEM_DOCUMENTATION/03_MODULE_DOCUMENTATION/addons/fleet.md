# Module: fleet

- **Module ID:** MOD-072
- **Path:** `addons/fleet`
- **Manifest:** `addons/fleet/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Manage your fleet and track car costs


Vehicle, leasing, insurances, cost
==================================
With this module, Odoo helps you managing all your vehicles, the
contracts associated to those vehicle as well as services, costs
and many other features necessary to the management of your fleet
of vehicle(s)

Main Features
-------------
* Add vehicles to your fleet
* Manage contracts for vehicles
* Reminder when a contract reach its expiration date
* Add services, odometer values for all vehicles
* Show all costs associated to a vehicle or to a type of service
* Analysis graph for costs


Declared dependencies: `base`, `mail`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 30 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 15 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 15 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 8 | Test files found by path/name convention. |
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
    "security/fleet_security.xml",
    "views/fleet_vehicle_model_views.xml",
    "views/fleet_vehicle_views.xml",
    "views/fleet_vehicle_cost_views.xml",
    "views/fleet_board_view.xml",
    "views/mail_activity_views.xml",
    "views/res_config_settings_views.xml",
    "views/fleet_vehicle_odometer_report.xml",
    "views/res_partner_views.xml",
    "data/fleet_cars_data.xml",
    "data/fleet_data.xml",
    "data/mail_message_subtype_data.xml",
    "data/mail_activity_type_data.xml",
    "wizard/fleet_vehicle_send_mail_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/fleet_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "fleet/static/src/**/*"
    ],
    "web.assets_tests": [
      "fleet/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/fleet/__init__.py` (6 lines)
- `addons/fleet/__manifest__.py` (61 lines)
- `addons/fleet/data/fleet_cars_data.xml` (271 lines)
- `addons/fleet/data/fleet_data.xml` (44 lines)
- `addons/fleet/data/fleet_demo.xml` (1,042 lines)
- `addons/fleet/data/mail_activity_type_data.xml` (11 lines)
- `addons/fleet/data/mail_message_subtype_data.xml` (12 lines)
- `addons/fleet/i18n/af.po` (2,930 lines)
- `addons/fleet/i18n/am.po` (2,926 lines)
- `addons/fleet/i18n/ar.po` (2,966 lines)
- `addons/fleet/i18n/az.po` (2,962 lines)
- `addons/fleet/i18n/bg.po` (2,989 lines)
- `addons/fleet/i18n/bs.po` (2,937 lines)
- `addons/fleet/i18n/ca.po` (2,982 lines)
- `addons/fleet/i18n/cs.po` (2,966 lines)
- `addons/fleet/i18n/da.po` (2,957 lines)
- `addons/fleet/i18n/de.po` (3,014 lines)
- `addons/fleet/i18n/el.po` (2,944 lines)
- `addons/fleet/i18n/es.po` (3,004 lines)
- `addons/fleet/i18n/es_419.po` (3,014 lines)
- `addons/fleet/i18n/es_CL.po` (160 lines)
- `addons/fleet/i18n/et.po` (2,967 lines)
- `addons/fleet/i18n/eu.po` (2,929 lines)
- `addons/fleet/i18n/fa.po` (2,964 lines)
- `addons/fleet/i18n/fi.po` (3,012 lines)
- `addons/fleet/i18n/fleet.pot` (2,926 lines)
- `addons/fleet/i18n/fo.po` (2,929 lines)
- `addons/fleet/i18n/fr.po` (3,020 lines)
- `addons/fleet/i18n/fr_CA.po` (145 lines)
- `addons/fleet/i18n/gl.po` (2,929 lines)
- `addons/fleet/i18n/gu.po` (2,936 lines)
- `addons/fleet/i18n/he.po` (2,966 lines)
- `addons/fleet/i18n/hi.po` (2,963 lines)
- `addons/fleet/i18n/hr.po` (2,963 lines)
- `addons/fleet/i18n/hu.po` (2,954 lines)
- `addons/fleet/i18n/id.po` (2,983 lines)
- `addons/fleet/i18n/is.po` (2,931 lines)
- `addons/fleet/i18n/it.po` (3,014 lines)
- `addons/fleet/i18n/ja.po` (2,976 lines)
- `addons/fleet/i18n/ka.po` (2,929 lines)
- `addons/fleet/i18n/kab.po` (2,931 lines)
- `addons/fleet/i18n/km.po` (2,932 lines)
- `addons/fleet/i18n/ko.po` (2,966 lines)
- `addons/fleet/i18n/ku.po` (2,934 lines)
- `addons/fleet/i18n/lb.po` (2,931 lines)
- `addons/fleet/i18n/lo.po` (2,979 lines)
- `addons/fleet/i18n/lt.po` (2,982 lines)
- `addons/fleet/i18n/lv.po` (2,944 lines)
- `addons/fleet/i18n/mk.po` (2,929 lines)
- `addons/fleet/i18n/mn.po` (3,010 lines)
- `addons/fleet/i18n/my.po` (2,932 lines)
- `addons/fleet/i18n/nb.po` (2,943 lines)
- `addons/fleet/i18n/nl.po` (3,001 lines)
- `addons/fleet/i18n/pl.po` (2,993 lines)
- `addons/fleet/i18n/pt.po` (2,972 lines)
- `addons/fleet/i18n/pt_BR.po` (3,011 lines)
- `addons/fleet/i18n/ro.po` (2,974 lines)
- `addons/fleet/i18n/ru.po` (2,986 lines)
- `addons/fleet/i18n/sk.po` (2,960 lines)
- `addons/fleet/i18n/sl.po` (2,965 lines)
- `addons/fleet/i18n/sq.po` (2,929 lines)
- `addons/fleet/i18n/sr@latin.po` (2,944 lines)
- `addons/fleet/i18n/sv.po` (2,986 lines)
- `addons/fleet/i18n/th.po` (2,955 lines)
- `addons/fleet/i18n/tr.po` (2,989 lines)
- `addons/fleet/i18n/uk.po` (2,965 lines)
- `addons/fleet/i18n/uz.po` (3,442 lines)
- `addons/fleet/i18n/vi.po` (2,969 lines)
- `addons/fleet/i18n/zh_CN.po` (2,965 lines)
- `addons/fleet/i18n/zh_TW.po` (2,958 lines)
- `addons/fleet/models/__init__.py` (17 lines)
- `addons/fleet/models/fleet_service_type.py` (21 lines)
- `addons/fleet/models/fleet_vehicle.py` (580 lines)
- `addons/fleet/models/fleet_vehicle_assignation_log.py` (20 lines)
- `addons/fleet/models/fleet_vehicle_log_contract.py` (192 lines)
- `addons/fleet/models/fleet_vehicle_log_services.py` (85 lines)
- `addons/fleet/models/fleet_vehicle_model.py` (127 lines)
- `addons/fleet/models/fleet_vehicle_model_brand.py` (48 lines)
- `addons/fleet/models/fleet_vehicle_model_category.py` (18 lines)
- `addons/fleet/models/fleet_vehicle_odometer.py` (38 lines)
- `addons/fleet/models/fleet_vehicle_state.py` (19 lines)
- `addons/fleet/models/fleet_vehicle_tag.py` (17 lines)
- `addons/fleet/models/mail_activity_type.py` (15 lines)
- `addons/fleet/models/res_config_settings.py` (10 lines)
- `addons/fleet/models/res_partner.py` (32 lines)
- `addons/fleet/report/__init__.py` (2 lines)
- `addons/fleet/report/fleet_report.py` (164 lines)
- `addons/fleet/report/odometer_report.py` (234 lines)
- `addons/fleet/security/fleet_security.xml` (21 lines)
- `addons/fleet/security/ir.access.csv` (30 lines)
- `addons/fleet/static/description/icon.png` (44 lines)
- `addons/fleet/static/description/icon.svg` (1 lines)
- `addons/fleet/static/description/icon_hi.png` (192 lines)
- `addons/fleet/static/img/brand_abarth-image.png` (108 lines)
- `addons/fleet/static/img/brand_acura-image.png` (98 lines)
- `addons/fleet/static/img/brand_alfa-image.png` (123 lines)
- `addons/fleet/static/img/brand_audi-image.png` (86 lines)
- `addons/fleet/static/img/brand_austin-image.png` (74 lines)
- `addons/fleet/static/img/brand_bentley-image.png` (74 lines)
- `addons/fleet/static/img/brand_bmw-image.png` (75 lines)
- `addons/fleet/static/img/brand_bugatti-image.png` (112 lines)
- `addons/fleet/static/img/brand_buick-image.png` (104 lines)
- `addons/fleet/static/img/brand_byd-image.png` (95 lines)
- `addons/fleet/static/img/brand_cadillac-image.png` (104 lines)
- `addons/fleet/static/img/brand_chevrolet-image.png` (68 lines)
- `addons/fleet/static/img/brand_chrysler-image.png` (46 lines)
- `addons/fleet/static/img/brand_citroen-image.png` (76 lines)
- `addons/fleet/static/img/brand_corre-la-licorne-image.png` (146 lines)
- `addons/fleet/static/img/brand_daewoo-image.png` (88 lines)
- `addons/fleet/static/img/brand_dodge-image.png` (74 lines)
- `addons/fleet/static/img/brand_ferrari-image.png` (37 lines)
- `addons/fleet/static/img/brand_fiat-image.png` (69 lines)
- `addons/fleet/static/img/brand_ford-image.png` (90 lines)
- `addons/fleet/static/img/brand_gmc-image.png` (71 lines)
- `addons/fleet/static/img/brand_holden-image.png` (97 lines)
- `addons/fleet/static/img/brand_honda-image.png` (92 lines)
- `addons/fleet/static/img/brand_hyundai-image.png` (94 lines)
- `addons/fleet/static/img/brand_infiniti-image.png` (65 lines)
- `addons/fleet/static/img/brand_isuzu-image.png` (59 lines)
- `addons/fleet/static/img/brand_jaguar-image.png` (45 lines)
- `addons/fleet/static/img/brand_jeep-image.png` (73 lines)
- `addons/fleet/static/img/brand_kia-image.png` (99 lines)
- `addons/fleet/static/img/brand_koenigsegg-image.png` (80 lines)
- `addons/fleet/static/img/brand_lagonda-image.png` (46 lines)
- `addons/fleet/static/img/brand_lamborghini-image.png` (89 lines)
- `addons/fleet/static/img/brand_lancia-image.png` (126 lines)
- `addons/fleet/static/img/brand_land-rover-image.png` (102 lines)
- `addons/fleet/static/img/brand_lexus-image.png` (54 lines)
- `addons/fleet/static/img/brand_lincoln-image.png` (38 lines)
- `addons/fleet/static/img/brand_lotus-image.png` (139 lines)
- `addons/fleet/static/img/brand_maserati-image.png` (76 lines)
- `addons/fleet/static/img/brand_maybach-image.png` (91 lines)
- `addons/fleet/static/img/brand_mazda-image.png` (96 lines)
- `addons/fleet/static/img/brand_mercedes-image.png` (83 lines)
- `addons/fleet/static/img/brand_mg-image.png` (108 lines)
- `addons/fleet/static/img/brand_mini-image.png` (49 lines)
- `addons/fleet/static/img/brand_mitsubishi-image.png` (62 lines)
- `addons/fleet/static/img/brand_morgan-image.png` (58 lines)
- `addons/fleet/static/img/brand_nissan-image.png` (87 lines)
- `addons/fleet/static/img/brand_oldsmobile-image.png` (57 lines)
- `addons/fleet/static/img/brand_opel-image.png` (74 lines)
- `addons/fleet/static/img/brand_peugeot-image.png` (91 lines)
- `addons/fleet/static/img/brand_pontiac-image.png` (51 lines)
- `addons/fleet/static/img/brand_porsche-image.png` (56 lines)
- `addons/fleet/static/img/brand_rambler-image.png` (102 lines)
- `addons/fleet/static/img/brand_renault-image.png` (66 lines)
- `addons/fleet/static/img/brand_rolls-royce-image.png` (73 lines)
- `addons/fleet/static/img/brand_saab-image.png` (113 lines)
- `addons/fleet/static/img/brand_scion-image.png` (64 lines)
- `addons/fleet/static/img/brand_skoda-image.png` (118 lines)
- `addons/fleet/static/img/brand_smart-image.png` (55 lines)
- `addons/fleet/static/img/brand_steyr-image.png` (127 lines)
- `addons/fleet/static/img/brand_subaru-image.png` (82 lines)
- `addons/fleet/static/img/brand_suzuki-image.png` (74 lines)
- `addons/fleet/static/img/brand_tesla-motors-image.png` (88 lines)
- `addons/fleet/static/img/brand_toyota-image.png` (101 lines)
- `addons/fleet/static/img/brand_trabant-image.png` (87 lines)
- `addons/fleet/static/img/brand_volkswagen-image.png` (94 lines)
- `addons/fleet/static/img/brand_volvo-image.png` (103 lines)
- `addons/fleet/static/img/brand_willys-image.png` (95 lines)

Additional files not expanded here: 22. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
