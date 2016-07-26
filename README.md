# Ortus Autlogin Script

Tiny (76 byte) and simple script to automatically login to ortus. 

## Usage

### 1. Using Bookmarks

1) Add following line to bookmarks, replacing %login% and %password% with your login and password accrodingly.
```javascript
javascript:((l='%login%',p='%password%')=>{$('#IDToken1').val(l);$('#IDToken2').val(p);LoginSubmit()})()
```

2) When on ortus login page click on that bookmark to automatically login.

### 2. Using Greasemonkey, Tampermonkey or any other user script manager.

1) Create new userscript targeting "https://id2.rtu.lv/openam/*"

2) Paste the following line to user code, replacing %login% and %password% with your login and password accrodingly.
```javascript
((l='%login%',p='%password%')=>{$('#IDToken1').val(l);$('#IDToken2').val(p);LoginSubmit()})()
```

## About

I am tired of entering my login and password every time I go to ortus. Their login page does not allow password saving (at least in chrome), so I wrote a little script to automatically enter credentails and login. 

If anyone doesn't like immediately invoked function - minified script is available. I am using it to group settings in the parameters and make password changing little faster. 


## License

[wtfpl](http://www.wtfpl.net/)




