
#关于github项目与学习的概要
>PS:本文基本都是通过项目实战来学习的

>分三篇: [攻坚篇](#anchor),`项目介绍篇`,`插件篇`

******


* <span id = "anchor">攻坚篇</span>
    * [PorterDuffXfermode的正确使用方式](https://github.com/luhaoaimama1/zone-sdk/blob/master/README-Xfermode.md)
    * [NestedScrolling Child与Parent的实例学习](https://github.com/luhaoaimama1/zone-sdk/blob/master/README-NestedScrolling.md)

        >页面效果:zone-sdk:->onTouch事件传递与其辅助类的研究->即可看到;
    * [打造无敌解耦的BaseActivity](https://github.com/luhaoaimama1/zone-sdk/blob/master/README-BaseActivity.md)

        >解耦，各司其职。拍照等涉及onActivityResult的封装
    * [Android 屏幕适配终极解决方案（包含生成程序dp sp与解决方案）](https://github.com/luhaoaimama1/AnnotationStudy/blob/master/README.md)

        >[ldpi,mdip,hdpi,xhdip,xxhdpi生成DP](https://github.com/luhaoaimama1/JavaZone/blob/master/JavaTest_Zone/src/%E9%80%82%E9%85%8D/MakeXml_Dp.java)

        >[ldpi,mdip,hdpi,xhdip,xxhdpi生成SP](https://github.com/luhaoaimama1/JavaZone/blob/master/JavaTest_Zone/src/%E9%80%82%E9%85%8D/MakeXml_Sp.java)
        ```
        ldpi("values-ldpi",0.75F),mdpi("values-mdpi",1.0F),hdpi("values-hdpi",1.5F),xhdpi("values-xhdpi",2F),xxhdpi("values-xxhdpi",3F);
        ```
        >[如果想支持多种像素文件夹那种 看这个](https://github.com/luhaoaimama1/JavaZone/blob/master/JavaTest_Zone/src/%E9%80%82%E9%85%8D/MakeXml_AccurateSize.java)
    * [如果有人对json解析实体类感兴趣,请看这个项目](https://github.com/luhaoaimama1/JsonParser)

        >因为当时公司用的都是string,所以就没有匹配其他类型~ 老项目(GBK编码 GUI项目) 命名什么的不要吐槽了~ 写的很坑不过理解的话应该还可以

* 项目介绍篇(按顺序 从好到一般)
    * [zone-sdk](https://github.com/luhaoaimama1/zone-sdk)
    
        >所有基础工具类 收集与封装 与demo测试;
    * [ZAdapter](https://github.com/luhaoaimama1/ZAdapter)
    
        >demo:包含一些list 与recycler 所遇到的难题的解决方案

        >功能:listView与RecyclerView 的adapter仅仅改下类名即可公用;并且可以省去强转的麻烦;
    * [ZAnimate](https://github.com/luhaoaimama1/ZAnimate)
    
        >[2d库](https://github.com/luhaoaimama1/ZAnimate):就是把androidnineold 变成连用的方式 ,并且减少了不必要的参数,与预设动画的支持;

        >[3d库](https://github.com/luhaoaimama1/ZAnimate/blob/master/README-3D.md):理解方式遵循ae的图层
    * [Shine](https://github.com/luhaoaimama1/Shine)

        >与github上的shimmer类似; 多了个 bitmap加shine与倾斜角度 等等
    * [Zbanner](https://github.com/luhaoaimama1/Zbanner)

        >功能:可无限循环,亦可不无限循环,定时。兼容。包含指示器(简单的);
    * [APT 与动态代理](https://github.com/luhaoaimama1/AnnotationStudy/blob/master/README.md)

        >APT:butterKinfe 的那种靠编译时注解,生成文件,以供调用;

        >动态代理:在demo里可以看到 易于理解;主要明白 生成的代理类可以实现接口;
    * [Gesture类的学习与扩展](https://github.com/luhaoaimama1/GestureStudy)

        >功能:位移,缩放,旋转 都可以得到的手势支持 (zone-sdk中已经包含了)
    * [5.0事物动画的学习](https://github.com/luhaoaimama1/TransitionStudy)

        >功能:Transition类的研究,与5.0事物动画(list嵌套等)的实现与注意;
    * [okhttp](https://github.com/luhaoaimama1/ZOkHttp)

        >功能:网络请求库;支持 `get` `post` `post file` `cookie` `https`等功能;
    * [ZView](https://github.com/luhaoaimama1/ZView)

        >目的:为了搜集 常用的 小型的 稳定的 自定义View Ps:虽然暂时还很小~ 但是架不住收集的时间长啊
    * [Http_Rflist_Helper](https://github.com/luhaoaimama1/Http_Rflist_Helper/blob/master/README-cn.md)

        >一个可以把网络请求 和pullview关联，从而不需要处理 翻页 上拉下拉的动画处理 与 数据更新问题 并且可以全局切换网络请求库

* 插件篇
    * [快速生成六种单例](https://github.com/luhaoaimama1/SingletonTest)

        >功能:快速生成六种单例模式

        >痛点:单例模式无法继承,导致每次都需要写 很费劲。并且是固定写法;

    * [空格检测](https://github.com/luhaoaimama1/SpaceTest2)

         >功能:检查字符串是否有空格
 
         >痛点:当一个类url常量过多,不小心开头弄出空格,还好使,但是cache缓存方面却失常的问题...

******
[▲ 回到顶部](#top)