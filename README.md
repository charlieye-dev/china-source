[apt](#Apt)

[pip](#Pip)

[example](#Example)

## Apt

1. 备份原始的源

```
cp /etc/apt/sources.list /etc/apt/sources.list.bak
```

3. 配置apt源到**/etc/apt/sources.list**文件

    - 阿里源

      ```
      deb http://mirrors.aliyun.com/ubuntu/ focal main restricted universe multiverse
      deb-src http://mirrors.aliyun.com/ubuntu/ focal main restricted universe multiverse
      
      deb http://mirrors.aliyun.com/ubuntu/ focal-security main restricted universe multiverse
      deb-src http://mirrors.aliyun.com/ubuntu/ focal-security main restricted universe multiverse
      
      deb http://mirrors.aliyun.com/ubuntu/ focal-updates main restricted universe multiverse
      deb-src http://mirrors.aliyun.com/ubuntu/ focal-updates main restricted universe multiverse
      
      deb http://mirrors.aliyun.com/ubuntu/ focal-proposed main restricted universe multiverse
      deb-src http://mirrors.aliyun.com/ubuntu/ focal-proposed main restricted universe multiverse
      
      deb http://mirrors.aliyun.com/ubuntu/ focal-backports main restricted universe multiverse
      deb-src http://mirrors.aliyun.com/ubuntu/ focal-backports main restricted universe multiverse
      ```

    - 网易163源

      ```
      deb http://mirrors.163.com/ubuntu/ focal main restricted universe multiverse
      deb-src http://mirrors.163.com/ubuntu/ focal main restricted universe multiverse
      
      deb http://mirrors.163.com/ubuntu/ focal-security main restricted universe multiverse
      deb-src http://mirrors.163.com/ubuntu/ focal-security main restricted universe multiverse
      
      deb http://mirrors.163.com/ubuntu/ focal-updates main restricted universe multiverse
      deb-src http://mirrors.163.com/ubuntu/ focal-updates main restricted universe multiverse
      
      deb http://mirrors.163.com/ubuntu/ focal-proposed main restricted universe multiverse
      deb-src http://mirrors.163.com/ubuntu/ focal-proposed main restricted universe multiverse
      
      deb http://mirrors.163.com/ubuntu/ focal-backports main restricted universe multiverse
      deb-src http://mirrors.163.com/ubuntu/ focal-backports main restricted universe multiverse
      ```

## Pip

1. 在根目录下创建.pip文件夹

```
mkdir ~/.pip
```

2. 在创建好的.pip文件夹下创建pip源配置文件

```
touch ~/.pip/pip.conf
```

3. 配置pip源到**pip.conf**文件

    - 阿里源
     
      ```
      [global]
      index-url=http://mirrors.aliyun.com/pypi/simple
      trusted-host=mirrors.aliyun.com
      ```

## Example

```
cat << EOF > /etc/apt/sources.list
> deb http://mirrors.aliyun.com/ubuntu/ focal main restricted universe multiverse
> deb-src http://mirrors.aliyun.com/ubuntu/ focal main restricted universe multiverse
> 
> deb http://mirrors.aliyun.com/ubuntu/ focal-security main restricted universe multiverse
> deb-src http://mirrors.aliyun.com/ubuntu/ focal-security main restricted universe multiverse
> 
> deb http://mirrors.aliyun.com/ubuntu/ focal-updates main restricted universe multiverse
> deb-src http://mirrors.aliyun.com/ubuntu/ focal-updates main restricted universe multiverse
> 
> deb http://mirrors.aliyun.com/ubuntu/ focal-proposed main restricted universe multiverse
> deb-src http://mirrors.aliyun.com/ubuntu/ focal-proposed main restricted universe multiverse
> 
> deb http://mirrors.aliyun.com/ubuntu/ focal-backports main restricted universe multiverse
> deb-src http://mirrors.aliyun.com/ubuntu/ focal-backports main restricted universe multiverse
> EOF
```
