# Module: auth_passkey

- **Module ID:** MOD-022
- **Path:** `addons/auth_passkey`
- **Manifest:** `addons/auth_passkey/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Log in with a Passkey


The implementation of Passkeys using the webauthn protocol.
===========================================================

Passkeys are a secure alternative to a username and a password.
When a user logs in with a Passkey, MFA will not be required.


Declared dependencies: `base_setup`, `web`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 61 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 9 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 2 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base_setup",
    "web"
  ],
  "data": [
    "views/auth_passkey_key_views.xml",
    "views/auth_passkey_login_templates.xml",
    "views/res_users_identitycheck_views.xml",
    "views/res_users_views.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "auth_passkey/static/lib/simplewebauthn.js",
      "auth_passkey/static/src/services/check_identity/*",
      "auth_passkey/static/src/views/*",
      "auth_passkey/static/src/scss/res_users.scss"
    ],
    "web.assets_frontend": [
      "auth_passkey/static/lib/simplewebauthn.js",
      "auth_passkey/static/src/interactions/*",
      "auth_passkey/static/src/services/check_identity/*"
    ],
    "web.assets_tests": [
      "auth_passkey/static/tests/*.js"
    ]
  }
}
```

### Representative source files

- `addons/auth_passkey/__init__.py` (2 lines)
- `addons/auth_passkey/__manifest__.py` (40 lines)
- `addons/auth_passkey/_vendor/webauthn/INFO` (6 lines)
- `addons/auth_passkey/_vendor/webauthn/LICENSE` (26 lines)
- `addons/auth_passkey/_vendor/webauthn/__init__.py` (20 lines)
- `addons/auth_passkey/_vendor/webauthn/authentication/__init__.py` (0 lines)
- `addons/auth_passkey/_vendor/webauthn/authentication/generate_authentication_options.py` (51 lines)
- `addons/auth_passkey/_vendor/webauthn/authentication/verify_authentication_response.py` (183 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/__init__.py` (45 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/aaguid_to_string.py` (27 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/algorithms.py` (91 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/asn1/__init__.py` (0 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/asn1/android_key.py` (131 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/base64url_to_bytes.py` (12 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/bytes_to_base64url.py` (8 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/byteslike_to_bytes.py` (11 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/cose.py` (79 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/decode_credential_public_key.py` (120 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/decoded_public_key_to_cryptography.py` (66 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/encode_cbor.py` (20 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/exceptions.py` (58 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/generate_challenge.py` (12 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/generate_user_handle.py` (17 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/hash_by_alg.py` (41 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/known_root_certs.py` (199 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/options_to_json.py` (124 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/parse_attestation_object.py` (24 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/parse_attestation_statement.py` (26 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/parse_authentication_credential_json.py` (100 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/parse_authenticator_data.py` (106 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/parse_backup_flags.py` (34 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/parse_cbor.py` (20 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/parse_client_data_json.py` (65 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/parse_registration_credential_json.py` (97 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/pem_cert_bytes_to_open_ssl_x509.py` (12 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/snake_case_to_camel_case.py` (14 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/structs.py` (534 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/tpm/__init__.py` (4 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/tpm/parse_cert_info.py` (74 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/tpm/parse_pub_area.py` (60 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/tpm/structs.py` (409 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/validate_certificate_chain.py` (74 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/verify_safetynet_timestamp.py` (19 lines)
- `addons/auth_passkey/_vendor/webauthn/helpers/verify_signature.py` (72 lines)
- `addons/auth_passkey/_vendor/webauthn/py.typed` (0 lines)
- `addons/auth_passkey/_vendor/webauthn/registration/__init__.py` (0 lines)
- `addons/auth_passkey/_vendor/webauthn/registration/formats/__init__.py` (0 lines)
- `addons/auth_passkey/_vendor/webauthn/registration/formats/android_key.py` (185 lines)
- `addons/auth_passkey/_vendor/webauthn/registration/formats/android_safetynet.py` (198 lines)
- `addons/auth_passkey/_vendor/webauthn/registration/formats/apple.py` (123 lines)
- `addons/auth_passkey/_vendor/webauthn/registration/formats/fido_u2f.py` (128 lines)
- `addons/auth_passkey/_vendor/webauthn/registration/formats/packed.py` (106 lines)
- `addons/auth_passkey/_vendor/webauthn/registration/formats/tpm.py` (309 lines)
- `addons/auth_passkey/_vendor/webauthn/registration/generate_registration_options.py` (141 lines)
- `addons/auth_passkey/_vendor/webauthn/registration/verify_registration_response.py` (288 lines)
- `addons/auth_passkey/controllers/__init__.py` (1 lines)
- `addons/auth_passkey/controllers/main.py` (20 lines)
- `addons/auth_passkey/i18n/ar.po` (270 lines)
- `addons/auth_passkey/i18n/auth_passkey.pot` (262 lines)
- `addons/auth_passkey/i18n/az.po` (266 lines)
- `addons/auth_passkey/i18n/bg.po` (266 lines)
- `addons/auth_passkey/i18n/bs.po` (268 lines)
- `addons/auth_passkey/i18n/ca.po` (269 lines)
- `addons/auth_passkey/i18n/cs.po` (272 lines)
- `addons/auth_passkey/i18n/da.po` (273 lines)
- `addons/auth_passkey/i18n/de.po` (281 lines)
- `addons/auth_passkey/i18n/el.po` (266 lines)
- `addons/auth_passkey/i18n/es.po` (279 lines)
- `addons/auth_passkey/i18n/es_419.po` (280 lines)
- `addons/auth_passkey/i18n/et.po` (268 lines)
- `addons/auth_passkey/i18n/fa.po` (266 lines)
- `addons/auth_passkey/i18n/fi.po` (279 lines)
- `addons/auth_passkey/i18n/fr.po` (281 lines)
- `addons/auth_passkey/i18n/he.po` (267 lines)
- `addons/auth_passkey/i18n/hi.po` (266 lines)
- `addons/auth_passkey/i18n/hr.po` (272 lines)
- `addons/auth_passkey/i18n/hu.po` (266 lines)
- `addons/auth_passkey/i18n/id.po` (273 lines)
- `addons/auth_passkey/i18n/it.po` (281 lines)
- `addons/auth_passkey/i18n/ja.po` (279 lines)
- `addons/auth_passkey/i18n/kab.po` (267 lines)
- `addons/auth_passkey/i18n/ko.po` (272 lines)
- `addons/auth_passkey/i18n/ku.po` (266 lines)
- `addons/auth_passkey/i18n/lo.po` (276 lines)
- `addons/auth_passkey/i18n/lt.po` (268 lines)
- `addons/auth_passkey/i18n/lv.po` (268 lines)
- `addons/auth_passkey/i18n/mn.po` (266 lines)
- `addons/auth_passkey/i18n/my.po` (267 lines)
- `addons/auth_passkey/i18n/nb.po` (266 lines)
- `addons/auth_passkey/i18n/nl.po` (280 lines)
- `addons/auth_passkey/i18n/pl.po` (273 lines)
- `addons/auth_passkey/i18n/pt.po` (269 lines)
- `addons/auth_passkey/i18n/pt_BR.po` (278 lines)
- `addons/auth_passkey/i18n/ro.po` (273 lines)
- `addons/auth_passkey/i18n/ru.po` (274 lines)
- `addons/auth_passkey/i18n/sk.po` (267 lines)
- `addons/auth_passkey/i18n/sl.po` (269 lines)
- `addons/auth_passkey/i18n/sr@latin.po` (267 lines)
- `addons/auth_passkey/i18n/sv.po` (273 lines)
- `addons/auth_passkey/i18n/th.po` (270 lines)
- `addons/auth_passkey/i18n/tr.po` (275 lines)
- `addons/auth_passkey/i18n/uk.po` (269 lines)
- `addons/auth_passkey/i18n/uz.po` (315 lines)
- `addons/auth_passkey/i18n/vi.po` (268 lines)
- `addons/auth_passkey/i18n/zh_CN.po` (270 lines)
- `addons/auth_passkey/i18n/zh_TW.po` (273 lines)
- `addons/auth_passkey/mobile_utils.py` (36 lines)
- `addons/auth_passkey/models/__init__.py` (3 lines)
- `addons/auth_passkey/models/auth_passkey_key.py` (193 lines)
- `addons/auth_passkey/models/res_users.py` (88 lines)
- `addons/auth_passkey/models/res_users_identitycheck.py` (41 lines)
- `addons/auth_passkey/security/ir.access.csv` (7 lines)
- `addons/auth_passkey/static/lib/simplewebauthn.js` (396 lines)
- `addons/auth_passkey/static/src/interactions/passkey_login.js` (28 lines)
- `addons/auth_passkey/static/src/scss/res_users.scss` (5 lines)
- `addons/auth_passkey/static/src/services/check_identity/check_identity.js` (30 lines)
- `addons/auth_passkey/static/src/services/check_identity/check_identity.xml` (19 lines)
- `addons/auth_passkey/static/src/views/auth_passkey_identity_check_form_view.js` (31 lines)
- `addons/auth_passkey/static/src/views/auth_passkey_key_create_form_view.js` (30 lines)
- `addons/auth_passkey/static/tests/passkeys_delete.js` (76 lines)
- `addons/auth_passkey/static/tests/passkeys_login.js` (41 lines)
- `addons/auth_passkey/static/tests/passkeys_registration.js` (117 lines)
- `addons/auth_passkey/static/tests/passkeys_verify.js` (72 lines)
- `addons/auth_passkey/tests/__init__.py` (1 lines)
- `addons/auth_passkey/tests/test_passkey_demo.py` (524 lines)
- `addons/auth_passkey/views/auth_passkey_key_views.xml` (67 lines)
- `addons/auth_passkey/views/auth_passkey_login_templates.xml` (17 lines)
- `addons/auth_passkey/views/res_users_identitycheck_views.xml` (22 lines)
- `addons/auth_passkey/views/res_users_views.xml` (50 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
