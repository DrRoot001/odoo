# API Overview

Static inspection found 975 route decorator declarations across the repository. Route paths, HTTP methods, authentication modes, request schemas, and response schemas are often expressed across decorators, method bodies, serializers, and inherited controllers; they are therefore inventoried by source location rather than guessed into a universal schema.

The source implementation is under `odoo/http/` and addon controller files. No claim is made that every route is enabled in a particular deployment.
