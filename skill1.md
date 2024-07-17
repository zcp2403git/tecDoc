技能

·组件依赖管理
====
+ 组件依赖打平 
  - 解决循环依赖，解决项目A依赖项目B,项目
+ B依赖项目C,项目C依赖项目A
·切换aar和源码
。依赖变更
bytex检测组件api完整性
，依赖版本强制锁定
。通过拉取预构建的二进制aar文件，缩短构建时
间
包体积优化
动态化/插件化--落地人脸识别，扫码库、3d3
0
擎等三方组件
官方动态化方案Android app bundle-爱奇艺插
件化框架
，资源加载原理-通过反射assetsManager，
调用addPath方法添加路径,重写activity的
getResource方法
。资源id生成规则:packageld+typelD
代码加载原理
。单classloader-反射插入宿主
多classloader-反射classloader
parent，利用classloader双亲委托
。插件化方案 shadow
耦合形态
·独立形态
。R文件去除
:getstatic修改为LDC指令。无用代码下线通过classloader收集哪些class被调用·通过编译选项 -shrink 移除无用代码和资源编译优化常量内联、access方法内联、get-set内联删除行号
0
。资源优化
图片上云
图片png编译期自动转webp
。其他
·短方法内联、
、access方法内联
·log方法删除、行号删除
热修复平台搭建
。
o tinker
权限管理
内部发布、灰度、全量
日志库端到端
。客户端日志库
mmap--MappedByteBuffer
上传到网头(a0
。业务后端
。通过hlog指定topic
。后端
网关根据上传的type转发topic
，flink消费绑定日志topic，存储到ck表
·ck建表--增加索引--布降过滤器索引
物化视图
前端
0
查询ck表
。为什么不用es用ck
。ClickHouse采用SQL语法，比ES的
DSL更加简单，新用户学习成本更
低。
·ClickHouse稳定性更高，运维成本更
岔
clickhouse支持物化视图
。云端一体
。云端
。客户端
mvi模式
·单向数据流:通过单向的数据流动可确保状态的一致性和可预测性。响应式特性:MVI利用响应式编程的思想，通过传递意图的方式实现了对状态变化的高效处理。。targetSDK升级整理targetSDk廾级影响点输出帮助指南、FAQ，协助业务线解决问题通过自研的匹配api脚本全局扫码字节码输出调用链表格，按业务线分组整理组件列表表格，按业务线归属，避免遗漏。性能优化
。启动优化·App启动任务框架·启动依赖管理--有向无环图显性的运行期依赖把之前启动逻辑的“隐性依赖”完全暴露在阳光之下，改启动逻辑不用提心吊胆;线程管控，网络接口合并，布局预加载、数据预加载AsyncLayoutlnflater 用于进行 xml 的异步加载，但很容易出现锁的问题甚至导致了更多的耗时。防劣化监控平台;·APM抓取耗时方法，视频录制回放稳定性-App启动容灾崩溃自动防护。。启动防护页。启动崩溃监控埋点统计+grafana。App自动降级灰度降级容错兜底逻辑标记清除0异常排查
bugreport-崩溃、ANR
