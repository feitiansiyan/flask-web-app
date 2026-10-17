# Flask 自动部署实验

这是实验第一阶段的项目：网页显示 `Hello, World!`。
GitHub Actions 工作流将在服务器首次部署完成、SSH 密钥配置成功后添加。

## 文件说明

- `src/app.py`：网页程序，监听 5000 端口。
- `src/__init__.py`：将 src 标记为 Python 包。
- `tests/test_app.py`：检查首页状态码为 200，正文为 `Hello, World!`。
- `requirements.txt`：按实验指导固定依赖版本。

## 测试

安装依赖后，在项目根目录执行：

```bash
python -m unittest discover -s tests -v
```

## 后续修改

自动部署验证阶段，需要同时将程序和测试里的 `Hello, World!` 改成
`Hello, NEU!`，再提交到 main 分支。

不要把 GitHub 访问令牌、服务器密码、SSH 私钥或头歌信息配置文件上传到本仓库。
