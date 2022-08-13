# 项目 (Project)

要创建一个项目，只需要调用`Project` DSL。

```kotlin
fun main() {
    Project("Project Name") { }
}
```

在 Project DSL 中可设置窗口属性、流程，添加场景等。

```kotlin
fun main() {
    Project("Project Name") {
        // 设置窗口
        window {
            title = "标题"
        }
        // 设置窗口属性（一对一）
        hints(
            // 设置窗口在 postStart() 前不可见
            GLFW_VISIBLE to GLFW_FALSE
        )
        // 添加场景
        "scene_id" { }
    }
}
```

更多详细内容会在后面的章节讲解。
