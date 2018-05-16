# HVSQLite
This project is a C implementation of a basic SQLite stack. 
I'm following this [awesome tutorial](https://cstack.github.io/db_tutorial/) and adding my own improvements and customizations.

The main goal here is to learn how a database works from top to bottom.

![](https://cstack.github.io/db_tutorial/assets/images/arch2.gif)

## Running
This project is being developed using Xcode and Ruby for the tests.

### Executable
The Xcode project is configured with 2 schemes, 1 for running the executable and another for the tests. 
![](https://i.imgur.com/xKxTmHM.png)

### Tests
The `HVSQLiteTests` scheme, under `Post-actions`, has the following shell command to run all the tests. 

```
exec > ${PROJECT_DIR}/tests.log 2>&1
rspec ${PROJECT_DIR}/spec/main_spec.rb
```
![](https://i.imgur.com/40JXqty.png)

The tests' results will be available on the project's directory inside the `tests.log` file.
