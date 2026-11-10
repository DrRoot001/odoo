# Workflow Catalog

The repository implements workflows through ORM methods, HTTP controllers, scheduled actions, bus/mail services, XML actions, and addon-specific state fields. A universal business workflow catalog is not valid without an installed module set. Verified platform workflows are:

1. Server bootstrap and configuration.
2. Addon dependency resolution and loading.
3. HTTP request routing and response handling.
4. ORM transaction/constraint/access processing.
5. Scheduled/background action execution.
6. Test discovery/execution.

Business-domain workflows must be traced from the relevant module page and source files; example ERP flows are not asserted unless found in code.
