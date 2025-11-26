# FlycoTabLayout 扩展说明

本库基于 [FlycoTabLayout](https://github.com/Rookie-007/FlycoTabLayout) 进行扩展，新增了选中和未选中字体大小属性，方便自定义 Tab 显示效果。

---

## AndroidX 依赖

```groovy
dependencies {
    implementation 'com.github.Rookie-007:FlycoTabLayout-master:3.6.0'
}
```

---

## 新增属性说明

| 属性名            | 类型 | 说明                       |
|------------------|------|----------------------------|
| `tl_selectSize`    | dp/sp | 选中 Tab 的字体大小       |
| `tl_unselectSize`  | dp/sp | 未选中 Tab 的字体大小     |

---

## 使用示例

```xml
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
```

---

## 使用说明

1. 将库添加到项目依赖中（如上所示）。  
2. 在 XML 中使用 `SlidingTabLayout`，通过 `tl_selectSize` 和 `tl_unselectSize` 设置选中和未选中的字体大小。  
3. 其他属性可继续使用原 FlycoTabLayout 的配置，如 `tl_indicator_gravity`、`tl_textBold`、`tl_underline_color` 等。

---

## 注意事项

- 字体大小单位建议使用 `sp`，可更好适配不同屏幕。  
- 确保在布局文件中正确引入 `tl` 命名空间，例如：

```xml
xmlns:tl="http://schemas.android.com/apk/res-auto"
```