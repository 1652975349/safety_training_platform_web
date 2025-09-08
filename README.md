# 低代码安全培训平台后台管理系统

## 项目结构

```
safety_training_platform/
├── README.md                 # 项目说明文档
├── database.sql             # 数据库表结构
├── index.html               # 主页面（角色选择）
├── common/
│   ├── header.html          # 顶部通栏组件
│   ├── sidebar.html         # 左侧菜单组件
│   └── styles.css           # 公共样式文件
├── student/                 # 学员端页面
│   ├── dashboard.html       # 学员首页
│   ├── my-training.html     # 我的培训
│   ├── learning-resources.html # 学习资源
│   ├── exams.html           # 考试中心
│   ├── profile.html         # 个人中心
│   ├── points.html          # 积分中心
│   └── notifications.html   # 通知中心
├── admin/                   # 管理员端页面
│   ├── dashboard.html       # 管理员首页
│   ├── personnel.html       # 人员管理
│   ├── training.html        # 培训管理
│   ├── content.html         # 内容管理
│   ├── statistics.html      # 统计分析
│   ├── settings.html        # 系统设置
│   └── notifications.html   # 通知管理
└── assets/                  # 静态资源
    ├── images/              # 图片资源
    └── icons/               # 图标资源
```

## 功能模块说明

### 学员端功能
1. **我的培训** - 查看管理员下发的课程、练习、考试
2. **学习资源** - 视频/文档学习，学时和积分同步
3. **考试中心** - 模拟考试和正式考试
4. **个人中心** - 个人信息、证书、学时、积分、排行
5. **积分中心** - 积分明细和排行榜
6. **通知中心** - 培训通知推送

### 管理员端功能
1. **人员管理** - 批量导入导出、扫码注册、分部门分专业
2. **培训管理** - 创建培训、设定学时、组卷、下发、催办
3. **内容管理** - 上传课件、题库管理
4. **统计分析** - 人数、学时、通过率、积分统计
5. **系统设置** - 密码设定、权限设置
6. **通知管理** - 培训通知推送管理

## 技术特点

- 响应式设计，支持PC端和移动端
- 模块化组件设计，便于维护
- 角色切换功能，支持学员/教师/管理员
- 人脸识别防作弊功能集成
- 多端同步支持

## 使用说明

1. 打开 `index.html` 选择角色进入系统
2. 学员端：查看培训内容、参加考试、管理个人信息
3. 管理员端：管理人员、创建培训、统计分析

## 页面功能详情

### 学员端页面
- **dashboard.html** - 学员首页，显示学习概览、统计信息、最近培训等
- **my-training.html** - 我的培训，查看管理员下发的课程、练习、考试
- **learning-resources.html** - 学习资源，视频/文档学习，学时和积分同步
- **exams.html** - 考试中心，模拟考试和正式考试，人脸防作弊
- **profile.html** - 个人中心，个人信息、证书、学时、积分、排行
- **points.html** - 积分中心，积分明细和排行榜
- **notifications.html** - 通知中心，培训通知推送

### 管理员端页面
- **dashboard.html** - 管理员首页，系统概览、快速操作、最近活动
- **personnel.html** - 人员管理，批量导入导出、扫码注册、分部门分专业
- **training.html** - 培训管理，创建培训、设定学时、组卷、下发、催办
- **content.html** - 内容管理，上传课件、题库管理
- **statistics.html** - 统计分析，人数、学时、通过率、积分统计
- **settings.html** - 系统设置，密码设定、权限设置
- **notifications.html** - 通知管理，培训通知推送管理

## 技术特点

- 响应式设计，支持PC端和移动端
- 模块化组件设计，便于维护
- 角色切换功能，支持学员/教师/管理员
- 人脸识别防作弊功能集成
- 多端同步支持
- 纯HTML+CSS+JavaScript实现，无需后端

## 浏览器兼容性

- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

## 部署说明

1. 将所有文件上传到Web服务器
2. 确保服务器支持HTML5和现代JavaScript
3. 配置适当的MIME类型
4. 建议使用HTTPS协议以确保安全性

## 开发说明

- 公共组件位于 `common/` 文件夹
- 样式文件统一在 `common/styles.css`
- 页面通过JavaScript动态加载公共组件
- 支持模块化开发，便于扩展和维护
