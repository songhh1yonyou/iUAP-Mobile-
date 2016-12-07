A.	Hybrid-HTML5框架图说明：
该模式指Summer版本Summer工程，在集成开发环境中，使用HTML5+CSS3+JavaScript技术，可利用平台提供的前端框架、原生交互接口，快速开发与原生应用相媲美的移动应用。模糊native 和web的界限。
Hybrid-HTML5：建议使用h5做展现，使用平台提供的原生服务做交互。
		APP最外层是Native的壳，包括：
•Native Container：APP最终运行在Native 容器中，也正是Native容器的存在，平台提供的原生交互、调用设备服务等才得以起作用。
•WebView render Mobile UI：使用h5做展现部分，使用webview渲染UI，包括HTML、CSS、JavaScript
•bridge：webview渲染 的UI中 JS与Native Container间通信桥梁。
B.	优势：
展现用h5，可广泛利用开源框架；交互用原生，使用户体验更好，模糊native与web 的界限。
