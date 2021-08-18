# SynologyDrive 如何设置同步屏蔽选项

在 MacOS 系统下，访达里前往文件夹：`~/.SynologyDrive/data/session`

里面有数字文件夹，此数字文件夹对应的是创建同步项目的文件夹。

如要修改第一个同步项目的配置文件。

就依次找到 `数字/conf/blacklist.filter`

`blacklist.filter` 就是配置文件，编辑此文件。

在`[Directory]` 下 新增 `black_name = "node_modules"`

编辑文件：

```bash
bianxhdeMacBook-Pro:3 bianxh$ vi ~/.SynologyDrive/data/session/3/conf/blacklist.filter
```

更新如下内容，增加不同步的文件类型和文件夹：

```bash
[File]
black_ext = "tmp", "temp", "swp", "lnk", "pst"

max_size = 0

[Directory]
black_name = "target", "node_modules"
```

效果如下：
![20210818130250](http://bxh7425014.bianxh.top/img/20210818130250.png)
