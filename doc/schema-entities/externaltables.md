# External tables (preview)

An **external table** is a Kusto schema entity that references data stored outside Azure Data Explorer.
Similar to [tables](tables.md), an external table has a well-defined schema (an ordered list of column name/type pairs). Unlike tables, data is stored and managed outside Azure Data Explorer. Most commonly the data is stored in some standard format such as CSV, Parquet, Avro, and is not ingested by Azure Data Explorer.

An external table is created once (see [External Table control commands](../../management/externaltables.md))
and can be referenced by its name. External table names canâ€™t overlap with Kusto table names.

> [!NOTE]
> Kusto supports [exporting data to an external table](../../management/data-export/export-data-to-an-external-table.md).
> as well as [querying external tables](https://docs.microsoft.com/en-us/azure/data-explorer/data-lake-query-data).
