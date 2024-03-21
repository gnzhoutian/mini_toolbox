# 说明
[![Documentation Status](https://readthedocs.org/projects/mini-tools/badge/?version=latest)](https://mini-tools.readthedocs.io/zh/latest/?badge=latest)


## Example Package

This is a simple example package. You can use
[GitHub-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
to write your content.

## 代办问题

```shell
1. pyproject.toml配置
2. 文档配置
3. test编写?
4. src目录是否必要?
5. 编码规范确定?

```

## 打包说明

```shell
1. 注册账户, 配置token  # https://pypi.org/
    # cat ${HOME}/.pypirc
    [pypi]
        username = __token__
        password = pypi-xxxxxxxxxxxxxxxxxxxxxxxxxx
    
2. 安装依赖
    python3 -m pip install --upgrade pip setuptools wheel
    pip3 install build virtualenv twine

3. 执行打包
    python3 -m build

4. 执行上传
    python3 -m twine upload --repository pypi dist/*
    
5. 本地调试
    pip3 install -e .  # 将本地目录作为库安装

```

## 参考链接

- [Python项目打包](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
- 