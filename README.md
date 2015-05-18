![rDSN](https://raw.githubusercontent.com/Microsoft/rDSN/master/resources/rdsn.jpg)
Robust Distributed System Nucleus (rDSN) is an open framework for quickly building and managing high performance and robust distributed systems. An early version of rDSN has been used in Bing for building a distributed data service, and the system has been online and running well. Based on the feedbacks, rDSN is improved and now [made public](http://research.microsoft.com/en-us/projects/rdsn/default.aspx) with the MIT open source license. The idea is a [coherent and principled design](https://github.com/Microsoft/rDSN/wiki/Design-Rational) that distributed applications, tools, and frameworks can be developed independently and later on integrated (almost) transparently. Following are some highlights for different audience of this framework.

I am a [developer](https://github.com/Microsoft/rDSN#developers-a-framework-for-quickly-building-and-managing-high-performance-and-robust-distributed-systems-see-tutorial)  |   [researcher](https://github.com/Microsoft/rDSN#researchers-and-tool-oriented-developers-a-tool-platform-which-eases-tool-development-and-enables-transparent-integration-with-upper-applications)  |   [student](https://github.com/Microsoft/rDSN#students-a-distributed-system-learning-platform-where-you-can-easily-simplify-understand-and-manipulate-a-system-see-tutorial) =>

##### Developers: a framework for quickly building and managing high performance and robust distributed systems. (see [Tutorial](https://github.com/Microsoft/rDSN/wiki/A-Tutorial-for-Developers))

* flexible programming and deployment
 * multiple-platform support (Linux, Windows, Mac)
 * [quick prototyping](https://github.com/Microsoft/rDSN/wiki/A-Tutorial-for-Developers#step-1-write-the-service-interface-and-run) via code generation with Thrift and Protocol Buffer, extensible for others
 * [enhanced RPC library](https://github.com/Microsoft/rDSN/wiki/A-Tutorial-for-Developers#step-14-connect-the-service-with-other-languages-optional) with multi-port, multi-channel, multi-language-client support
 * flexible to [plugin your own](https://github.com/Microsoft/rDSN/wiki/Tool-API:-Component-Providers,-Join-Points,-and-State-Extensions#component-providers) low level constructs (network, logging, task queue, lock, etc.)
 * single executable, multiple role, multiple instance [deployment](https://github.com/Microsoft/rDSN/wiki/A-Tutorial-for-Developers#step-3-run-with-the-native-runtime-and-deployment)
* **built-in three-layer support from [a growing set of tools and frameworks](https://github.com/Microsoft/rDSN/wiki/Available-Tools,-Policies-and-Frameworks)**
 * layer 1: single node tools and policies: simulation, fault injection, tracing, profiling, replay, throttling, ...
 ![rDSN-layer1](https://raw.githubusercontent.com/Microsoft/rDSN/master/resources/rdsn-layer1.jpg)
 * layer 2: from single node to a partitioned and/or replicated service
 ![rDSN-layer2](https://raw.githubusercontent.com/Microsoft/rDSN/master/resources/rdsn-layer2.jpg)
 * layer 3: from single service to workflow across multiple services to handle end-to-end incoming workloads (coming later)

##### Researchers and tool-oriented developers: a tool platform which eases tool development and enables transparent integration with upper applications.

* reliably expose dependencies and non-determinisms in upper systems to the underlying tools at a semantic-rich level (i.e., task)
 * completeness made easy for tools
 * reduced state space for tools to handle
 * easier to map tool results to application logic
* dedicated Tool API for tool and runtime policy development
* transparent integration of the tools with the upper applications to make real impact

##### Students: a distributed system learning platform where you can easily simplify, understand and manipulate a system. (see [Tutorial](https://github.com/Microsoft/rDSN/wiki/A-Tutorial-for-Developers))

* configurable system complexity to learn step by step
 * single thread to multiple threads
 * synchronous and reliable messages to asynchronous and unreliable ones
* easy test, debug, and monitoring for system understanding, as with the developers
* easy further tool development, as with the researchers

***

### Further Links

* [Installation](https://github.com/Microsoft/rDSN/wiki/Installation)
* [Tutorial](https://github.com/Microsoft/rDSN/wiki/A-Tutorial-for-Developers)
* [Built-in Tools, Runtime Policies and Distributed Frameworks](https://github.com/Microsoft/rDSN/wiki/Available-Tools,-Policies-and-Frameworks)
* [Extend rDSN] (https://github.com/Microsoft/rDSN/wiki/Tool-API:-Component-Providers,-Join-Points,-and-State-Extensions)
* [Programming Rules and FAQ](https://github.com/Microsoft/rDSN/wiki/Programming-Rules-and-FAQ)
* [Contribute to rDSN](https://github.com/Microsoft/rDSN/wiki/Contribute)

