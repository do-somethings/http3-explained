# API

常规TCP程序最成功的要素之一便是标准化的套接字（socket）API。API功能定义良好，使用API能让你轻松地在各操作系统中移植TCP程序而保持一样的功能。

但在QUIC中情况不是这样的。QUIC没有标准API。

在QUIC中，你需要选择一个现存的实现库，并且一直使用它的API。这在某种程度上把应用“绑定”到了单一的库上。换库意味着使用另外的API，可能带来不小的工作量。

另外，QUIC一般在用户空间实现，所以它不像现存TCP和UDP的套接字API那样方便扩展。使用QUIC意味着选择了套接字API之外的另一种API。
