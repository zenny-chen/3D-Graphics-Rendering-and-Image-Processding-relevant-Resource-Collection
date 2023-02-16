# 3D Graphics Rendering and Image Processing relevant Resource Collection
3D图形渲染及数字图像处理算法相关文集

<br />

- [彩阳的CSDN博客](http://blog.csdn.net/jiangcaiyang123/article/category/1246122)
- [侯思松博客](http://blog.csdn.net/housisong)
- [mg博客](https://www.cnblogs.com/minggoddess/)
- [handyTOOL的简书OpenGL ES文集](https://www.jianshu.com/nb/11846847)
- [梁老师的博客园](https://www.cnblogs.com/len3d/)
- [Morgan McGuire](https://research.nvidia.com/person/morgan-mcguire?tdsourcetag=s_pcqq_aiomsg)
- [What exactly is a softlock?](https://gaming.stackexchange.com/questions/357095/what-exactly-is-a-softlock)
- [GPU渲染管线之旅（GPU渲染管线中的硬件实现）](https://www.zhihu.com/column/c_1265245746099941376)
- [OpenGL -- 屏幕成像和渲染原理解析](https://www.toutiao.com/article/7153963074285322791/)
- [图形学:名词解释](https://blog.csdn.net/hellotruth/article/details/40889701)
- [完美的视图旋转算法](https://www.cnblogs.com/len3d/p/5530401.html)
- [OpenGL缓冲区对象之UBO](https://blog.csdn.net/csxiaoshui/article/details/32101977)
- [Opengl入门系列- FBO的渲染到纹理的用法](https://blog.csdn.net/zangle260/article/details/40430929)
- [非常详细易懂的法线贴图(Normal Mapping)](https://blog.csdn.net/qq_26900671/article/details/79048727)
- [凹凸映射（Bump Map）实现原理](https://blog.csdn.net/archielau/article/details/9124341)
- [OpenGL调试技巧汇总](https://blog.csdn.net/zjz520yy/article/details/83034140)
- [Performance Tunning for Tile-Based Architecture Tile-Based架构下的性能调校](http://www.cnblogs.com/gameknife/p/3515714.html)
- [FBO中多重采样抗锯齿（MSAA：MultiSampling Anti-Aliasing）](http://blog.csdn.net/pizi0475/article/details/7932915)
- [WebGL2系列之多采样渲染缓冲对象](https://blog.csdn.net/netcy/article/details/95948811)
- [颜色空间——Gamma与线性颜色空间](https://www.cnblogs.com/guanzz/p/7416821.html)
- [一文理解 YUV](https://zhuanlan.zhihu.com/p/75735751)
- [PVR/PVRTC解压源码](https://github.com/Volcore/quickpvr)
- [png转换成pvz源代码](https://github.com/cjhanson/PNGPOTimizer/tree/CCZ)
- [移动平台游戏的性能优化](http://www.csdn.net/article/2015-05-27/2824785)
- [数字图像处理 傅里叶变换](http://blog.csdn.net/zkp0601/article/details/41295283)
- [轻量级隐写分析模型](https://www.toutiao.com/i6895918997670363651/)
- [D3D渲染技术之纹理](https://blog.csdn.net/jxw167/article/details/82824741)

在Direct3D的颜色表示中，**_SNORM** 后缀表示带符号的规格化的整数；它在一个资源中表示为一个带符号的整型数据，且在shader中被解释为一个带符号的范围在[-1, 1]的浮点值。对于以2的补码形式的整数来说，最大值为1.0f（一个5位的二进制数01111映射为1.0f），最小值是-1.0f（一个5位二进制数10000映射为-1.0f）。此外，第二小的数也被映射为-1.0f（一个5位的二进制数10001被映射为-1.0f）。整数结果的表示被均匀地分布在(-1.0 ... 0.0f) 浮点值范围内，且相对的其补集表示的数在 (0.0f ... 1.0f) 范围内。**_UNORM** 后缀表示无符号规格化整数；它在一个资源中被解释为一个无符号整数，且在shader中被解释为一个无符号的规格化的浮点数，范围在[0, 1]内。所有0被映射为0.0f，而所有的1被映射为1.0f。一个均匀分布的浮点值序列被表示为从0.0f到1.0f。例如，一个2比特的UNORM（00, 01, 10, 11）分别表示为：0.0f，1/3，2/3及1.0f。

在Vulkan中，**SSCALED** 后缀表示带符号的整数；它在主机端的资源中表示一个带符号的整数，且在shader中被解释为一个与主机端的值相对应的带符号的浮点数。**USCALED** 后缀表示无符号的整数；它在主机端的资源中表示一个无符号的整数，且在shader中被解释为一个与主机端的值相对应的无符号的浮点数。

详情可见：[VK_FORMAT_R8G8B8A8_[U/S]SCALED vs VK_FORMAT_A8B8G8R8_[U/S]SCALED_PACK32 ?](https://community.khronos.org/t/vk-format-r8g8b8a8-u-s-scaled-vs-vk-format-a8b8g8r8-u-s-scaled-pack32/6769)

- [Tutorial 12 : OpenGL Extensions](http://www.opengl-tutorial.org/intermediate-tutorials/tutorial-12-opengl-extensions/)
- [OpenGL ES3使用MSAA（多重采样抗锯齿）的方法](https://www.cnblogs.com/zenny-chen/p/5058575.html)
- 这篇文章是关于颜色混合半透明效果讲解得比较透彻的：[GLSL Programming/GLUT/Transparency](https://en.wikibooks.org/wiki/GLSL_Programming/GLUT/Transparency)
这里需要注意的是，由于iOS中的图形流水线机制是将从片段着色器输出的像素颜色值，在送到颜色混合固定功能单元之前就已经预先乘了alpha值。这种情况下需要使用`glBlendFunc(GL_ONE, GL_ONE_MINUS_SRC_ALPHA)`来做颜色混合。
- [opengl es2 premultiplied vs straight alpha + blending](https://stackoverflow.com/questions/19674740/opengl-es2-premultiplied-vs-straight-alpha-blending)
- [Order-Independent Transparency](https://www.cnblogs.com/mavaL/p/3525890.html)
- [OpenGL Dual Source Blending](https://www.khronos.org/opengl/wiki/Blending)
- [OpenGL ES 2.0+ 如何设置点的大小](https://gamedev.stackexchange.com/questions/11095/opengl-es-2-0-point-sprites-size)
- [Point Sprites](http://www.informit.com/articles/article.aspx?p=770639&seqNum=7)
- [Chapter 7. Sprites and Text](https://www.oreilly.com/library/view/iphone-3d-programming/9781449388133/ch07.html)
- [OpenGL Interpolation Qualifiers (GLSL)](https://www.geeks3d.com/20130514/opengl-interpolation-qualifiers-glsl-tutorial/)
- [gluLookAt](https://www.khronos.org/registry/OpenGL-Refpages/gl2.1/xhtml/gluLookAt.xml)
- [GluLookAt code](https://www.khronos.org/opengl/wiki/GluLookAt_code)
- [从零开始的Vulkan](https://www.zhihu.com/column/c_1542671286655873024)
- [一起学Vulkan图形开发](https://www.zhihu.com/column/chenyong2vulkan)
- [Render graphs and Vulkan — a deep dive](http://themaister.net/blog/2017/08/15/render-graphs-and-vulkan-a-deep-dive/)
- [Vulkan坐标系](https://zhuanlan.zhihu.com/p/97496535)
- [Vulkan 右手坐标系见解](https://zhuanlan.zhihu.com/p/365830760)
- [How to use a vulkan sampler with unnormalized texture-coordinates?](https://stackoverflow.com/questions/65790303/how-to-use-a-vulkan-sampler-with-unnormalized-texture-coordinates-without-trig)
- [Vulkan查询支持哪些图像形式的VkFormat——vkGetPhysicalDeviceFormatProperties](https://registry.khronos.org/vulkan/specs/1.3-extensions/man/html/vkGetPhysicalDeviceFormatProperties.html)
- [Vulkan查询支持哪些纹理采样格式的VkFormat——vkGetPhysicalDeviceImageFormatProperties](https://registry.khronos.org/vulkan/specs/1.3-extensions/man/html/vkGetPhysicalDeviceImageFormatProperties.html)
- [Vulkan中的同步与缓存控制](https://zhuanlan.zhihu.com/p/161619652)
- [\[译\]Vulkan教程(23)暂存buffer](https://www.cnblogs.com/bitzhuwei/p/Vulkan-Tutoria-23-Staging-buffer.html)
- [Vulkan Mobile Best Practices - Management of Command Buffers and Multi-Threaded Recording](https://community.arm.com/arm-community-blogs/b/graphics-gaming-and-vr-blog/posts/vulkan-mobile-best-practices-and-management)
- [从Vulkan API看Shader的数据绑定机制](https://zhuanlan.zhihu.com/p/111882744)
- [Vulkan推荐用法(三星设备)](https://zhuanlan.zhihu.com/p/97321638)
- [vulkan_延迟渲染](https://blog.csdn.net/qq_35312463/article/details/105878760)
- [从零开始的Vulkan（附一）：多Subpass实现延迟渲染](https://zhuanlan.zhihu.com/p/558644452)
- [A simple Vulkan Compute example](http://www.duskborn.com/posts/a-simple-vulkan-compute-example/)
- [\[vulkan\] compute shader](https://zhuanlan.zhihu.com/p/56106712)
- [使用计算着色器（Compute Shader）模拟粒子效果【OpenGL】](https://blog.csdn.net/panda1234lee/article/details/70521910)
- [OpenGL ES3.1使用计算着色器（Compute Shader）](https://blog.csdn.net/qq_39561000/article/details/103112147)
- [同步连续的OpenGL Compute Shader调用](https://qastack.cn/computergraphics/400/synchronizing-successive-opengl-compute-shader-invocations)
- [Would love to see optional Geometry Shaders](https://github.com/gpuweb/gpuweb/issues/1239)
- [【OpenGL】笔记二十七、几何着色器](https://blog.csdn.net/ycrsw/article/details/125128835)
- [OpenGL之几何着色器(Geometry Shader)详解](https://blog.csdn.net/What_can_you_do/article/details/128255831)
- [浅谈OpenGL之DSA](https://www.cnblogs.com/hellobb/p/13943969.html)
- [OpenGL三维纹理坐标](http://blog.sina.com.cn/s/blog_687960370101gyh8.html)
- [OpenGL版本低于4.5的glBindTextureUnit的替代品?](http://ask.sov5.cn/q/xaqaFk3Esa)
- [OpenGL之——多纹理，混合纹理设置渲染](https://blog.csdn.net/qq_35294564/article/details/86546797)
- [Issue with RGBA32F texture format and mipmapping using OpenGL ES 3.0](https://stackoverflow.com/questions/44754479/issue-with-rgba32f-texture-format-and-mipmapping-using-opengl-es-3-0)
- [Render to half float texture](https://stackoverflow.com/questions/23253497/render-to-half-float-texture)
- [Data Type \(GLSL\)](https://www.khronos.org/opengl/wiki/Data_Type_\(GLSL\))（其中包含了结构体类型 **`struct`**）
- GLSL中，结构体必须至少含有一个成员声明。成员声明符可以包含精度限定符，但不能使用其他限定符，否则会导致编译时错误。GLSL中的结构体不支持位域（**bit fields**）。成员的类型必须是已经定义过的（不允许存在不完整类型）。如果成员声明包含了一个初始化器，那么会产生编译时错误。如果成员是一个数组，那么它必须具有一个指定的非零大小，且用于指定该大小的表达式必须是一个 **整数常量表达式**（[Constant Expressions](https://registry.khronos.org/OpenGL/specs/gl/GLSLangSpec.4.60.html#constant-expressions)）。
- [Interface Block \(GLSL\)](https://www.khronos.org/opengl/wiki/Interface_Block_\(GLSL\))
- [OpenGL Image Load Store Wiki](https://www.khronos.org/opengl/wiki/Image_Load_Store)
- Khronos OpenGL官方文档中关于描述的 **`gbufferImage`** 类型，实际所对应的类型为：**`imageBuffer`**、**`iimageBuffer`** 和 **`uimageBuffer`**。该类型对应于Vulkan中具有 **`VK_BUFFER_USAGE_STORAGE_TEXEL_BUFFER_BIT`** usage的 **`VkBuffer`**。同时在使用此buffer时需要结合 **`VkBufferView`** 一起使用。
- [Trouble with imageStore\(\) \(OpenGL 4.3\)](https://stackoverflow.com/questions/14285849/trouble-with-imagestore-opengl-4-3) （In desktop OpenGL, it is perfectly legal to upload floating-point data to a normalized integer texture; OpenGL is expected to convert the data as best it can. ES doesn't do conversions, so it has to change the internal format (the third parameter) to match the data.）
- [Can't access fbo attached texture in GLSL compute shader with gimage2D](https://stackoverflow.com/questions/22947896/cant-access-fbo-attached-texture-in-glsl-compute-shader-with-gimage2d)
- [Vulkan input attachments and sub passes](https://www.saschawillems.de/blog/2018/07/19/vulkan-input-attachments-and-sub-passes/)
- [Input Attachments - reading random location? Read/Write in same pass?](https://community.khronos.org/t/input-attachments-reading-random-location-read-write-in-same-pass/7035)
- 多个color attachment的输出：
```glsl
#version 450 core
layout(location = 0) out vec4 color_out;
layout(location = 1) out vec4 color_out1;
void main(void)
{
    color_out = vec4(0.0, 0.5, 0.0, 0.8);
    color_out1 = vec4(1.0, 1.0, 1.0, 1.0);
}
```
- [Precise Qualifier in GLSL and NVIDIA GeForce Cards](https://www.geeks3d.com/20120106/precise-qualifier-in-glsl-and-nvidia-geforce-cards/)
- [OpenGL 图像的加载和存储](https://blog.csdn.net/dayenglish/article/details/51439296)
- [OpenGL图像\(image\)](https://blog.csdn.net/qq_16555407/article/details/84307374)
- [difference between glTextureBarrier\(\) and glMemoryBarrier\(GL_TEXTURE_FETCH_BARRIER_BIT\)](https://stackoverflow.com/questions/37448712/difference-between-gltexturebarrier-and-glmemorybarriergl-texture-fetch-barri)
- [Vertex Rendering](https://www.khronos.org/opengl/wiki/Vertex_Rendering)
- [Early Fragment Test](https://www.khronos.org/opengl/wiki/Early_Fragment_Test)
- [Primitive Restart and OpenGL Interoperability](https://www.codeproject.com/articles/201263/part-6-primitive-restart-and-opengl-interoperabili)
- [OpenGL ES 3.0: 图元重启\(Primitive restart\)](https://www.cnblogs.com/psklf/p/5750783.html)
- [OpenGL 图元重启](https://blog.csdn.net/yulinxx/article/details/77896541)
- [2D变3D，视角随意换，神还原高清立体感，还是不用3D建模的那种 | 代码数据开源](https://mp.weixin.qq.com/s/zz3WQvnwoGLg58SCRn7YjA)
- [android framebuffer和HAL以及显示系统](https://blog.csdn.net/wanglongwang201209/article/details/12616197)
- [Android下Opengl ES实现单屏幕双眼显示](https://blog.csdn.net/u011371324/article/details/68946779)
- [Advanced Graphics Programming Techniques](https://www.opengl.org/archives/resources/code/samples/sig99/advanced99/notes/notes.html)
- [计算机视觉的计算几何及Python实现](https://www.toutiao.com/a6637430623361303053)
- [Bit blit](https://en.wikipedia.org/wiki/Bit_blit)
- [GLSL \#include](https://www.gamedev.net/forums/topic/316061-glsl-include/)
- [What are the key differences between Open Shader Language and GLSL](https://stackoverflow.com/questions/46093694/what-are-the-key-differences-between-open-shader-language-and-glsl)
- [Arm Frame Buffer Compression (AFBC)](https://developer.arm.com/architectures/media-architectures/afbc)
- [一步一步实现基于GPU的pathtracer（一）：基础](https://www.cnblogs.com/time-flow1024/p/6943508.html)
- [一步一步实现基于GPU的pathtracer（二）：求交算法](https://www.cnblogs.com/time-flow1024/p/6944203.html)
- [一步一步实现基于GPU的pathtracer（三）：path tracing 简述](https://www.cnblogs.com/time-flow1024/p/9974702.html)
- [Path Tracing](https://www.jianshu.com/p/428317cd522a)
- [对pathtracing的一些个人理解](https://www.cnblogs.com/time-flow1024/p/6844208.html)
- [什么是路径追踪？](https://www.toutiao.com/article/7121909050081542688/)
- [光线追踪—层次包围盒（ Bounding Volume Hierarchies ）](https://blog.csdn.net/sunshine543123/article/details/107041122)
- [如果想在GPU里软件方式计算射线和场景加速求交，SDF和BVH哪个好，各有什么优缺点？](https://www.zhihu.com/question/476683981)
- [UE4 Real-time Hair Advances](https://www.fxguide.com/fxfeatured/ue4-real-time-hair-advances/)
- [UE5 Lumen原理介绍](https://zhuanlan.zhihu.com/p/380720641)
- [UE5 Nanite原理介绍](https://zhuanlan.zhihu.com/p/393930818)
- [UE5渲染技术简介：Nanite篇](https://zhuanlan.zhihu.com/p/382687738)
- [动画电影LookDev流程科普](https://zhuanlan.zhihu.com/p/407833635)
- [Introducing Learned Motion Matching](https://montreal.ubisoft.com/en/introducing-learned-motion-matching/)
- [Reflection Probe](https://www.jianshu.com/p/585dd805c137)
- [各向异性（anisotropic）浅提](https://blog.csdn.net/YuYunTan/article/details/84348037)
- [Shader Anisotropic 各项异性](https://blog.csdn.net/baidu_16312167/article/details/75527961)
- [Tile-Based Deferred Shading](https://zhuanlan.zhihu.com/p/85447953)
- [图形引擎实战：HDRP移动版高清渲染管线改造](https://zhuanlan.zhihu.com/p/567981404)
- [1.HDRP入门](https://zhuanlan.zhihu.com/p/458453634)
- [Unity上怎么在移动端使用Render pass实现高性能的延迟着色？](https://www.zhihu.com/question/485735429)
- [延迟着色和Forward+在移动端各有什么利弊？](https://www.zhihu.com/question/487242931)
- [OpenGL HDR](https://learnopengl.com/Advanced-Lighting/HDR)
- [Phong 光照模型（镜面反射）](https://www.cnblogs.com/jqm304775992/p/4890634.html)
- [Mipmapping with Bidirectional Techniques](https://blog.yiningkarlli.com/2018/10/bidirectional-mipmap.html)
- [Bidirectional reflectance distribution function](https://en.wikipedia.org/wiki/Bidirectional_reflectance_distribution_function)
- [BRDF Importance Sampling for Polygonal Lights](https://momentsingraphics.de/Siggraph2021.html)
- [这是我们要的未来 英伟达RTX光线追踪技术解析](https://www.toutiao.com/i6768787614779572743/)
- [Ray Tracing In Vulkan（Vulkan中的光线追踪）](https://zhuanlan.zhihu.com/p/114920256)
- [DirectX Raytracing（DXR） functional Spec阅读笔记+注解](https://zhuanlan.zhihu.com/p/34894883)
- [更快更清晰！NVIDIA首次实现SDF实时渲染，速度提升3个数量级](https://www.toutiao.com/i6924108185934660110/)
- [Deep Rendering](https://studios.disneyresearch.com/deep-rendering/)
- [张心欣破Nanite招数于此](https://zhuanlan.zhihu.com/p/140943267)
- [CG技术的转折点，算法TD的觉醒路](https://mp.weixin.qq.com/s?__biz=MzU2MTU4MTc1Ng==&mid=2247617154&idx=2&sn=7aad0ddbc6aa74752ee3b04cc36d1b42&chksm=fc75d151cb02584760362b56f52eee81ed670da4398a46bfd8d3e1f0c800d8319d362ab22ad3&mpshare=1&scene=23)
- [GPU-Motunui](https://www.render-blog.com/)
- [OpenSubDiv](http://graphics.pixar.com/opensubdiv/docs/intro.html)
- [开源库 OpenVDB获得过奥斯卡奖的开源 C++ 库加入ASWF](https://www.cgspread.com/9867.html)（VDB即：**Volumetric Database**）
- [Arnold Documentation](https://www.arnoldrenderer.com/arnold/documentation/)
- [\[Arnold\] Standins and the ASS file cache](https://docs.arnoldrenderer.com/plugins/servlet/mobile#content/view/19205227)
- [Arnold(C4DToA)阿诺德渲染教程(111)：Arnold体系架构、设计理念、指导思想、技术内幕等 来自Solid Angle开发团队 最新的文献指南](https://www.btbat.com/10349.html/comment-page-11)
- [Maya Release GPU memory for unused textures](https://knowledge.autodesk.com/support/maya/learn-explore/caas/CloudHelp/cloudhelp/2016/ENU/Maya/files/GUID-74599EBE-1DC5-4ECE-86C0-A0216ABE0794-htm.html)
- [maya文件路径变量环境变量](https://blog.csdn.net/tian0000hai/article/details/90608132)

<br />

### OpenGL中对各种四元向量数据类型的分量标识
- 顶点坐标：x, y, z, w
- 纹理坐标：s, t, r, q
- 颜色通道：r, g, b, a

<br />

### PS2模拟器相关技术

- [Alpha Testing in the GS world](https://pcsx2.net/developer-blog/279-alpha-testing-gs-world.html)
- [Setting up Windows version](https://wiki.pcsx2.net/Setting_up_Windows_version)

<br />

### 以下为各个图形API的图形流水线

![1.png](https://github.com/zenny-chen/3D-Graphics-Rendering-and-Image-Processding-relevant-Resource-Collection/blob/master/1.png)

![2.png](https://github.com/zenny-chen/3D-Graphics-Rendering-and-Image-Processding-relevant-Resource-Collection/blob/master/2.png)

![3.png](https://github.com/zenny-chen/3D-Graphics-Rendering-and-Image-Processding-relevant-Resource-Collection/blob/master/3.png)

我们可以看到，OpenGL与OpenGL ES基本是一样的。此外，如果想了解OpenGL图形渲染流水线更为细节的情况，可参考此文：https://www.khronos.org/opengl/wiki/Rendering_Pipeline_Overview

<br />

## Pixel与Texel

***pixel***这个单词来源于**pix**与**element**的缩写，表示**图像元素**，因此简称**像素**。
同样，***texel***则是**texture**与**element**的缩写，表示**纹理元素**。


