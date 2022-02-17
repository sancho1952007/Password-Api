# Password-Api

## Api Usage :-
***Python***
```python
from urllib import request
import json

data=request.urlopen("https://password-api.sanchogodinho.repl.co/lengthOfPassword")
data=json.loads(data.read())
if ('error' in data):
    print(data["error"])
else:
    password=data["password"]
    print(password)
```

***HTML***
```
