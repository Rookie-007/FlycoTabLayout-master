// AndroidX
dependencies {
    implementation 'com.github.Rookie-007:FlycoTabLayout-master:3.6.0'
}
新增属性说明
tl_selectSize：选中 tab 的字体大小

tl_unselectSize：未选中 tab 的字体大小

使用示例
xml
复制代码
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