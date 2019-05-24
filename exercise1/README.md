# Exercise 1

## 1) Write TypeDefs
- Open [types.py](https://github.com/Speedy1991/graphql_workshop/blob/master/exercise1/schema/types.py)
- TODO: Fill the fields with the related scalar types
- INFO: The fields you define in the TypeDefs will be queryable on your schema

## 2) Write resolvers
- Open [query.py](https://github.com/Speedy1991/graphql_workshop/blob/master/exercise1/schema/query.py)
- TODO: Define the fields and resolvers

## Questions

```
resolve_random_names(self, info, **kwargs):
    return ["Peter", "Paul", "Amy"]
    
resolve_number(self, info, **kwargs):
    return 5
```

Do you know the related field definitions?


## Sample

Query:
```
{
  students {
    id
    age
    name
    semester
  }
}
```

Result:

```
{
  "data": {
    "students": [
      {
        "id": "1",
        "age": 22,
        "name": "John",
        "semester": 1
      },
      {
        "id": "2",
        "age": 32,
        "name": "Ponnappa",
        "semester": 3
      },
      ...
```