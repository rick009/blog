# xhprof使用记录

## xhprof_enable()

启动 xhprof 性能分析器 

### 参数

* flags

    分析添加额外信息的可选标记，主要有以下几种：
    * XHPROF_FLAGS_NO_BUILTINS=1
    * XHPROF_FLAGS_CPU=2
    * XHPROF_FLAGS_MEMORY=4

* options

    array 的可选选项，就是通过传递 'ignored_functions' 选项来忽略性能分析中的某些函数

## xhprof_disable()

停止 xhprof 性能分析器，并返回收集的性能数据，主要包括以下数据

XHPROF_FLAGS_CPU + XHPROF_FLAGS_MEMORY 模式

* ct：call times，调用次数
* wt：wall/wait time (ms)，等待时间
* cpu：CPU时间
* mu：memory usage (bytes)，内存使用量
* pmu：peak memory usage，内存使用峰值


