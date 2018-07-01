1. 使用初始镜像构建测试镜像

```bash
$ docker build -t jxzsxsp/ontology:1.0.0-testmode .
```

2. 将测试镜像发布到远程仓库

```bash
$ docker push jxzsxsp/ontology:1.0.0-testmode
```

3. 从远程仓库拉取测试镜像

```bash
$ docker pull jxzsxsp/ontology:1.0.0-testmode
```

4. 从测试镜像启动容器

```bash
$ docker run -itd -p 20333-20339:20333-20339 -p 20000:20000 --name ontology_1_testmode jxzsxsp/ontology:1.0.0-testmode
```

5. 查看版本

```bash
curl -X GET http://localhost:20334/api/v1/version
```