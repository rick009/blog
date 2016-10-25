# xhprof使用记录

## xhprof_enable()

启动 xhprof 性能分析器 

## xhprof_disable()

停止 xhprof 性能分析器，并返回收集的性能数据，主要包括以下数据

XHPROF_FLAGS_CPU + XHPROF_FLAGS_MEMORY 模式

* ct：call times，调用次数
* wt：wall/wait time (ms)，等待时间
* cpu：CPU时间
* mu：memory usage (bytes)，内存使用量
* pmu：peak memory usage，内存使用峰值


