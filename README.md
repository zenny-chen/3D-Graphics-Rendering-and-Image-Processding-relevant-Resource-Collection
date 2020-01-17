# 3D-Graphics-Rendering-and-Image-Processding-relevant-Resource-Collection
3D图形渲染及数字图像处理算法相关文集

<br />

1. [彩阳的CSDN博客](http://blog.csdn.net/jiangcaiyang123/article/category/1246122)
1. [OpenGL缓冲区对象之UBO](https://blog.csdn.net/csxiaoshui/article/details/32101977)
1. [使用计算着色器（Compute Shader）模拟粒子效果【OpenGL】](https://blog.csdn.net/panda1234lee/article/details/70521910)
1. [Performance Tunning for Tile-Based Architecture
Tile-Based架构下的性能调校](http://www.cnblogs.com/gameknife/p/3515714.html)
1. [FBO中多重采样抗锯齿（MSAA：MultiSampling Anti-Aliasing）](http://blog.csdn.net/pizi0475/article/details/7932915)
1. [PVR/PVRTC解压源码](https://github.com/Volcore/quickpvr)
1. [png转换成pvz源代码](https://github.com/cjhanson/PNGPOTimizer/tree/CCZ)
1. [移动平台游戏的性能优化](http://www.csdn.net/article/2015-05-27/2824785)
1. [侯思松博客](http://blog.csdn.net/housisong)
1. [数字图像处理 傅里叶变换](http://blog.csdn.net/zkp0601/article/details/41295283)
1. [mg博客](https://www.cnblogs.com/minggoddess/)
1. [Render graphs and Vulkan — a deep dive](http://themaister.net/blog/2017/08/15/render-graphs-and-vulkan-a-deep-dive/)
1. [OpenGL ES3使用MSAA（多重采样抗锯齿）的方法](https://www.cnblogs.com/zenny-chen/p/5058575.html)
1. 这篇文章是关于颜色混合半透明效果讲解得比较透彻的：[GLSL Programming/GLUT/Transparency](https://en.wikibooks.org/wiki/GLSL_Programming/GLUT/Transparency)
这里需要注意的是，由于iOS中的图形流水线机制是将从片段着色器输出的像素颜色值，在送到颜色混合固定功能单元之前就已经预先乘了alpha值。这种情况下需要使用`glBlendFunc(GL_ONE, GL_ONE_MINUS_SRC_ALPHA)`来做颜色混合。
1. [OpenGL ES 2.0+ 如何设置点的大小](https://gamedev.stackexchange.com/questions/11095/opengl-es-2-0-point-sprites-size)
1.  [Point Sprites](http://www.informit.com/articles/article.aspx?p=770639&seqNum=7)
1. [Chapter 7. Sprites and Text](https://www.oreilly.com/library/view/iphone-3d-programming/9781449388133/ch07.html)
1. 在OpenGL ES 2.0以及之后，着色模式作为着色器语言中的**插值限定符**（**Interpolation Qualifiers**），使用`flat`或`smooth`来指定。默认缺省为`smooth`插值。
1. [android framebuffer和HAL以及显示系统](https://blog.csdn.net/wanglongwang201209/article/details/12616197)
1. [Android下Opengl ES实现单屏幕双眼显示](https://blog.csdn.net/u011371324/article/details/68946779)
1. [Advanced Graphics Programming Techniques](https://www.opengl.org/archives/resources/code/samples/sig99/advanced99/notes/notes.html)
1. [计算机视觉的计算几何及Python实现](https://www.toutiao.com/a6637430623361303053)
1. [Bit blit](https://en.wikipedia.org/wiki/Bit_blit)
1. [A simple Vulkan Compute example](http://www.duskborn.com/posts/a-simple-vulkan-compute-example/)
1. [GLSL \#include](https://www.gamedev.net/forums/topic/316061-glsl-include/)
1. [What are the key differences between Open Shader Language and GLSL](https://stackoverflow.com/questions/46093694/what-are-the-key-differences-between-open-shader-language-and-glsl)
1. [Arm Frame Buffer Compression (AFBC)](https://developer.arm.com/architectures/media-architectures/afbc)
1. [一步一步实现基于GPU的pathtracer（一）：基础](https://www.cnblogs.com/time-flow1024/p/6943508.html)
1. [一步一步实现基于GPU的pathtracer（二）：求交算法](https://www.cnblogs.com/time-flow1024/p/6944203.html)
1. [一步一步实现基于GPU的pathtracer（三）：path tracing 简述](https://www.cnblogs.com/time-flow1024/p/9974702.html)

<br />

以下为各个图形API的图形流水线

![1.png](https://github.com/zenny-chen/3D-Graphics-Rendering-and-Image-Processding-relevant-Resource-Collection/blob/master/1.png)

![2.png](https://github.com/zenny-chen/3D-Graphics-Rendering-and-Image-Processding-relevant-Resource-Collection/blob/master/2.png)

![3.png](https://github.com/zenny-chen/3D-Graphics-Rendering-and-Image-Processding-relevant-Resource-Collection/blob/master/3.png)

我们可以看到，OpenGL与OpenGL ES基本是一样的。此外，如果想了解OpenGL图形渲染流水线更为细节的情况，可参考此文：https://www.khronos.org/opengl/wiki/Rendering_Pipeline_Overview

<br />

## Pixel与Texel

***pixel***这个单词来源于**pix**与**element**的缩写，表示**图像元素**，因此简称**像素**。
同样，***texel***则是**texture**与**element**的缩写，表示**纹理元素**。


