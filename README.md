# Ortus Autlogin Script

Tiny (77 byte) and simple script to automatically login to ortus. 

## Usage

### 1. Using Bookmarks

1) Add following line to bookmarks, replacing %login% and %password% with your login and password accrodingly.
```javascript
javascript:((l='%login%',p='%password%')=>{$('#IDToken1').val(l);$('#IDToken2').val(p);LoginSubmit()})();
```
2) When on ortus login page click on that bookmark to automatically login.

### 2. Using Greasemonkey, Tampermonkey or any other user script manager.

1) Create new userscript targeting "https://id2.rtu.lv/openam/*"
2) Paste the following line to user code, replacing %login% and %password% with your login and password accrodingly.
```javascript
((l='%login%',p='%password%')=>{$('#IDToken1').val(l);$('#IDToken2').val(p);LoginSubmit()})();
```




