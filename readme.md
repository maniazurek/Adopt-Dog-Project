# List of technologies used in project

- HTML
- CSS
- CSS variables
- fetch()
- vanilla JavaScript
- Rest API

# Documentation

## 1. API

**Base url**: https://dogs-api.fly.dev

**GET** /dogs

_Query parameters_:

1. gender: `String` (optional)

   Available values: `'male'`, `'female'`

2. size: `String` (optional)

   Available values: `'1small'`, `'2medium'`, `'3large'`

3. name: `String` (optional)

   Available values: `Any string`,

4. page: `Number` (optional)

   Available values: `1 - ∞`

   Default value: `1`

5. sort: `String` (optional)

   Available values: `'name'`, `'size'`

   Default value: `'name'`

_Response success_:

```
{
  records: Array<{
    _id: ObjectId,
    name: String,
    gender: String,
    size: String,
    image: String,
    __v: Int32
  }>,
  totalCount: Number,
  success: Boolean
}
```

_Response error_:

```
{
  error: ErrorObject,
  success: Boolean
}
```
