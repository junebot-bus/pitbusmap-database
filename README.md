# pitbusmap transit database

Served to the app over the air by `DatabaseRetriever`:

    dcbusmap.sqlite        the Core Data store
    dcbusmap_version.txt   the version the app compares against

The filenames are `dcbusmap.*` in every city's repo because
`City.databaseName` is shared across all cities. That is intentional.

`dcbusmap_version.txt` is pinned at **1.0**, which is below the
version this city's app bundles, so no update is offered. The store here matches
what the current build already ships. Raise the version only when publishing
data that is genuinely newer than any shipped bundle.
