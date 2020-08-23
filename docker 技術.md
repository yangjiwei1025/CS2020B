# docker 技術
```
利用 Docker 來自架 Gitlab
```

#
```
Docker —— 從入門到實踐
https://philipzheng.gitbooks.io/docker_practice/content/introduction/

10個Q&A快速認識Docker
https://www.ithome.com.tw/news/91847

Docker 基本架構概念教學
https://www.youtube.com/watch?v=pa1Zao1Hy2c&t=102s
```
# 利用 Docker 來自架 Gitlab
```
https://medium.com/appworks-school/%E7%B0%A1%E6%98%93%E6%95%99%E5%AD%B8-%E5%88%A9%E7%94%A8-docker-%E6%9E%B6%E8%A8%AD-gitlab-b392f75584dd
```
```
1.下載回本機端(打開終端機，輸入下列語法)
docker image pull gitlab/gitlab-ce:9.0.5-ce.0

2.新建並啟用 Container
docker run --detach --publish 8787:80 --name gitlab gitlab/gitlab-ce:9.0.5-ce.0

- - detach: 在背景執行一個 Container
- - public [8787:80]: 設定一個 port 還做 docker 裡頭的 web 接口
- - name [gitlab]: 自訂一個 Container 的名稱
```
