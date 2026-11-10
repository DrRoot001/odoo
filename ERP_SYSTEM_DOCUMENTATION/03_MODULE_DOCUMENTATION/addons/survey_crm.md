# Module: survey_crm

- **Module ID:** MOD-568
- **Path:** `addons/survey_crm`
- **Manifest:** `addons/survey_crm/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Generate leads from surveys


    Bridge module between Survey and CRM.
    Enables the creation of a lead from a survey when the participant selects lead-generating answers.
    An option on the suggested answers can be activated to make them lead-generating.
    

Declared dependencies: `survey`, `crm`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 11 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 7 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "survey",
    "crm"
  ],
  "data": [
    "views/survey_question_views.xml",
    "views/survey_survey_views.xml",
    "views/survey_user_views.xml"
  ],
  "demo": [
    "demo/lead_qualification_survey_demo.xml",
    "demo/lead_qualification_answer_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "survey_crm/static/src/components/lead_generation_dropdown/crm_lead_gen_element.js"
    ]
  }
}
```

### Representative source files

- `addons/survey_crm/__init__.py` (1 lines)
- `addons/survey_crm/__manifest__.py` (28 lines)
- `addons/survey_crm/demo/lead_qualification_answer_demo.xml` (83 lines)
- `addons/survey_crm/demo/lead_qualification_survey_demo.xml` (195 lines)
- `addons/survey_crm/i18n/ar.po` (426 lines)
- `addons/survey_crm/i18n/az.po` (419 lines)
- `addons/survey_crm/i18n/bg.po` (419 lines)
- `addons/survey_crm/i18n/bs.po` (420 lines)
- `addons/survey_crm/i18n/ca.po` (419 lines)
- `addons/survey_crm/i18n/cs.po` (419 lines)
- `addons/survey_crm/i18n/da.po` (420 lines)
- `addons/survey_crm/i18n/de.po` (439 lines)
- `addons/survey_crm/i18n/el.po` (419 lines)
- `addons/survey_crm/i18n/es.po` (443 lines)
- `addons/survey_crm/i18n/es_419.po` (432 lines)
- `addons/survey_crm/i18n/et.po` (419 lines)
- `addons/survey_crm/i18n/fa.po` (419 lines)
- `addons/survey_crm/i18n/fi.po` (432 lines)
- `addons/survey_crm/i18n/fr.po` (434 lines)
- `addons/survey_crm/i18n/he.po` (420 lines)
- `addons/survey_crm/i18n/hi.po` (419 lines)
- `addons/survey_crm/i18n/hr.po` (420 lines)
- `addons/survey_crm/i18n/hu.po` (419 lines)
- `addons/survey_crm/i18n/id.po` (433 lines)
- `addons/survey_crm/i18n/it.po` (438 lines)
- `addons/survey_crm/i18n/ja.po` (432 lines)
- `addons/survey_crm/i18n/kab.po` (419 lines)
- `addons/survey_crm/i18n/ko.po` (427 lines)
- `addons/survey_crm/i18n/ku.po` (419 lines)
- `addons/survey_crm/i18n/lo.po` (428 lines)
- `addons/survey_crm/i18n/lt.po` (421 lines)
- `addons/survey_crm/i18n/lv.po` (419 lines)
- `addons/survey_crm/i18n/mn.po` (419 lines)
- `addons/survey_crm/i18n/my.po` (419 lines)
- `addons/survey_crm/i18n/nb.po` (419 lines)
- `addons/survey_crm/i18n/nl.po` (432 lines)
- `addons/survey_crm/i18n/pl.po` (435 lines)
- `addons/survey_crm/i18n/pt.po` (420 lines)
- `addons/survey_crm/i18n/pt_BR.po` (441 lines)
- `addons/survey_crm/i18n/ro.po` (420 lines)
- `addons/survey_crm/i18n/ru.po` (440 lines)
- `addons/survey_crm/i18n/sk.po` (418 lines)
- `addons/survey_crm/i18n/sl.po` (420 lines)
- `addons/survey_crm/i18n/sr@latin.po` (420 lines)
- `addons/survey_crm/i18n/survey_crm.pot` (411 lines)
- `addons/survey_crm/i18n/sv.po` (420 lines)
- `addons/survey_crm/i18n/th.po` (420 lines)
- `addons/survey_crm/i18n/tr.po` (433 lines)
- `addons/survey_crm/i18n/uk.po` (420 lines)
- `addons/survey_crm/i18n/uz.po` (507 lines)
- `addons/survey_crm/i18n/vi.po` (425 lines)
- `addons/survey_crm/i18n/zh_CN.po` (435 lines)
- `addons/survey_crm/i18n/zh_TW.po` (419 lines)
- `addons/survey_crm/models/__init__.py` (5 lines)
- `addons/survey_crm/models/survey_question.py` (16 lines)
- `addons/survey_crm/models/survey_question_answer.py` (7 lines)
- `addons/survey_crm/models/survey_survey.py` (51 lines)
- `addons/survey_crm/models/survey_user_input.py` (223 lines)
- `addons/survey_crm/models/templates/__init__.py` (1 lines)
- `addons/survey_crm/models/templates/survey_survey.py` (95 lines)
- `addons/survey_crm/static/src/components/lead_generation_dropdown/crm_lead_gen_element.js` (31 lines)
- `addons/survey_crm/static/src/img/survey_sample_lead_qualification.svg` (13 lines)
- `addons/survey_crm/tests/__init__.py` (1 lines)
- `addons/survey_crm/tests/test_survey_crm.py` (144 lines)
- `addons/survey_crm/views/survey_question_views.xml` (17 lines)
- `addons/survey_crm/views/survey_survey_views.xml` (48 lines)
- `addons/survey_crm/views/survey_user_views.xml` (25 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
