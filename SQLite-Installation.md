# SQLite installation

The latest version of Mac OS X has pre-installed SQLite. if it doesn't, steps to install are as follows:

## 1. Download SQLite tools

Go to the [SQLite download page](https://sqlite.org/download.html), and download sqlite-autoconf-*.tar.gz.

## 2. Run SQLite tools

Navigate to the folder where the download file located using Terminal, and run the following command:

```bash
$ tar xvzf sqlite-autoconf-3071502.tar.gz
$ cd sqlite-autoconf-3071502
$ ./configure --prefix=/usr/local
$ make
$ make install
```

**Note：** 

1. After the command $ make executed，choose to install the command line tools if it shows the make command requires it.
2. After the command $ make install executed, and permission denied error occurs, run the following command instead:

```bash
$ sudo make install
```

## 3. Verify the installation

```bash
$ sqlite3
```

When the installation completed, it should display the following result:

```bash
SQLite version 3.31.1 2020-01-27 19:55:54
Enter ".help" for usage hints.
Connected to a transient in-memory database.
Use ".open FILENAME" to reopen on a persistent database.
sqlite> 
```

Issue commands from the sqlite command prompt.

