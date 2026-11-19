# img

个人图床仓库（配合 PicGo 使用）。

## 外链格式

图片放到仓库任意路径（建议按日期建目录，如 `2026/11/`），提交后即可用下面的地址访问：

```
https://cdn.jsdelivr.net/gh/hejiahao298/img@main/<图片路径>
```

示例：`2026/11/demo.png` →  
`https://cdn.jsdelivr.net/gh/hejiahao298/img@main/2026/11/demo.png`

备用（直连 GitHub CDN，无缓存延迟）：

```
https://raw.githubusercontent.com/hejiahao298/img/main/<图片路径>
```

## 注意事项

- jsDelivr 会缓存已访问过的文件，**同一路径覆盖上传后短时间内仍会返回旧图**；需要立即生效请换个文件名。
- jsDelivr 限制单个文件 20 MB，建议上传前压缩。
- 仓库保持 **Public**，否则 jsDelivr 无法读取。

## PicGo 配置（GitHub 图床）

| 配置项 | 值 |
| --- | --- |
| 仓库名 | `hejiahao298/img` |
| 分支 | `main` |
| Token | GitHub Personal Access Token（需 `repo` 权限） |
| 存储路径 | `images/{year}/{month}/` |
| 设定自定义域名 | `https://cdn.jsdelivr.net/gh/hejiahao298/img@main` |
