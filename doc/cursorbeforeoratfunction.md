# cursor_before_or_at()

A predicate over the records of a table to compare their ingestion time
against a database cursor.

**Syntax**

`cursor_before_or_at` `(` *RHS* `)`

**Arguments**

* *RHS*: Either an empty string literal, or a valid database cursor value.

**Returns**

A scalar value of type `bool` that indicates whether the record was ingested
before or at the database cursor *RHS* (`true`) or not (`false`).

**Comments**

See [database cursors](../management/databasecursor.md) for additional
details on database cursors.

This function can only be invoked on records of a table which has the
[IngestionTime policy](../concepts/ingestiontimepolicy.md) enabled.