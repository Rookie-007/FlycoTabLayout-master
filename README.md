repositories {
    maven { url 'https://jitpack.io' }
}

dependencies {
    implementation 'com.github.Rookie-007:FlycoTabLayout-master:3.6.0'
}

在原有FlycoTabLayout-master基础上，添加选中tab字体大小和颜色单独配置
    tl:tl_selectSize="20dp"    选中文字大小
    tl:tl_unselectSize="10dp"  未选中文字大小
示例如下：
        <com.flyco.tablayout.SlidingTabLayout
                android:id="@+id/tl_1"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:background="#666666"
                android:paddingBottom="15dp"
                android:paddingTop="15dp"
                tl:tl_selectSize="20dp"
                tl:tl_unselectSize="10dp"
                tl:tl_indicator_gravity="TOP"
                tl:tl_textBold="SELECT"
                tl:tl_underline_color="#1A000000"
                tl:tl_underline_gravity="TOP"
                tl:tl_underline_height="1dp"/>