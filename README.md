# SwitchButton
SwitchButto  *beautiful+lightweight+custom-style-easy*switch widget for android</br>
SwitchButton 是 Android 上的一个开关按钮控件<br>



UseAge
-------
gradle:
```grovvy
repositories {

     maven { url 'https://jitpack.io' }
}

...

dependencies {
   implementation 'com.github.zhangi789:SwitchButton:2.0'
}
```

layout.xml:
```xml
  <cn.util.smart.com.SwitchButton
        android:layout_gravity="center"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="20dp"
        app:sb_button_color="#db99c7"
        app:sb_shadow_color="#A36F95"
        app:sb_background="#FFF"
        app:sb_checkline_color="#a5dc88"
        app:sb_checked_color="#A36F95"
        app:sb_width="64dp"
        app:sb_height="30dp"
        app:sb_uncheckcircle_color="#A36F95"
        />
```

Activity.java:
```java
SwitchButton switchButton = (SwitchButton)
    findViewById(R.id.switch_button);

switchButton.setChecked(true);
switchButton.isChecked();
switchButton.toggle();     //switch state
switchButton.toggle(false);//switch without animation
switchButton.setShadowEffect(true);//disable shadow effect
switchButton.setEnabled(false);//disable button
switchButton.setEnableEffect(false);//disable the switch animation
switchButton.setOnCheckedChangeListener(new SwitchButton.OnCheckedChangeListener() {
    @Override
    public void onCheckedChanged(SwitchButton view, boolean isChecked) {
        //TODO do your job
    }
});


```

More Style:
```xml
<attr name="sb_shadow_radius" format="reference|dimension"/>       阴影半径
<attr name="sb_shadow_offset" format="reference|dimension"/>       阴影偏移
<attr name="sb_shadow_color" format="reference|color"/>            阴影颜色
<attr name="sb_uncheck_color" format="reference|color"/>           关闭颜色
<attr name="sb_checked_color" format="reference|color"/>           开启颜色
<attr name="sb_border_width" format="reference|dimension"/>        边框宽度
<attr name="sb_checkline_color" format="reference|color"/>         开启指示器颜色
<attr name="sb_checkline_width" format="reference|dimension"/>     开启指示器线宽
<attr name="sb_uncheckcircle_color" format="reference|color"/>     关闭指示器颜色
<attr name="sb_uncheckcircle_width" format="reference|dimension"/> 关闭指示器线宽
<attr name="sb_uncheckcircle_radius" format="reference|dimension"/>关闭指示器半径
<attr name="sb_checked" format="reference|boolean"/>               是否选中
<attr name="sb_shadow_effect" format="reference|boolean"/>         是否启用阴影
<attr name="sb_effect_duration" format="reference|integer"/>       动画时间，默认300ms
<attr name="sb_button_color" format="reference|color"/>            按钮颜色
<attr name="sb_show_indicator" format="reference|boolean"/>        是否显示指示器，默认true：显示
<attr name="sb_background" format="reference|color"/>              背景色，默认白色
<attr name="sb_enable_effect" format="reference|boolean"/>    是否启用特效，默认true   
<attr name="sb_width" format="reference|dimension"/>      宽         
<attr name="sb_height" format="reference|dimension"/>    高     
```


License
-------
MIT, See the <a href="https://github.com/zhangi789/SwitchButton.git">[LICENSE]</a> file for details.
