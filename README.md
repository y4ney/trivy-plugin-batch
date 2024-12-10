# trivy-plugin-batch

一个可以批量扫描 TXT 文件中的镜像文件的 [Trivy](https://github.com/aquasecurity/trivy) 插件。

## 安装

使用前，需要先安装 report 插件

```bash
trivy plugin install github.com/miao2sec/trivy-plugin-report
```

然后再安装本插件

```bash
trivy plugin install github.com/y4ney/trivy-plugin-batch
```

## 帮助页面

```bash
trivy batch --help
使用方法: trivy batch [-h,--help] <txt_file>
 一个可以批量扫描 TXT 文件中的镜像文件的 Trivy 插件。

选项:
  -h, --help    显示使用手册.

示例:
  # 从 TXT 文件中获取镜像文件，进行扫描
  trivy batch <txt_file>
```

## 使用方法

直接指定一个 txt 文件即可

```bash
# 扫描 images.txt 中的镜像文件
trivy batch images.txt
```
