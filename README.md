登录

```
url：47.107.244.80:xxx/login
method:'post'
params(需要提交的参数）:
	'username':xxx,
	'password':xxx,
	
return data:
	'message':xxx,
	'data':None,
	'code':xxx
```

注册

```
url：47.107.244.80:xxx/login
method:'post'
params(需要提交的参数）:
	'username':xxx,
	'password':xxx,
	're_password':xxx,
	'hostname':xxx
	
return data:
	'message':xxx,
	'data':None,
	'code':xxx
```

返回单个传感器的具体数据

```
url：47.107.244.80:xxx/get_detail
method:'post'
params(需要提交的参数）:
	'type':xxx, 
#'rain', 'sensirion', 'body', 'depth', 'lock', 'led', 'alarm',
 'fire', 'uv', 'smoke', 'light', 'man'(只能从里面选)
	
	
return data:
	'message':xxx,
	'data':
	{
       'introduce':xxx,
       'list':[
           {
               type:xxx,
               'create_time':xxx
           },{},{},{},{}
       ]  #返回最新五条
	},
	'code':xxx

```

控制某个传感器

```
url：47.107.244.80:xxx/contorl
method:'post'
params(需要提交的参数）:
	'type':xxx, 
#'rain', 'sensirion', 'body', 'depth', 'lock', 'led', 'alarm',
 'fire', 'uv', 'smoke', 'light', 'man'(只能从里面选)
	
	
return data:
	'message':xxx,
	'data':None,
	'code':xxx
```

获取所有最新一条数据

```
url：47.107.244.80:xxx/get_all
method:'post'
params(需要提交的参数）:

return data:
	'message':xxx,
	'data':{
        'rain': xxx,
        'temperature': xxx,
        'humidity': xxx,
        'body': xxx,
        'depth': xxx,
        'lock': xxx,
        'led': xxx,
        'alarm': xxx,
        'fire': xxx,
        'uv': xxx,
        'smoke': xxx,
        'light': xxx,
        'man': xxx
	},
	'code':xxx
```

