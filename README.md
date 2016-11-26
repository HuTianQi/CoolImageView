# CoolImageView
A imageView  is similar to QQ that imageView background picture can move up and down，But the function is more powerful than QQ,it also supports left and right movement  

[![license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/HuTianQi/CoolImageView#license)
[![platform](https://img.shields.io/badge/platform-Android-yellow.svg)](https://www.android.com)

##Dynamic effect preview （Because the gif resources are large, please wait for the resources to complete the load）
this is  background picture left and right movement  
![image](https://github.com/HuTianQi/CoolImageView/blob/master/beauty.gif)    
 this is background picture move up and down  
![image](https://github.com/HuTianQi/CoolImageView/blob/master/beauty_.gif)   


##How to use
step1: Add the following to your attrs.xml file (in res/values):
-----
```xml
<resources>
    <declare-styleable name="CoolImageView">
        <attr name="direction" format="string"/>
    </declare-styleable>
</resources>
```

step2:Add the following code to the root view of your layout:  
-----
```xml
xmlns:app="http://schemas.android.com/apk/res-auto"
```

step3:Add the widget code in the appropriate place in your xml file, Here's a sample implementation:  
-----
```xml
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:id="@+id/activity_main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical"
    tools:context="com.example.hzhuqi.coolimagview.MainActivity">
    
    <com.example.hzhuqi.coolimagview.CoolImageView
        android:layout_width="wrap_content"
        android:layout_height="300dp"
        android:src="@mipmap/qq"
        app:direction="horizontal"

       >
    </com.example.hzhuqi.coolimagview.CoolImageView>

    <com.example.hzhuqi.coolimagview.CoolImageView
        android:layout_marginTop="@dimen/activity_vertical_margin"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:src="@mipmap/qq_"
        app:direction="vertical"
        >
    </com.example.hzhuqi.coolimagview.CoolImageView>
</LinearLayout>

```

##Notice:
you should set direction properties in your xml file,If you don't want to do that.You can use ordinary ImageView instead

##License
MIT License

Copyright (c) 2016 hq_sunshine

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
