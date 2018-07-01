1. 构建初始镜像

```bash
$ docker build -t jxzsxsp/ontology:1.0.0 .
```

2. 用初始镜像启动容器

```bash
$ docker run -itd --name ontology_1 jxzsxsp/ontology:1.0.0
```

3. 进入初始镜像启动容器

```bash
$ docker exec -it ontology_1 bash
```

4. 创建钱包文件，输入两次密码

```bash
# ./ontology account add -d
# exit
```

5. 重新打包初始镜像

```bash
$ docker commit ontology_1 jxzsxsp/ontology:1.0.0
```

6. 将初始镜像发布到远程仓库

```bash
$ docker push jxzsxsp/ontology:1.0.0
```