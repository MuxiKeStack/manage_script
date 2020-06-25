# manage_script

> Scripts for MuxiKeStack.

+ history_course：云课堂课程
+ using_course：选课手册课程

## 课程导入

每学期选课手册公布时，运维人员执行脚本，手动导入选课手册的课程和云课堂的课程

#### 环境变量

```shell
export MUXIKSTACK_DB_ADDR=127.0.0.1:3306
export MUXIKSTACK_DB_USERNAME=root
export MUXIKSTACK_DB_PASSWORD=root
```

#### 导入选课手册

导入选课手册要先将Excel文件移动至`using_course`目录下，然后在`using_course`目录下执行

```shell
go run main.go -file sample.xlsx
```

#### 导入云课堂课程

同样，进入`history_course`目录，运行go文件

```shell
go run main.go
```
