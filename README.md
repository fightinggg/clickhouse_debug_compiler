# clickhouse_debug_compiler
这个项目帮助用户构建一个专用的clickhouse学习环境

# 如何使用
## step.1 进入容器

```
docker run --privileged  -d  -p 2222:22 -v $HOME:/root --name clickhouse_debug_env fightinggg/clickhouse_debug_env:master
```

## step.2 开始编译
这一步目前由于clickhouse编译时间过长，导致github无法完成编译任务，目前放到用户这边自己编译
```
cd /Clickhouse/build && build
```

## step.3 运行clickhouse
```
program/clickhouse-server
```

## step.4 从远程gdb连接clickhouse

