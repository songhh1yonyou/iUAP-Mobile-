虽然Hybrid开发模式流行，不代表native、web模式完全被代替。如native APP ：iOS Camera+， 还有比较流行的轻应用等。

iuap mobile平台面对移动开发模式的多元化的支持，可以用下图展示：

![](/assets/110.png)

可以分为三条分支：  
（1）    Native-UI：交叉编译式  
通过开发工具，使用HTML、CSS、JS开发，经过Build编译的过程生成APP。Build编译的过程是将HTML、CSS编译生成native UI的过程，所以运行时，其实加载的是iOS、Android原生的UI。  
//TODO  
这种方式，关于动作的加载，可参考《xXXXXX》。  
（2）    Hybrid-native：私有浏览器模式  
通过开发工具，使用HTML、CSS、JS开发，经过Build编译的过程生成APP。运行时：使用HTML、CSS、JS开发的资源可以通过私有浏览器与iOS、Android原生控件交互。

（3）    Web UI/Hybrid UI：Web APP  
通过开发工具，使用HTML、CSS、JS开发，也可引用开源的HTML框架，使用原生浏览器加载。最终发布形式为：轻应用（Light APP）。

三条分支对应的框架图：  
![](/assets/111.png)  
                                                                                     图i UAP Mobile Hybrid开发模式全景

