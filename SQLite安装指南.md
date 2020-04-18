# SQLite安装指南

最新版本的 Mac OS X 会预安装 SQLite，如果没有可用的程序，可按下列步骤进行：

## 1. 下载安装包

请访问 [SQLite 下载页面](https://sqlite.org/download.html)，从源代码区下载 sqlite-autoconf-*.tar.gz。

## 2. 使用 Terminal 执行 bash 命令安装

打开terminal，进入压缩文件所在的文件夹，执行下述步骤：

```bash
$ tar xvzf sqlite-autoconf-3071502.tar.gz
$ cd sqlite-autoconf-3071502
$ ./configure --prefix=/usr/local
$ make
$ make install
```

**注意事项：** 

1. 执行 $ make 时，若系统提示 the make command requires command line tools, 依照提示选择安装即可。
2. 执行 $ make install 时，若出现因权限问题导致的安装失败，可执行如下命令。若无问题，请前往第三步。

```bash
$ sudo make install
```

## 3. 测试

```bash
$ sqlite3
```

出现下列提示即表明安装成功。

```bash
SQLite version 3.31.1 2020-01-27 19:55:54
Enter ".help" for usage hints.
Connected to a transient in-memory database.
Use ".open FILENAME" to reopen on a persistent database.
sqlite> 
```

即可在 SQLite 命令提示符下，输入 SQLite 命令，执行所需操作。

