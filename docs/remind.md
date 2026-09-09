# zensical的github部署

## github仓库设置

```
1.Actions设置下==>General设置==>Workflow permissions设置==>勾选“Read and write permissions”和“Allow GitHub Actions to create and approve pull requests”，然后保存。
2.Pages设置下==>Build and deployment的Source设置更改为“Github Actions”。
```

## 终端来到工作区目录（内含.venv文件夹），激活虚拟环境。
```
.venv\Scripts\activate（已创建虚拟环境）
python -m venv .venv（未创建虚拟环境，则使用该命令创建）
```

## 用zensical new 创建网站文件夹，用zenscial serve 预览网页效果，用zensical build 生成网页html。

##  将所有文件添加到暂存区
```
git add .
```

## 提交文件(关键是要提交到main上)
```
git commit -m "Initial commit"
```

## 关联远程仓库（若尚未关联，替换为你的实际地址）
```
git remote add origin https://github.com/zhongxj481/zblog.git
```

## 推送到远程 main 分支
```
git branch -M main
git push origin main
```
