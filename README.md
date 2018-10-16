# 功能

在多台机器上执行命令

# 用法

```bash
Prun -r 'CSV-RANGE' 'COMMAND'
Prun -f HOSTSFILE 'COMMAND'
Prun -h
```

# 依赖

* pssh
* sshpass

# 使用前的环境配置

```bash
$ echo "YOUR-PASSWORD" > ~/.passwd
```

# 示例

```bash
$ Prun -r 'host1.example.com,host2.example.com' 'whoami'
$ cat hosts
host1.example.com
host2.example.com
$ Prun -f host 'whoami'
```
