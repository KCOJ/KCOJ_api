# KCOJ_api
A Python Module for get data from [real KCOJ](https://140.124.184.228/upload/).

## Install
```bash
pip install KCOJ-api
```

## Usage

Create a `KCOJ` object.
```python
>>> from KCOJ_api import KCOJ
>>> kcoj = KCOJ("https://140.124.184.228/upload/")
```

Use `login()` to login real KCOJ.
```python
>>> kcoj.login("username", "password", 4)
<Response [200]>
```

Check online status.
```python
>>> kcoj.logged
True
```

Get question list.
```python
>>> kcoj.get_question()
{'001': {'deadline': '2018/09/19 23:59:59', 'expired': True, 'status': False, 'language': 'Python'}, '002': {'deadline': '2018/09/19 23:59:59', 'expired': True, 'status': False, 'language': 'Python'}, '003': {'deadline': '2018/09/19 23:59:59', 'expired': True, 'status': False, 'language': 'Python'}, '004': {'deadline': '2018/09/19 23:59:59', 'expired': True, 'status': False, 'language': 'Python'},
...
```
