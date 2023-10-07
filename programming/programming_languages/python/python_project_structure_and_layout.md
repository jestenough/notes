## Multiply Requirements Files

To follow this **pattern first** need to create a `requirements/` directory in the `<repository_root>`. Then need to create `.txt` files that match the contents of your setting directory.

- `base.txt`
- `local.txt`
- `staging.txt`
- `production.txt`

E.g. in the `base.txt`

```python
Django==4.0.0
psycopg2-binary==2.8.8
djangorestframework==4.0.0
```

Your `local.txt` file should have dependencies used for local development, such as:
```python
-r base.txt  # includes the base.txt requirements file

django-debug-toolbar==4.0
```

Production installations should be close to what is used in other locations, so `production.txt` commonly just calls `base.txt`
```python
-r base.txt # includes the base.txt requirements file
```