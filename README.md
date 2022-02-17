# Password-Api

## What Is Password-Api?
<pre>
It's A Simple Password API Developed By Me!
It Generates Random Password That You Can Use!
It Can Generate Password Upto 10000 Characters Long!
</pre>

<br>

## Api URL?
<pre>Api Original URL: <a href='https://password-api.sanchogodinho.repl.co/'>https://password-api.sanchogodinho.repl.co/</a></pre>

<br>

## Api Methods?
<pre>GET</pre>

<br>

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

<br>

***Node JS***  
<br>
*Terminal :-*
```bash
npm i axios
```
*Node JS Code :-*
```javascript
const axios = require('axios');

const data = axios.get('https://password-api.sanchogodinho.repl.co/lengthOfPassword').then(data => {
    if ('error' in data.data){
        console.log(data.data.error);
    }
    else{
        password = data.data.password;
        console.log(password);
    }
});
```

<br>

**Note: The lengthOfPassword Should Be Replaced With A Number That You Choose The Length Of The Password.**
