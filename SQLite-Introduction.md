# What is SQLite?

SQLite is an in-process lightweight library that provides a relational database management system. It is called a self-contained, serverless, zero-configuration and transactional SQL database engine by developers. It was written in the C programming language by D. Richard Hipp in 2000 and the source code for SQLite is in the public domain. It is available for anyone for any use free of charge.

# How does SQLite work?

SQLite compiles SQL text into bytecode, then run that bytecode in a virtual machine. 
The sqlite3_prepare_v2() and related interfaces serve as a compiler to convert SQL text into bytecode. The sqlite3_stmt object works as a container to implement a single SQL query for a single bytecode program use. The sqlite3_step() interface sends a bytecode program into the virtual machine and runs the program until it either completes, returns a row of results, hits a fatal error, or is interrupted.

# What are its significant features?

* SQLite is self-contained and comes with zero-configuration, so it is easy to install, setup, and build. It is designed and used as an embedded database and offers a popular option for web browsers to store data locally or on the client-side. It is widely used across different operating systems and does not rely on external dependencies. 

* The SQLite library is compact and its size can be less than 600KB depending on the target platform and compiler optimization settings. It performs well in low-memory environments. It accesses the files containing the data directly instead of accessing a server. With optimized use, SQLite can be faster than direct filesystem I/O. 

* SQLite is ACID-compliant and implements most of the standard SQL. It is lightweight compared to others such as MySql and Oracle, and it provides simple and easy-to-use APIs. SQLite uses dynamic types for tables. This means you can store any value in any column, regardless of the data type. It allows one single database connection to manipulate multiple database files all at once.
