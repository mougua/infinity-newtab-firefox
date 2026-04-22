# InfinityTab New Tab

一个简单的 Firefox 浏览器扩展，自定义新标签页为 inftab.com 网站。

## 功能

- 将 Firefox 新标签页重定向到 [inftab.com](https://inftab.com/)
- 以全屏 iframe 方式加载目标页面
- 支持沙盒隔离，安全运行

## 安装

### 从源码安装

1. 克隆或下载本项目
2. 打开 Firefox，访问 `about:debugging#/runtime/this-firefox`
3. 点击"临时加载附加组件..."
4. 选择项目中的 `manifest.json` 文件

### 使用预构建版本

在 `web-ext-artifacts/` 目录下有已构建的扩展文件：

- `infinitytab_new_tab-1.0.0.xpi` - 适用于 Firefox 58+
- `infinitytab_new_tab-1.0.0.zip` - 打包文件

## 项目结构

```
firefox-tab/
├── manifest.json      # 扩展配置文件
├── newtab.html        # 新标签页内容
└── web-ext-artifacts/ # 构建输出目录
```

## 技术细节

- **Manifest Version**: 2
- **最低 Firefox 版本**: 58.0
- **扩展 ID**: infinitytab-newtab@mylab

## 开发

使用 [web-ext](https://extensionworkshop.com/documentation/develop/getting-started-with-web-ext/) 工具进行开发：

```bash
# 安装 web-ext
npm install -g web-ext

# 启动开发模式（自动重载）
web-ext run

# 构建发布版本
web-ext build
```
