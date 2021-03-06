# my-vue-admin

一个简单的 vue 管理后台模版。基于 [vue-admin-template](https://github.com/PanJiaChen/vue-admin-template) 开源项目搭建，参考了 [RuoYi-Vue](https://gitee.com/y_project/RuoYi-Vue) 的用户管理、角色管理、日志管理等模块，并做了一些简化和修改：
1. 用户管理去掉部门、性别和岗位。所以不需要 RuoYi-Vue 的部门管理和岗位管理。
2. 角色管理菜单权限仅支持到菜单级别，不支持按钮级别。所以不需要 RuoYi-Vue 的菜单管理，菜单目录直接前端根据路由自动生成，减轻了后端配置菜单的麻烦。

![image](https://github.com/willxiao90/my-vue-admin/blob/master/doc/snapshot1.png)

## Build Setup

```bash
# 克隆项目
git clone https://github.com/willxiao90/my-vue-admin.git

# 进入项目目录
cd my-vue-admin

# 安装依赖
npm install

# 建议不要直接使用 cnpm 安装以来，会有各种诡异的 bug。可以通过如下操作解决 npm 下载速度慢的问题
npm install --registry=https://registry.npm.taobao.org

# 启动服务
npm run dev
```

浏览器访问 [http://localhost:9528](http://localhost:9528)

## 发布

```bash
# 构建测试环境
npm run build:stage

# 构建生产环境
npm run build
```

## 其它

```bash
# 预览发布环境效果
npm run preview

# 预览发布环境效果 + 静态资源分析
npm run preview -- --report

# node 服务构建
npm run server-build

# node 服务启动
npm run server

# 代码格式检查
npm run lint

# 代码格式检查并自动修复
npm run lint -- --fix
```

更多信息请参考： 
- [vue-admin-template 文档](https://panjiachen.github.io/vue-element-admin-site/zh/)
- [RuoYi 文档](http://doc.ruoyi.vip/)
