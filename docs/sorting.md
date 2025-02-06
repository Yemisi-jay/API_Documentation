# Sorting

You can use the `orderBy` parameter to specify the order of records in the response. This allows you to sort the results in ascending or descending order.

### Ascending Order

By default, results are returned in ascending order. For example, to return a list of transactions in ascending order (oldest first), use the following syntax:

``` bash

curl --location --request GET 'https://api.test.woodcoreapp.com/api/v1/clients?orderBy=date' \
--header 'Authorization: Bearer wc_test_5l0Fk28F2EUWiy01Vs9x7fEDWdYY8zqu90E986m8'
```
### Descending Order

To return results in descending order, prepend a `-`(negative sign) to the parameter value. For example, to return the same list of transactions with the newest transactions first, use the following syntax:

``` bash

curl --location --request GET 'https://api.test.woodcoreapp.com/api/v1/clients?orderBy=-date' \
--header 'Authorization: Bearer wc_test_5l0Fk28F2EUWiy01Vs9x7fEDWdYY8zqu90E986m8'
```