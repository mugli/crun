# 根据正则生成所有可能性

* [English](./README.md)
* [简体中文](./README_cn.md)

## 用法

```
Usage of crun:
           crun <regexp>
        or crun "\d{3}"
        or crun "[0-9a-z]{2}"
        or crun "(root|admin) [0-9]{1}"
```

### 实例

``` bash
# 生成 1到6位长度的数字所有可能性组合
crun "\d{1,6}"

# 暴力美学
crun "(root|admin):[0-9]{4,5}"

# 注意: 如果量太大会超卡的
```

### 下载 & 安装
``` bash
go get -u -v github.com/wzshiming/crun/cmd/crun
```