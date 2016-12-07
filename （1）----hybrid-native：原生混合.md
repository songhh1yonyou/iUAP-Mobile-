A.	Hybrid-Native框架图说明：
该模式指原版本DSL工程，在集成开发环境中使用设计器以拖拉拽的形式设计UI模型、数据模型；以JS调用平台封装的设备服务、工具服务等；通过编译、打包过程生成APP。
	APP最外层是Native的壳，包括：
•Native render Mobile UI：工程编译，使用设计器生成UI最终编译成原生UI；APP运行态：使用原生渲染
•JavaScript：开发者使用JS调用的方法，包括设备服务、工具服务等；APP运行态：使用WebView加载相应的JS逻辑。
•bridge：原生UI与webview 加载JS逻辑间通信桥梁。
B.	优势：
UI Native 化，更接近原生，也称为：semi-hybrid

