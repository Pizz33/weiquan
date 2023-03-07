### 0x00 前言
首先感谢这些优秀的开源项目。
```
https://github.com/0x727/SchTask_0x727
https://github.com/zha0gongz1/iscsicpl_bypassUAC/
```
原理：
```
选择主机随机进程名作为计划任务程序文件名
将计划任务程序文件复制到 %AppData%\Microsoft\Windows\Themes\ 中
创建的计划任务名取同一随机进程名
计划任务触发器以分钟为单位，无限期持续
更改 Index、删除 SD 的键值，隐藏计划任务对应的 XML 文件
```
插件需要按照以下顺序使用
### 0x01 设置维权马儿路径
![image.png](https://cdn.nlark.com/yuque/0/2023/png/22613130/1678176550033-23375eda-4e1d-4a41-b05f-61842a10a7ea.png#averageHue=%237a7b7b&clientId=uf236cec4-409d-4&from=paste&height=215&id=u553490c4&name=image.png&originHeight=322&originWidth=568&originalType=binary&ratio=1.5&rotation=0&showTitle=false&size=33923&status=done&style=none&taskId=uc5a63540-19ac-41d4-af02-521960c4dca&title=&width=378.6666666666667)
![image.png](https://cdn.nlark.com/yuque/0/2023/png/22613130/1678176587188-8cda2ed6-b3cf-4d54-9a94-e8eb63f557e5.png#averageHue=%23a8cbdd&clientId=uf236cec4-409d-4&from=paste&height=87&id=u90a15837&name=image.png&originHeight=130&originWidth=364&originalType=binary&ratio=1.5&rotation=0&showTitle=false&size=11474&status=done&style=none&taskId=u72fee996-79ac-45cd-944c-04353946408&title=&width=242.66666666666666)
### 0x02 上传维权工具
上传到C:\Windows\Temp目录下，写死的。
![image.png](https://cdn.nlark.com/yuque/0/2023/png/22613130/1678176623112-aad855c9-aabb-440e-8fcc-4cf3a9ab7ff1.png#averageHue=%23565556&clientId=uf236cec4-409d-4&from=paste&height=124&id=uf47373f9&name=image.png&originHeight=186&originWidth=523&originalType=binary&ratio=1.5&rotation=0&showTitle=false&size=20480&status=done&style=none&taskId=ua34d2304-aedf-45af-b29e-c81f97645ab&title=&width=348.6666666666667)
![image.png](https://cdn.nlark.com/yuque/0/2023/png/22613130/1678176680570-570a900b-575e-47c1-8c6a-676a8c500437.png#averageHue=%23101010&clientId=uf236cec4-409d-4&from=paste&height=131&id=uc3611208&name=image.png&originHeight=196&originWidth=1017&originalType=binary&ratio=1.5&rotation=0&showTitle=false&size=46418&status=done&style=none&taskId=uaf9640ac-c782-47d3-bbfd-22d89396a74&title=&width=678)
#### 2.1 管理员权限维权
如果是管理员权限，可直接维权。
![image.png](https://cdn.nlark.com/yuque/0/2023/png/22613130/1678176766986-9b8fdfcb-4b9c-4e0f-8e90-df45f3958c98.png#averageHue=%23f4f5f5&clientId=uf236cec4-409d-4&from=paste&height=204&id=u7c46f12e&name=image.png&originHeight=306&originWidth=423&originalType=binary&ratio=1.5&rotation=0&showTitle=false&size=37267&status=done&style=none&taskId=u61f97be7-307c-45f4-b210-782ccaa730c&title=&width=282)
![image.png](https://cdn.nlark.com/yuque/0/2023/png/22613130/1678176750199-f89605ed-99cb-4940-9f90-c1f047c6427b.png#averageHue=%23090909&clientId=uf236cec4-409d-4&from=paste&height=212&id=ue7e9b590&name=image.png&originHeight=318&originWidth=1049&originalType=binary&ratio=1.5&rotation=0&showTitle=false&size=36615&status=done&style=none&taskId=ubf9cc1cc-0759-4f1c-bcf4-5029df1ef6e&title=&width=699.3333333333334)
#### 2.2 Bypass Uac
普通用户需要bypassuac
![image.png](https://cdn.nlark.com/yuque/0/2023/png/22613130/1678176806795-80707383-d684-42d9-b266-b7d035324ba7.png#averageHue=%23909194&clientId=uf236cec4-409d-4&from=paste&height=101&id=u69f6ad64&name=image.png&originHeight=151&originWidth=378&originalType=binary&ratio=1.5&rotation=0&showTitle=false&size=19044&status=done&style=none&taskId=u16d1858c-4b12-4719-9eb5-0da29b9f1fc&title=&width=252)
![image.png](https://cdn.nlark.com/yuque/0/2023/png/22613130/1678176837071-688470c6-238c-4b24-b550-1818a1f30e92.png#averageHue=%23080808&clientId=uf236cec4-409d-4&from=paste&height=65&id=u080ae3d2&name=image.png&originHeight=97&originWidth=1260&originalType=binary&ratio=1.5&rotation=0&showTitle=false&size=10783&status=done&style=none&taskId=ucb6251e4-ccd4-4c09-8c8d-ce8e6ba05f8&title=&width=840)
### 0x03 删除计划任务（后续考虑集成到插件中）
把%AppData%\Microsoft\Windows\Themes\ 目录下生成的马删掉
![image.png](https://cdn.nlark.com/yuque/0/2023/png/22613130/1678176936365-706949e8-6211-492d-82d5-b2f2a537ea75.png#averageHue=%231e1b1b&clientId=uf236cec4-409d-4&from=paste&height=233&id=ud78e788f&name=image.png&originHeight=350&originWidth=1266&originalType=binary&ratio=1.5&rotation=0&showTitle=false&size=75105&status=done&style=none&taskId=ub768f7a1-6fad-45c9-aa80-3735bab5830&title=&width=844)
删除注册表
```
计算机\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Schedule\TaskCache\Tree\Microsoft\Windows\UPnP
```
![image.png](https://cdn.nlark.com/yuque/0/2023/png/22613130/1678177000978-982acb98-1161-4a6c-9ab8-b45b3052a956.png#averageHue=%23fcfbfa&clientId=uf236cec4-409d-4&from=paste&height=457&id=ude84411d&name=image.png&originHeight=686&originWidth=1383&originalType=binary&ratio=1.5&rotation=0&showTitle=false&size=124426&status=done&style=none&taskId=u031ecdf0-c96c-4881-834c-651b812b0fd&title=&width=922)
删除配置文件
```
C:\Windows\System32\Tasks\Microsoft\Windows\UPnP
```
![image.png](https://cdn.nlark.com/yuque/0/2023/png/22613130/1678177221844-fc487a9e-ce02-4c16-a2c3-27ab62bc4145.png#averageHue=%23211f1e&clientId=uf236cec4-409d-4&from=paste&height=219&id=ue4ba90ca&name=image.png&originHeight=328&originWidth=1303&originalType=binary&ratio=1.5&rotation=0&showTitle=false&size=46913&status=done&style=none&taskId=uf970257a-e975-4fe3-8261-e66a3b64759&title=&width=868.6666666666666)
