# Relationships

Relationships are implemented through Odoo ORM field declarations (`Many2one`, `One2many`, `Many2many`, reference/property fields), delegated inheritance, and application-level methods. Static model metadata alone does not establish every cardinality; use `Entity_Dictionary.csv` together with field declarations in the cited source files. A deployed ERD must be generated after selecting/installing the target addon set.
