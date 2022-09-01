# python

# python-snippets






### make a dict double qouted string and remove spaces inbetween
```python
    def get_data(data):
        '''
        remove all whitespace characters (space, tab, newline, and so on)
        and return object
        return format '{"event":"getportinfo"}' => without any spaces in sigle qoutes key value in double qoutes
        '''
        sdata = str(json.dumps(data))
        rdata = ''.join(sdata.split())
        # print("data after conversion",rdata)
        return rdata
```


### If you face issue while installing python on window 7 , try first installing visual studio 2015 c++ distribution
#### https://www.microsoft.com/en-in/download/details.aspx?id=48145
#### https://support.microsoft.com/en-us/topic/update-for-universal-c-runtime-in-windows-c0514201-7fe6-95a3-b0a5-287930f3560c



```batch
@echo off
start /WAIT /B python -m pip install --upgrade pip wheel setuptools
start /WAIT /B pip install Django==3.2.10
start /WAIT /B python -m venv venv
cmd /WAIT /B /k "venv\Scripts\activate.bat"

```


```batch

netstat -ano | findstr :8000
taskkill  /F /PID 19368 

```


```python
import pickle

user = [

    {'name': 'Ramesh gupta',
     'username': 'rgupta','
     },
    {'name': 'Suresh Sharma',
     'username': 'ssh',
     },

]

pickle.dump(user, open('user.pkl', 'wb'))

my_dict = pickle.load(open('./user.pkl', 'rb'))
print(my_dict)


```
