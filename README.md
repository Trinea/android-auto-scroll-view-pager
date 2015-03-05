Android Auto Scroll ViewPager
==============================
ViewPager which can auto scrolling, cycling, decelerating.  
ViewPager which can be slided normal in parent ViewPager.  

中文介绍见: [Android自动滚动 轮播循环的ViewPager](http://www.trinea.cn/android/auto-scroll-view-pager/)
![android-auto-scroll-view-pager](http://farm3.staticflickr.com/2843/12805132475_e595664a81_o.gif)

## Sample Application
<a href="https://play.google.com/store/apps/details?id=cn.trinea.android.demo" target="_blank" title="Download From Google Play"><img src="http://www.android.com/images/brand/get_it_on_play_logo_small.png" title="Download From Google Play"/></a>
    <a href="http://trinea.github.com/apk/trinea-android-demo.apk" target="_blank" title="Scan to download"><img src="https://farm3.staticflickr.com/2930/14017948972_bafb6df1b5_o.png" title="Scan to download"/></a>
    <a href="http://trinea.github.com/apk/trinea-android-demo.apk" target="_blank" title="Click to download">Download</a>  

Demo File: [AutoScrollViewPagerSingleDemo.java](https://github.com/Trinea/android-demo/blob/master/src/cn/trinea/android/demo/AutoScrollViewPagerDemo.java)  
Demo Project: [android-demo](https://github.com/Trinea/android-demo)  

## Usage
- include this library, use

``` xml
<cn.trinea.android.view.autoscrollviewpager.AutoScrollViewPager
	android:id="@+id/view_pager"
	android:layout_width="match_parent"
	android:layout_height="wrap_content" />
```
replace
``` xml
<android.support.v4.view.ViewPager
	android:id="@+id/view_pager"
	android:layout_width="match_parent"
	android:layout_height="wrap_content" />
```
- `startAutoScroll()` start auto scroll, delay time is `getInterval()`.
- `startAutoScroll(int)` start auto scroll delayed.
- `stopAutoScroll()` stop auto scroll.

## Setting
- `setInterval(long)` set auto scroll time in milliseconds, default is `DEFAULT_INTERVAL`.  
- `setDirection(int)` set auto scroll direction, default is `RIGHT`.  
- `setCycle(boolean)` set whether automatic cycle when auto scroll reaching the last or first item, default is true. 
- `setScrollDurationFactor(double)` set the factor by which the duration of sliding animation will change.  
- `setSlideBorderMode(int)` set how to process when sliding at the last or first item, default is `SLIDE_BORDER_MODE_NONE`.
- `setStopScrollWhenTouch(boolean)` set whether stop auto scroll when touching, default is true.  
- `setBorderAnimation(boolean)` set whether animating when auto scroll at the last or first item, default is true.  
- You cannot combine with [ViewPagerIndicator](https://github.com/JakeWharton/Android-ViewPagerIndicator) if `setCycle(true)`. 
- If you want infinite loop, please see [AutoScrollViewPagerSingleDemo.java](https://github.com/Trinea/android-demo/blob/master/src/cn/trinea/android/demo/AutoScrollViewPagerDemo.java)  
**More:** http://www.trinea.cn/android/auto-scroll-view-pager/

## Proguard
``` xml
-keep class cn.trinea.android.** { *; }
-keepclassmembers class cn.trinea.android.** { *; }
-dontwarn cn.trinea.android.**
```

## Download
Maven:  
``` xml
<dependency>
    <groupId>cn.trinea.android.view.autoscrollviewpager</groupId>
    <artifactId>android-auto-scroll-view-pager</artifactId>
    <version>1.1.2</version>
</dependency>
```  

Gradle:  
``` xml
compile 'cn.trinea.android.view.autoscrollviewpager:android-auto-scroll-view-pager:1.1.2'
```  

## Contact Me
- [trinea@google plus](https://plus.google.com/u/0/111989205221366883984)
- [trinea@twitter](https://twitter.com/trinea_cn)
- [trinea@weibo](http://weibo.com/trinea)
- [trinea.cn](http://www.trinea.cn/)
- [trinea.cn#gmail.com](mailto:trinea.cn@gmail.com)

## License

    Copyright 2014 trinea.cn

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

