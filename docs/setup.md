# 配置环境

在配置环境之前，您需要先知道显卡支持的 OpenGL 版本。Ktgl 要求至少支持 OpenGL 3.2。

如果显卡不支持 OpenGL 3.2 版本，则需要更新显卡驱动或更换显卡。

## 使用 Gradle

使用 Gradle 可轻松配置 Ktgl 环境。只需在项目的`build.gradle`中添加依赖库即可。

```groovy
dependencies {
    // 加号应替换为指定版本
    implementation 'io.github.over-run:ktgl:+'
}
```

配置完成后即可开始创建**项目** (Project)。
