**canvas**：

1.作用：用于图形的绘制，通过脚本（通常是js）来完成。它只是一个图形容器。可以用来完成动画、游戏、图表、图像处理等原来需要flash完成的一些功能。
创建canvas元素：
<canvas id="can" width="800"  height="600">不支持Canvas</canvas>
**不建议使用CSS样式指定宽度和高度。**

HTML DOM 中getContext(contextID) 的方法： 返回一个用在画布上绘图的环境。contextID当前唯一合法值是"2d",它指定了一个二维绘图，并且导致这个方法返回一个环境对象，该对象导出一个二维绘图api。

**svg**

1.是一个可缩放的矢量图形，它使用xml格式定义图像，svg是用xml来描述二维图形和绘图程序的语言；是万维网联盟的标准（网络矢量图形标准）。
2.优势：
- 与JPEG和GIF图像比，尺寸更小，切可压缩性更强。
- 可伸缩
- 在任何分辨下都都可以高质量打印
- 可在图片质量不下降的情况下被放大
- svg图像中的文本是可选的，同时也是可以搜索的（很适合制作地图==）
- svg可以和Java一起运行
- svg文件是纯粹的xml
- 所有的浏览器都是支持svg文件

svg可以通过<embed>、<object>或者<iframe>这些标签嵌入HTML文档。

两者区别：
1.canvas有一个基于js的绘图api,er svg和vml使用一个xml文档来描述绘图。SVG 绘图很容易编辑与生成，但功能明显要弱一些。

**webGL**
1.是一种3D绘图标准，这种技术标准允许把js和OpenGL ES2.0结合在一起，通过OpenGL ES 2.0的一个js绑定，WebGL可以为HTML5 CAnvas提供硬件3D加速渲染。这样就可以根据系统显卡在浏览器中更流畅展示3D场景和模型、创建复杂的导航和数据视觉化。

2.WebGL完美地解决了现有的Web交互式三维动画的两个问题：

第一，它通过HTML脚本本身实现Web交互式三维动画的制作，无需任何浏览器插件支持;
第二，它利用底层的图形硬件加速功能进行的图形渲染，是通过统一的、标准的、跨平台的OpenGL接口实现的。