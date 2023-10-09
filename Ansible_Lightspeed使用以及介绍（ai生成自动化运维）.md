> 文档作者：MINE
> 写作时间：2023/7/14
> 操作环境：Centos

<a name="Sy52m"></a>
#### Ansible Lightspeed

- 是什么
```bash
Ansible Lightspeed是AI可以自动生成 Ansible Playbook 任务，
红帽表示，这一新功能使Ansible新手用户更容易实现任务自动化，
从而减轻了自动化专业人员创建低级任务的负担。
用户可以使用英文命令生成Ansible Playbooks自动化任务列表中可以使用的YAML命令。
```

- 使用：

       首先需要有vscode软件，这个软件就不用说了，用来写剧本很直观。<br />       1、打开vscode找到扩展，搜索框输入ansible，点击安装<br />       ![image.png](https://cdn.nlark.com/yuque/0/2023/png/32594981/1689326645823-17423c38-ebd1-4d15-8620-9c2eb0b713a4.png#averageHue=%23f9f9f9&clientId=u5ec36c9d-f4c5-4&from=paste&height=373&id=u575ed4a7&originHeight=1039&originWidth=1894&originalType=binary&ratio=1.3625000715255737&rotation=0&showTitle=false&size=186634&status=done&style=none&taskId=u9a5c2736-7c83-4624-892b-68b353a4afe&title=&width=679.2315673828125)<br /> 2、点击管理，小齿轮那个，点击扩展设置

![image.png](https://cdn.nlark.com/yuque/0/2023/png/32594981/1689326741881-d0fcdad9-cb35-4fc0-9047-b869214e4000.png#averageHue=%23f6f4f3&clientId=u5ec36c9d-f4c5-4&from=paste&height=777&id=u06352c49&originHeight=1059&originWidth=1920&originalType=binary&ratio=1.3625000715255737&rotation=0&showTitle=false&size=306559&status=done&style=none&taskId=u22329381-af5d-454a-b0d3-57e36aed45b&title=&width=1409.1742379508287)

3、鼠标滚轮往下拉，找到Ansible>Lightspeed:Enabled和     	 Ansible>Lightspeed>Suggestions:Enabled两个都勾选上就行。<br />![image.png](https://cdn.nlark.com/yuque/0/2023/png/32594981/1689326788176-b0a61048-9df6-4a67-888d-3fbe734ca73e.png#averageHue=%23f7f7f7&clientId=u5ec36c9d-f4c5-4&from=paste&height=788&id=u00e912d4&originHeight=1074&originWidth=1918&originalType=binary&ratio=1.3625000715255737&rotation=0&showTitle=false&size=252423&status=done&style=none&taskId=u26b0d3ce-b76d-4c01-9bbf-3f591599594&title=&width=1407.7063481196299)

- 4.授权登录，连接github，然后授权，点击ansible得标志，在点击Connect，点击扩展"Ansible"希望使用Ansible Lightspeed登录，打开外部网站。
- ![image.png](https://cdn.nlark.com/yuque/0/2023/png/32594981/1689327158427-8a3d222a-d394-41cc-8d13-2b82ef5d9c34.png#averageHue=%23f9f8f8&clientId=u5ec36c9d-f4c5-4&from=paste&height=722&id=ucf842e6d&originHeight=984&originWidth=1890&originalType=binary&ratio=1.3625000715255737&rotation=0&showTitle=false&size=163699&status=done&style=none&taskId=u0921af3c-c81a-4d56-80ee-cb39f470963&title=&width=1387.155890482847)
<a name="e9ybR"></a>
#### 登录github账号，授权红帽认证。
     ![image.png](https://cdn.nlark.com/yuque/0/2023/png/32594981/1689327258990-3a16a6e1-e191-44c1-8017-cad12413de69.png#averageHue=%23fbfbfa&clientId=u5ec36c9d-f4c5-4&from=paste&height=712&id=u5cc7163a&originHeight=970&originWidth=1920&originalType=binary&ratio=1.3625000715255737&rotation=0&showTitle=false&size=89261&status=done&style=none&taskId=uadf3c303-271f-41f1-8d30-36c53861177&title=&width=1409.1742379508287)


- 5. 鼠标滚轮拉到底，点击Agree，点击Authorize。

![image.png](https://cdn.nlark.com/yuque/0/2023/png/32594981/1689327351060-b1f51112-d3ee-4918-9cde-36f97fe3ef5a.png#averageHue=%23f6f4f3&clientId=u5ec36c9d-f4c5-4&from=paste&height=839&id=u15b93cc3&originHeight=1143&originWidth=1888&originalType=binary&ratio=1.3625000715255737&rotation=0&showTitle=false&size=291194&status=done&style=none&taskId=ue3d2a2da-a3e3-4dc1-85fc-7c1ec1b0232&title=&width=1385.6880006516483)<br />![image.png](https://cdn.nlark.com/yuque/0/2023/png/32594981/1689327418903-a8b635cb-353c-4f95-b79e-2faeff5b0bf5.png#averageHue=%23f8f6f5&clientId=u5ec36c9d-f4c5-4&from=paste&height=799&id=u149df9a8&originHeight=1088&originWidth=1904&originalType=binary&ratio=1.3625000715255737&rotation=0&showTitle=false&size=286208&status=done&style=none&taskId=u91cf6852-30a7-48e1-9815-cbf52c832ae&title=&width=1397.4311193012386)

![image.png](https://cdn.nlark.com/yuque/0/2023/png/32594981/1689327464872-9f67fecd-5538-4624-8154-47ba9454d429.png#averageHue=%23838282&clientId=u5ec36c9d-f4c5-4&from=paste&height=727&id=u4ea96661&originHeight=991&originWidth=1903&originalType=binary&ratio=1.3625000715255737&rotation=0&showTitle=false&size=78316&status=done&style=none&taskId=u76c9126e-bc58-4a7b-836b-bdda863f365&title=&width=1396.697174385639)

<a name="C97iy"></a>
#### 然后跳转到自动vscode，这是正确认证过的。github账号已经成功登录
![image.png](https://cdn.nlark.com/yuque/0/2023/png/32594981/1689327610150-38a6dc22-d8c9-408e-b719-66dee97871fb.png#averageHue=%23f9f8f8&clientId=u5ec36c9d-f4c5-4&from=paste&height=826&id=u1ebba787&originHeight=1125&originWidth=1920&originalType=binary&ratio=1.3625000715255737&rotation=0&showTitle=false&size=157155&status=done&style=none&taskId=u47763534-6679-463e-baf2-2bfecaf74e8&title=&width=1409.1742379508287)


<a name="Fuj35"></a>
#### 使用教程
连接一个ssh终端，并打开一个yml，剧本文件。可以看到ansible版本以及要选择的python版本。<br />有这个lightspeed标识，证明你的lightspeed才能用<br />![image.png](https://cdn.nlark.com/yuque/0/2023/png/32594981/1689327917066-18955a5a-515e-431b-90e8-eccc6e1a729c.png#averageHue=%23f9f8f7&clientId=u5ec36c9d-f4c5-4&from=paste&height=878&id=u4d0d1166&originHeight=1196&originWidth=1909&originalType=binary&ratio=1.3625000715255737&rotation=0&showTitle=false&size=295436&status=done&style=none&taskId=u2e70a2c6-9903-454e-9363-894ee802105&title=&width=1401.1008438792355)

鼠标光标移动到任务name的最后，然后按一下回车键，等待Ai生成结果<br />![image.png](https://cdn.nlark.com/yuque/0/2023/png/32594981/1689328453757-245b99bb-4dda-4eec-9499-a7c7b6052dbb.png#averageHue=%23f9f7f6&clientId=u5ec36c9d-f4c5-4&from=paste&height=858&id=ua0843a55&originHeight=1169&originWidth=1920&originalType=binary&ratio=1.3625000715255737&rotation=0&showTitle=false&size=231832&status=done&style=none&taskId=u00dc0183-c4be-46ac-9187-98971191ba5&title=&width=1409.1742379508287)


回车键按下后等待lightspeed生成，一定要等会，下面是生成的结果，生成结果后按住tab键，自动添加上ai生成的结果，很强大，妈妈再也不用担心我的学习。结果根据自定义修改<br />![image.png](https://cdn.nlark.com/yuque/0/2023/png/32594981/1689328633710-0f585e84-1e25-429a-b186-02e1fe425cfc.png#averageHue=%23f9f8f7&clientId=u5ec36c9d-f4c5-4&from=paste&height=857&id=ue3e2cac0&originHeight=1167&originWidth=1920&originalType=binary&ratio=1.3625000715255737&rotation=0&showTitle=false&size=212746&status=done&style=none&taskId=u88f12349-2cb3-423e-af83-f853077304c&title=&width=1409.1742379508287)

有视频教程，但是是油管的，所以需要魔法才能看，视频放在下方。不懂得直接看视频<br />[https://www.youtube.com/watch?v=yfXcGB7l0II](https://www.youtube.com/watch?v=yfXcGB7l0II)

![image.png](https://cdn.nlark.com/yuque/0/2023/png/32594981/1689328836642-dc2adefc-f12d-4183-9859-a68dc130a678.png#averageHue=%23bebdb5&clientId=u5ec36c9d-f4c5-4&from=paste&height=870&id=u2a855f8b&originHeight=1186&originWidth=1920&originalType=binary&ratio=1.3625000715255737&rotation=0&showTitle=false&size=942193&status=done&style=none&taskId=ub5b75c1e-81e8-4abb-b811-6a04d6e9255&title=&width=1409.1742379508287)
