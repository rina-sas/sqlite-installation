# SQLite installation

The latest version of Mac OS X comes with SQLite pre-installed. If yours does not, steps to install are as follows:

## 1. Download SQLite tools

Go to the [SQLite download page](https://sqlite.org/download.html), and download sqlite-autoconf-*.tar.gz.

## 2. Run SQLite tools

Navigate to the folder where the download file is located using Terminal, and run the following command:

```bash
$ tar xvzf sqlite-autoconf-3310100.tar.gz
$ cd sqlite-autoconf-3310100
$ ./configure --prefix=/usr/local
$ make
$ make install
```

**Note：** 

1. After the command $ make is executed, choose to install the command line tools if it shows the make command requires it.

2. If, after the command $ make install is executed, a permission denied error occurs, run the following command. Otherwise skip ahead to step three:

```bash
$ sudo make install
```

## 3. Verify the installation

```bash
$ sqlite3
```

When the installation is complete it should display the following result:

```bash
SQLite version 3.31.1 2020-01-27 19:55:54
Enter ".help" for usage hints.
Connected to a transient in-memory database.
Use ".open FILENAME" to reopen on a persistent database.
sqlite> 
```

Issue commands from the SQLite command prompt.
