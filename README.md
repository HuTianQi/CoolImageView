# CoolImageView
A imageView  is similar to QQ that ImageView background picture can move up and down，But the function is more powerful than QQ  

##动态效果：


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
