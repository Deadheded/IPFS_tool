## 这是一个IPFS工具，用来测试网关可用性和预览文件。

## This is an IPFS tool to test the availability of the gateway and preview files.

支持ipfs hash和ipns地址
Support ipfs hash and ipns address Demo address

功能介绍

##Features

# Gateway

用于检测网关列表中网关的可用性以及对source view区块中指定路径的可达性。
Used to detect the availability of the gateway in the gateway list and the reachability of the specified path in the source view block.

当source view区域中的路径输入框有内容时，网关测试将尝试加载其内容的head来确定路径指定的文件在此网关上是否可达。
When there is content in the path input box in the source view area, the gateway test will try to load the head of the content to determine whether the file 
specified by the path is reachable on this gateway.

当打开的网页地址的hash部分中带有path参数时，Gateway区块将被移动到source view区块下方以便查看资源。
When there is a path parameter in the hash part of the opened webpage address, the Gateway block will be moved to the bottom of the source view block for viewing resources.

# Source view

用于查看指定路径的资源。
Used to view the resources of the specified path.

点击view按钮时将使用Gateway区块中的Current gateway的值作为网关尝试加载资源。
When you click the view button, the value of Current gateway in the Gateway block will be used as the gateway to try to load the resource.

点击test then view按钮将先进行网关检测然后尝试加载资源。
Click the test then view button to perform gateway detection and then try to load resources.

地址hash参数

# Address hash

path : 自动填入资源浏览区块的ipfs地址，并将自动测试网关和加载此路径。如/#path=Qmc3tpg69Dvk8V5PpyNgetcPma7Q8DaGqtUgBK7iwBwjrd
parameter path: automatically fill in the ipfs address of the resource browsing block, and automatically test the gateway and load this path. 
Such as /#path=Qmc3tpg69Dvk8V5PpyNgetcPma7Q8DaGqtUgBK7iwBwjrd gateway:

gateway : 指定为当前页面的默认网关，如果有path的话将使用此网关加载资源。如/#path=Qmc3tpg69Dvk8V5PpyNgetcPma7Q8DaGqtUgBK7iwBwjrd&gateway=https://ipfs.io
Specify as the default gateway of the current page. If there is a path, this gateway will be used to load resources. 
Such as /#path=Qmc3tpg69Dvk8V5PpyNgetcPma7Q8DaGqtUgBK7iwBwjrd&gateway=https://ipfs.io
