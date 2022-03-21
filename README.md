# grouper

一个将本地某个指定的文件夹上传到云oss存储的服务，
特别是我在使用Axure制作PRD文档之后，需要将其与团队共享。

这虽然有很多方法，比如：Axure自带的云、国内的pmdaniu、axurehub等；
或者你可以改用墨刀、xiaopiao、mastergo等原型设计共享工具；
甚至你可以使用一些协同设计工具，说实话我不太喜欢那些在浏览器就能运行的设计工具，
他们很方便很轻量，但是我想说"有了在线PS工具，为什么你还要下载客户端"？
除了习惯已经养成外，web工具缺乏桌面程序的厚重，小手一抖返回上一页了over。

如果你和我一样，需要将Axure生成的文件夹上传托管，grouper或许是个不错的选择。
（ps: 名字怪怪的，或许有其他名字？）

编译命令
- go build -o grouper main.go

（ps: 如果你觉得名字不好听或不好写，你可以自行命名 -o 的参数）

编译后，使用命令：
- ./uper -h 查看帮助
- ./uper -n=name 指定项目名称，同样这也是你的**文件路径**和访问路径，并且文件夹存在
- ./uper -p=. 指定项目本地路径，默认为当前文件夹，可以不写

（ps: 如果你不喜欢使用"./"，你可以将其添加至环境变量）
