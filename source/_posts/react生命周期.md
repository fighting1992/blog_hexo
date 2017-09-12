---
title: react生命周期
date: 2017-07-18 15:39:50
tags: react
categories: web
---

## componentWillMount
- 组件首次渲染完成之前执行，只执行一次


## componentDidMount
- 真实的dom被渲染出来后调用，此时可通过refs访问到真实dom，注册事件等

## componentWillReceiveProps
- 组件接收到新的props时调用，并将其作为参数nextProps使用，此时可以更改组件props及state。

## componentWillUpdate
- 接收到新的props或者state后，进行渲染之前调用，此时不允许更新props或state。


## componentDidUpdate
- 完成渲染新的props或者state后调用，此时可以访问到新的DOM元素。

## shouldComponentUpdate
- 组件是否应当渲染新的props或state，返回false表示跳过后续的生命周期方法

## componentWillUnmount
- 组件卸载之前调用，多用于注销事件、清除定时器等
