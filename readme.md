# gmanka yml

some useful shortcuts for pyyaml

## installation

```bash
pip install gmanka_yml
```

## functions

- [to_str](#to_str)  
- [save_file](#save_file)  
- [read_file](#read_file)  
- [read_str](#read_str)  

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

## to_str[^](#functions)

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

## save_file[^](#functions)

same as [to_str](#to_str), but writing data to file instead of returning

```py
yml.save_file(
    data = my_dict,
    file_path = 'file.yml',
)
```
