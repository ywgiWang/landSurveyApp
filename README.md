# 轻量的土地调查管理系统
 A Lightweight Land Survey Application

## 软件使用场景
Software Usage Scenarios

- **野外土地调查**：支持调查人员在野外环境中实时查看地块分布、采集属性数据并上传现场照片
  **Field Land Survey**: Supports surveyors in real-time viewing of plot distribution, collecting attribute data, and uploading on-site photos in field environments
- **多团队协作作业**：允许多个调查小组同时操作，实时同步数据，避免重复调查
  **Multi-team Collaborative Operation**: Allows multiple survey teams to operate simultaneously, synchronizing data in real-time to avoid duplicate surveys
- **紧急事件快速响应**：在自然灾害或土地纠纷等紧急情况下，快速定位并记录现场情况
  **Emergency Rapid Response**: Quickly locates and records on-site conditions during emergencies such as natural disasters or land disputes
- **数据审核与归档**：提供标准化的数据导出功能，满足国土部门的归档和上报要求
  **Data Review and Archiving**: Provides standardized data export functions to meet the archiving and reporting requirements of land management departments
- **移动办公支持**：轻量化H5架构适配各类移动设备，无需安装专用客户端即可使用
  **Mobile Office Support**: Lightweight H5 architecture adapts to various mobile devices, enabling usage without installing dedicated clients

## 技术架构
 Technical Architecture
- **开发模式**：基于H5的轻量化Web应用
- **前端框架**：Vue.js
- **地图引擎**：Mapbox GL

## 软件功能介绍

### 1. 图斑状态可视化
 1. Plot Status Visualization
- 在地图上直观展示所有土地调查区块
- 颜色编码区分调查状态：
  - 🔴 红色：未调查区块
  - 🟡 黄色：暂存调查记录
  - 🟢 绿色：已完成调查区块

<div align="center">
<img src="./samples/Screenshot 2025-07-17 103821.png" height="300" />
</div>

### 2. 实时定位与导航
 2. Real-time Positioning and Navigation
- 集成GPS定位功能，实时显示用户当前位置
- 提供目标图斑导航功能，支持路径规划与指引

<div align="center">
<img src="./samples/Screenshot 2025-07-17 104656.png" height="300" />
<img src="./samples/Screenshot 2025-07-17 105524.png" height="300" />

</div>

### 3. 图斑属性管理
 3. Plot Attribute Management
- 完整的图斑属性表单填写界面
- 支持现场照片拍摄与上传，自动关联图斑信息
- 照片EXIF信息提取，包含位置数据

<div align="center">
<img src="./samples/Screenshot 2025-07-17 105051.png" height="300" />
<img src="./samples/Screenshot 2025-07-17 105106.png" height="300" />
<img src="./samples/Screenshot 2025-07-17 105128.png" height="300" />
</div>


### 4. 调查成果导出
 4. Survey Result Export
- 支持导出标准Shapefile格式空间数据
- 自动打包关联照片文件夹，保持文件组织结构
- 导出数据符合行业标准，可直接用于后续分析

### 5. 多人协作支持
 5. Multi-user Collaboration Support
- 多用户同时登录系统进行操作
- 数据实时同步，避免冲突
- 支持团队协作完成大规模调查任务
