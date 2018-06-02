# SimpleBeego

在命令行输入bee api SimpleBeego
```
D:\WorkSoftWare\Go\GoDev\src>bee api SimpleBeego
______
| ___ \
| |_/ /  ___   ___
| ___ \ / _ \ / _ \
| |_/ /|  __/|  __/
\____/  \___| \___| v1.9.1
2018/06/02 15:06:32 INFO     ▶ 0001 Creating API...
        create   D:\WorkSoftWare\Go\GoDev\src\SimpleBeego
        create   D:\WorkSoftWare\Go\GoDev\src\SimpleBeego\conf
        create   D:\WorkSoftWare\Go\GoDev\src\SimpleBeego\controllers
        create   D:\WorkSoftWare\Go\GoDev\src\SimpleBeego\tests
        create   D:\WorkSoftWare\Go\GoDev\src\SimpleBeego\conf\app.conf
        create   D:\WorkSoftWare\Go\GoDev\src\SimpleBeego\models
        create   D:\WorkSoftWare\Go\GoDev\src\SimpleBeego\routers\
        create   D:\WorkSoftWare\Go\GoDev\src\SimpleBeego\controllers\object.go
        create   D:\WorkSoftWare\Go\GoDev\src\SimpleBeego\controllers\user.go
        create   D:\WorkSoftWare\Go\GoDev\src\SimpleBeego\tests\default_test.go
        create   D:\WorkSoftWare\Go\GoDev\src\SimpleBeego\routers\router.go
        create   D:\WorkSoftWare\Go\GoDev\src\SimpleBeego\models\object.go
        create   D:\WorkSoftWare\Go\GoDev\src\SimpleBeego\models\user.go
        create   D:\WorkSoftWare\Go\GoDev\src\SimpleBeego\main.go
2018/06/02 15:06:32 SUCCESS  ▶ 0002 New API successfully created!
```
执行bee run
```
D:\WorkSoftWare\Go\GoDev\src\SimpleBeego>bee run
______
| ___ \
| |_/ /  ___   ___
| ___ \ / _ \ / _ \
| |_/ /|  __/|  __/
\____/  \___| \___| v1.9.1
2018/06/02 15:18:44 INFO     ▶ 0001 Using 'SimpleBeego' as 'appname'
2018/06/02 15:18:44 INFO     ▶ 0002 Initializing watcher...
SimpleBeego/models
SimpleBeego/controllers
SimpleBeego/routers
SimpleBeego
2018/06/02 15:18:50 SUCCESS  ▶ 0003 Built Successfully!
2018/06/02 15:18:50 INFO     ▶ 0004 Restarting 'SimpleBeego'...
2018/06/02 15:18:50 SUCCESS  ▶ 0005 './SimpleBeego' is running...
2018/06/02 15:18:50.401 [I] [parser.go:96] generate router from comments
2018/06/02 15:18:50.420 [I] [router.go:269] D:\WorkSoftWare\Go\GoDev\src\SimpleBeego\controllers no changed
2018/06/02 15:18:50.449 [I] [asm_amd64.s:2361] http server Running on http://:8080
SimpleBeego/routers
SimpleBeego
2018/06/02 15:18:56 SUCCESS  ▶ 0006 Built Successfully!
```
访问http://localhost:8080/v1/user
可以看到
```
{
    "user_11111": {
        "Id": "user_11111",
        "Username": "astaxie",
        "Password": "11111",
        "Profile": {
            "Gender": "male",
            "Age": 20,
            "Address": "Singapore",
            "Email": "astaxie@gmail.com"
        }
    }
}
```