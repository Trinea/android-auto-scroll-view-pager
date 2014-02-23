Android Auto Scroll ViewPager
==============================

auto scroll ViewPager or ViewPager in ViewPager

## Demo apk
<a href="https://play.google.com/store/apps/details?id=cn.trinea.android.demo" target="_blank" title="Download From Google Play"><img src="http://www.android.com/images/brand/get_it_on_play_logo_small.png" title="Download From Google Play"/></a>  

## Usage
include this library, use

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
startAutoScroll() start auto scroll  
startAutoScroll(int)} start auto scroll delayed  
stopAutoScroll()} stop auto scroll  

### Setting
setInterval(long) set auto scroll time in milliseconds, default is 1500ms  
setDirection(int)} set auto scroll direction, default is Right  
 setCycle(boolean) set whether automatic cycle when auto scroll reaching the last or first item, default is true  
 setSlideBorderMode(int) set how to process when sliding at the last or first item  
 setStopScrollWhenTouch(boolean) set whether stop auto scroll when touching, default is true  
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

[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/Trinea/android-auto-scroll-view-pager/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

[![githalytics.com alpha](https://cruel-carlota.pagodabox.com/980e58e9fe20890c1f61564a29311cdf "githalytics.com")](http://githalytics.com/Trinea/android-auto-scroll-view-pager)

