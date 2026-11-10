# Role-Permission Matrix

A universal static matrix is not valid for this repository because roles and permissions are declared across addons and may be extended through inheritance. Use the following evidence-driven matrix for a deployment-specific extraction:

| Scope | Evidence source | Status |
|---|---|---|
| User/group definitions | Addon XML data and base user/group models | Present; module-specific |
| Model CRUD access | `ir.model.access.csv` files | Present in selected addons |
| Record-level rules | `security/*.xml` and model rules | Present in selected addons |
| Route authentication | Controller decorators and request handling | Present; route-specific |
| Tenant/company restrictions | Model fields/rules and context logic | Requires deployment/module verification |
