# 场景 (Scene)

场景是 Ktgl 中必不可少的内容。没有场景将不能渲染或添加游戏对象。  
在[项目](project.md)一章中，我们创建了一个 ID 为`scene_id`的场景。我们将围绕这个 DSL 逐步添加游戏对象。

TODO

## 渲染

游戏对象设置完成后，我们发现场景还是没有渲染出来。这是因为我们没有设置场景。  
场景会在`preRunning()`后执行，因此，我们在 Project DSL 中调用`preRunning` DSL，并设置当前场景。

```kotlin
preRunning {
    currScene = "scene_id"
}
```

现在就能看到一个彩色的立方体了。
