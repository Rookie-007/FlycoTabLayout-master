依赖配置

repositories {
    maven { url 'https://jitpack.io' }
}

dependencies {
    implementation 'com.github.Rookie-007:FlycoTabLayout-master:3.6.0'
}


新增功能

在原有 FlycoTabLayout-master 基础上，支持单独配置选中/未选中 tab 的字体大小和颜色：

tl:tl_selectSize="20dp" → 选中 tab 字体大小

tl:tl_unselectSize="10dp" → 未选中 tab 字体大小

示例使用

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


我可以帮你把整个 README 风格化成类似官方库的文档格式，让使用方法、属性说明、示例代码分段清楚，方便直接发布。

你希望我帮你做吗？

你说：
做
ChatGPT 说：

好的，我帮你把 README/文档整理成清晰、易读、发布级别的格式，包含依赖、功能说明、属性说明、示例代码。下面是一个完整示例：

FlycoTabLayout-master

在原有 FlycoTabLayout-master 的基础上，新增了 选中/未选中 Tab 字体大小和颜色单独配置 功能。

📦 依赖

在项目 build.gradle 中添加 JitPack 仓库和依赖：

repositories {
    maven { url 'https://jitpack.io' }
}

dependencies {
    implementation 'com.github.Rookie-007:FlycoTabLayout-master:3.6.0'
}

✨ 新增功能

支持自定义 选中/未选中 Tab 字体大小和颜色：

属性	类型	说明
tl:tl_selectSize	dimension	选中 Tab 字体大小，例如 20dp
tl:tl_unselectSize	dimension	未选中 Tab 字体大小，例如 10dp
tl:tl_selectColor	color	选中 Tab 字体颜色
tl:tl_unselectColor	color	未选中 Tab 字体颜色

注意：其他原有属性依然支持，例如下划线、加粗等。

🛠 使用示例
<com.flyco.tablayout.SlidingTabLayout
    android:id="@+id/tl_1"
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:background="#666666"
    android:paddingBottom="15dp"
    android:paddingTop="15dp"
    
    tl:tl_selectSize="20dp"
    tl:tl_unselectSize="10dp"
    tl:tl_selectColor="#FF0000"
    tl:tl_unselectColor="#CCCCCC"
    
    tl:tl_indicator_gravity="TOP"
    tl:tl_textBold="SELECT"
    tl:tl_underline_color="#1A000000"
    tl:tl_underline_gravity="TOP"
    tl:tl_underline_height="1dp"/>

📖 属性说明（常用）

tl:tl_selectSize → 选中字体大小

tl:tl_unselectSize → 未选中字体大小

tl:tl_selectColor → 选中字体颜色

tl:tl_unselectColor → 未选中字体颜色

tl:tl_textBold → 文字加粗方式（SELECT, ALL 等）

tl:tl_indicator_gravity → 指示器位置（TOP, BOTTOM）

tl:tl_underline_color → 下划线颜色

tl:tl_underline_height → 下划线高度