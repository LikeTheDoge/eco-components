---
title: EUploadBtn
subtitle: 基础上传按钮
---

点击选择文件区域上传

## 主要功能

- 包含指定区域上传模式，区域内部自定义，

- 作为独立区域上传时，内部有直接上传按钮

- 上传需要显示 loading 效果

- todo: 上传完成成功提示，以及成功后回调函数
  
## Demo

[demo](Demo)

## API

- < slot > default

`() => VNode`

内部默认显示的内容

- < slot > hover-tip

`() => VNode`

用户拖拽文件悬浮时的提示信息

- < slot > loading-mask
  
`() => VNode`

用户上传文件的时候的 loading 占位

- < prop > upload
 
`(file:File) => Promise<void> ` 

上传事件回调，接受参数 `file` 为用户上传的文件 (浏览器原生 File 类型)

直接在上传回调中做文件相关的验证

todo:返回结果为 `true` 提示成功上传

- <del>< prop > validate </del> 