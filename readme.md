# gmanka yml

some useful shortcuts for pyyaml

```py
import gmanka_yml as yml

my_dict = {
    'element_1': 1,
    2: 'element_2',
    3: [
        'list_element_1',
        'list_element_2',
    ]
}
```

## to_str

converting any data to yml string and returning it

```py
print(yml.to_str(my_dict))
```

output:

```yaml
element_1: 1
2: element_2
3:
- list_element_1
- list_element_2
```

## save_file

same as [to_str](#to_str), but writing data to file instead of returning

```py
yml.save_file(
    data = my_dict,
    file_path = 'file.yml',
)
```
