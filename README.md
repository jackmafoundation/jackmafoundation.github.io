# shandian

闪电孵化器新官网 DEMO - Powered by Jekyll 

## 维护方式

这里已问题方式说明，可以先看下「目录结构」帮助理解。

* [Markdown 语法](https://github.com/tinyao/shandian/wiki/%E5%88%9B%E5%BB%BA%E6%88%96%E4%BF%AE%E6%94%B9%E6%96%87%E7%AB%A0)
* [创建或修改文章](https://github.com/tinyao/shandian/wiki/%E5%88%9B%E5%BB%BA%E6%88%96%E4%BF%AE%E6%94%B9%E6%96%87%E7%AB%A0)
* [创建或修改项目](https://github.com/tinyao/shandian/wiki/%E5%88%9B%E5%BB%BA%E6%88%96%E4%BF%AE%E6%94%B9%E9%A1%B9%E7%9B%AE)
* [如何上传图片，并在文章和项目中使用](https://github.com/tinyao/shandian/wiki/%E5%A6%82%E4%BD%95%E4%B8%8A%E4%BC%A0%E5%9B%BE%E7%89%87%EF%BC%8C%E5%B9%B6%E5%9C%A8%E6%96%87%E7%AB%A0%E5%92%8C%E9%A1%B9%E7%9B%AE%E4%B8%AD%E4%BD%BF%E7%94%A8)
* [创建或修改专题页面](https://github.com/tinyao/shandian/wiki/创建或修改专题页面)


## 目录结构

```
_includes: 
_layouts:
_posts: 放文章文件
_sass:
_startup: 放 startup 项目文件
about: About 相关页面文件
  - cooperators.md: 合作伙伴
  - members.md: 团队成员
  - joinus.md: 加入我们
  - nibachuangke.md: 泥巴创客
  - service-organization.md: 服务机构
assets
blog
service
  - activity.md: 活动
  - apply.md: 申请孵化
  - course.md: 创业课程
  - rules.md: 入驻规则

  - activity: 活动子项目
    - startup-training-2014.md
  - course: 课程子项目
    - programming-practice-2014.md
    - programming-practice-2014.md
    - learning-materials.md
sync
_config.yml
about.md: 关于页面
blog.md: 博客页面
index.html: 首页
service.md: 服务页面
startup-archived.md: 归档项目
startup.md: 孵化项目
```