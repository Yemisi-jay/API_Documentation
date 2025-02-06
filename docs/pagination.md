# Pagination

The WoodCore API provides a simple set of query parameters to handle pagination, making it easier to retrieve large datasets efficiently.

###  Description

Endpoints that return multiple results are paginated. To fetch data, you must supply an **offset** query parameter. You can also define the page size using the **limit** query parameter.

- **`perPage`**: Specifies the number of records per page.
- **`page`**: Specifies the page number to be retrieved.

###  Default Behavior

By default, the system returns **`15`** records per page if **`perPage`** is not specified.
