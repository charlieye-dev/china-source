## pip

1. 在根目录下创建.pip文件夹

```
mkdir ~/.pip
```

2. 在创建好的.pip文件夹下创建pip源配置文件

```
touch ~/.pip/pip.conf
```

3. 配置pip源到**pip.conf**文件(如下三选一)

    - 阿里源
     
      ```
      [global]
      index-url=http://mirrors.aliyun.com/pypi/simple
      trusted-host=mirrors.aliyun.com
      ```
