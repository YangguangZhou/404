# 404

Jerry Zhou的404页面

# [示例](https://jzhome.vercel.app/404)



如果网站是使用 [Vercel](https://vercel.com) 部署的，可以在根目录下添加 `vercel.json` ，其内容为：

```json
{
    "routes": [
        {"handle": "filesystem"},
        { "src": "/(.*)","status": 404,"dest": "/404/index.html" }
    ]
}
```

如要指定更多页面路径，可以在404这一行后面加上`{ "src": "网址", "dest": "文件相对路径" },`。
如：`{ "src": "/project", "dest": "/project/index.html" },`
