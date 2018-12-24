# README
jupyter tensorFlow notebook

# NO.1 virtualenv setup:
- setup virtualenv
```bash
sudo easy_install pip
sudo pip install --upgrade virtualenv

# --system-site-packages 使隔离环境可以访问系统python安装包
# --no-site-packages（default）使隔离环境不能访问系统python安装包
virtualenv --no-site-packages -p python3 venv

# 进入虚拟环境
source venv/bin/activate

# 退出虚拟环境
deactivate

# 删除虚拟环境
rm -r venv
```

- setup tensorflow
```bash
pip install --upgrade tensorflow
```

# NO.2 Docker step:
- using
```text
docker-compose up -d
```

# update Backend



# REFERENCE
## virtualenv using a three-way source
```bush
# Temporarily add third-party source
pip install -i http://mirrors.aliyun.com/pypi/simple/ packageName

vim ~/.pip/pip.conf                 -- created without

[global]
index-url = http://mirrors.aliyun.com/pypi/simple/

[install]
trusted-host=mirrors.aliyun.com
```

## jupyter 
```text
jupyter notebook --generate-config

jt -l                   -- list themes
jt -t chesterish        -- select themes
jt -r                   -- restore themes
```

## project related
```text
pip list
pip list --outdate


pip install --upgrade packageName     
pip install -U packageName          -- install or upgrade package
pip uninstall packageName           -- delete package

pip freeze > requirements.txt       -- generate requirements.txt
pip install -r requirements.txt 

#jupyter
#jupyterthemes
```

## python related
```text
source activate tensorflow      -- activation
which python
```

- [travis](https://travis-ci.org/)