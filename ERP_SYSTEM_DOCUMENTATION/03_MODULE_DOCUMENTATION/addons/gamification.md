# Module: gamification

- **Module ID:** MOD-074
- **Path:** `addons/gamification`
- **Manifest:** `addons/gamification/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Gamification process
====================
The Gamification module provides ways to evaluate and motivate the users of Odoo.

The users can be evaluated using goals and numerical objectives to reach.
**Goals** are assigned through **challenges** to evaluate and compare members of a team with each others and through time.

For non-numerical achievements, **badges** can be granted to users. From a simple "thank you" to an exceptional achievement, a badge is an easy way to exprimate gratitude to a user for their good work.

Both goals and badges are flexibles and can be adapted to a large range of modules and actions. When installed, this module creates easy goals to help new users to discover Odoo and configure their user profile.


Declared dependencies: `mail`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 19 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 10 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 19 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mail"
  ],
  "data": [
    "wizard/update_goal.xml",
    "wizard/grant_badge.xml",
    "views/res_users_views.xml",
    "views/gamification_karma_rank_views.xml",
    "views/gamification_karma_tracking_views.xml",
    "views/gamification_badge_views.xml",
    "views/gamification_badge_user_views.xml",
    "views/gamification_goal_views.xml",
    "views/gamification_goal_definition_views.xml",
    "views/gamification_challenge_views.xml",
    "views/gamification_challenge_line_views.xml",
    "views/gamification_menus.xml",
    "data/ir_cron_data.xml",
    "data/mail_template_data.xml",
    "data/gamification_badge_data.xml",
    "data/gamification_challenge_data.xml",
    "data/gamification_karma_rank_data.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/gamification_karma_rank_demo.xml",
    "data/gamification_karma_tracking_demo.xml"
  ]
}
```

### Representative source files

- `addons/gamification/__init__.py` (5 lines)
- `addons/gamification/__manifest__.py` (47 lines)
- `addons/gamification/data/gamification_badge_data.xml` (35 lines)
- `addons/gamification/data/gamification_challenge_data.xml` (96 lines)
- `addons/gamification/data/gamification_karma_rank_data.xml` (80 lines)
- `addons/gamification/data/gamification_karma_rank_demo.xml` (44 lines)
- `addons/gamification/data/gamification_karma_tracking_demo.xml` (110 lines)
- `addons/gamification/data/ir_cron_data.xml` (24 lines)
- `addons/gamification/data/mail_template_data.xml` (324 lines)
- `addons/gamification/i18n/af.po` (2,814 lines)
- `addons/gamification/i18n/am.po` (2,810 lines)
- `addons/gamification/i18n/ar.po` (3,621 lines)
- `addons/gamification/i18n/az.po` (2,822 lines)
- `addons/gamification/i18n/bg.po` (2,903 lines)
- `addons/gamification/i18n/bs.po` (2,823 lines)
- `addons/gamification/i18n/ca.po` (3,590 lines)
- `addons/gamification/i18n/cs.po` (3,665 lines)
- `addons/gamification/i18n/da.po` (2,913 lines)
- `addons/gamification/i18n/de.po` (3,832 lines)
- `addons/gamification/i18n/el.po` (2,826 lines)
- `addons/gamification/i18n/es.po` (3,800 lines)
- `addons/gamification/i18n/es_419.po` (3,797 lines)
- `addons/gamification/i18n/es_CL.po` (132 lines)
- `addons/gamification/i18n/et.po` (3,535 lines)
- `addons/gamification/i18n/eu.po` (2,813 lines)
- `addons/gamification/i18n/fa.po` (2,874 lines)
- `addons/gamification/i18n/fi.po` (3,812 lines)
- `addons/gamification/i18n/fo.po` (2,813 lines)
- `addons/gamification/i18n/fr.po` (3,809 lines)
- `addons/gamification/i18n/fr_CA.po` (126 lines)
- `addons/gamification/i18n/gamification.pot` (2,660 lines)
- `addons/gamification/i18n/gl.po` (2,813 lines)
- `addons/gamification/i18n/gu.po` (2,814 lines)
- `addons/gamification/i18n/he.po` (2,844 lines)
- `addons/gamification/i18n/hi.po` (3,543 lines)
- `addons/gamification/i18n/hr.po` (2,865 lines)
- `addons/gamification/i18n/hu.po` (2,893 lines)
- `addons/gamification/i18n/id.po` (3,770 lines)
- `addons/gamification/i18n/is.po` (2,814 lines)
- `addons/gamification/i18n/it.po` (3,812 lines)
- `addons/gamification/i18n/ja.po` (3,754 lines)
- `addons/gamification/i18n/ka.po` (2,813 lines)
- `addons/gamification/i18n/kab.po` (2,815 lines)
- `addons/gamification/i18n/km.po` (2,816 lines)
- `addons/gamification/i18n/ko.po` (3,746 lines)
- `addons/gamification/i18n/ku.po` (2,819 lines)
- `addons/gamification/i18n/lo.po` (3,739 lines)
- `addons/gamification/i18n/lt.po` (2,891 lines)
- `addons/gamification/i18n/lv.po` (2,826 lines)
- `addons/gamification/i18n/mk.po` (2,813 lines)
- `addons/gamification/i18n/mn.po` (2,879 lines)
- `addons/gamification/i18n/my.po` (2,815 lines)
- `addons/gamification/i18n/nb.po` (2,825 lines)
- `addons/gamification/i18n/nl.po` (3,783 lines)
- `addons/gamification/i18n/pl.po` (3,597 lines)
- `addons/gamification/i18n/pt.po` (3,759 lines)
- `addons/gamification/i18n/pt_BR.po` (3,795 lines)
- `addons/gamification/i18n/ro.po` (3,591 lines)
- `addons/gamification/i18n/ru.po` (3,793 lines)
- `addons/gamification/i18n/sk.po` (2,868 lines)
- `addons/gamification/i18n/sl.po` (3,560 lines)
- `addons/gamification/i18n/sq.po` (2,813 lines)
- `addons/gamification/i18n/sr@latin.po` (2,825 lines)
- `addons/gamification/i18n/sv.po` (3,583 lines)
- `addons/gamification/i18n/th.po` (3,726 lines)
- `addons/gamification/i18n/tr.po` (3,699 lines)
- `addons/gamification/i18n/uk.po` (3,544 lines)
- `addons/gamification/i18n/uz.po` (3,344 lines)
- `addons/gamification/i18n/vi.po` (3,768 lines)
- `addons/gamification/i18n/zh_CN.po` (3,725 lines)
- `addons/gamification/i18n/zh_TW.po` (3,598 lines)
- `addons/gamification/models/__init__.py` (12 lines)
- `addons/gamification/models/gamification_badge.py` (202 lines)
- `addons/gamification/models/gamification_badge_user.py` (70 lines)
- `addons/gamification/models/gamification_challenge.py` (814 lines)
- `addons/gamification/models/gamification_challenge_line.py` (28 lines)
- `addons/gamification/models/gamification_goal.py` (340 lines)
- `addons/gamification/models/gamification_goal_definition.py` (157 lines)
- `addons/gamification/models/gamification_karma_rank.py` (72 lines)
- `addons/gamification/models/gamification_karma_tracking.py` (139 lines)
- `addons/gamification/models/res_users.py` (400 lines)
- `addons/gamification/security/ir.access.csv` (25 lines)
- `addons/gamification/static/description/icon.png` (18 lines)
- `addons/gamification/static/description/icon.svg` (1 lines)
- `addons/gamification/static/description/icon_hi.png` (93 lines)
- `addons/gamification/static/img/badge_good_job-image.png` (105 lines)
- `addons/gamification/static/img/badge_hidden-image.png` (453 lines)
- `addons/gamification/static/img/badge_idea-image.png` (106 lines)
- `addons/gamification/static/img/badge_problem_solver-image.png` (191 lines)
- `addons/gamification/static/img/rank_bachelor.png` (102 lines)
- `addons/gamification/static/img/rank_bachelor_badge.svg` (1 lines)
- `addons/gamification/static/img/rank_doctor.png` (117 lines)
- `addons/gamification/static/img/rank_doctor_badge.svg` (1 lines)
- `addons/gamification/static/img/rank_master.png` (41 lines)
- `addons/gamification/static/img/rank_master_badge.svg` (1 lines)
- `addons/gamification/static/img/rank_misc_hat.png` (538 lines)
- `addons/gamification/static/img/rank_misc_mug.png` (458 lines)
- `addons/gamification/static/img/rank_misc_unicorn.png` (94 lines)
- `addons/gamification/static/img/rank_misc_wand.png` (378 lines)
- `addons/gamification/static/img/rank_misc_world.png` (417 lines)
- `addons/gamification/static/img/rank_newbie.png` (37 lines)
- `addons/gamification/static/img/rank_newbie_badge.svg` (1 lines)
- `addons/gamification/static/img/rank_student.png` (53 lines)
- `addons/gamification/static/img/rank_student_badge.svg` (1 lines)
- `addons/gamification/tests/__init__.py` (6 lines)
- `addons/gamification/tests/common.py` (20 lines)
- `addons/gamification/tests/test_challenge.py` (264 lines)
- `addons/gamification/tests/test_karma_tracking.py` (454 lines)
- `addons/gamification/views/gamification_badge_user_views.xml` (35 lines)
- `addons/gamification/views/gamification_badge_views.xml` (152 lines)
- `addons/gamification/views/gamification_challenge_line_views.xml` (15 lines)
- `addons/gamification/views/gamification_challenge_views.xml` (193 lines)
- `addons/gamification/views/gamification_goal_definition_views.xml` (99 lines)
- `addons/gamification/views/gamification_goal_views.xml` (191 lines)
- `addons/gamification/views/gamification_karma_rank_views.xml` (86 lines)
- `addons/gamification/views/gamification_karma_tracking_views.xml` (83 lines)
- `addons/gamification/views/gamification_menus.xml` (33 lines)
- `addons/gamification/views/res_users_views.xml` (37 lines)
- `addons/gamification/wizard/__init__.py` (5 lines)
- `addons/gamification/wizard/grant_badge.py` (34 lines)
- `addons/gamification/wizard/grant_badge.xml` (31 lines)
- `addons/gamification/wizard/update_goal.py` (25 lines)
- `addons/gamification/wizard/update_goal.xml` (19 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
