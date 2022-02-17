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

<br>

***HTML***
```html
<script>
    fetch('https://password-api.sanchogodinho.repl.co/lengthOfPassword').then(res => res.json()).then(data => {
        if ('error' in data){
            console.log(data.error)
        }
        else{
            password = data.password;
            console.log(password);
        }
    });
</script>
```
