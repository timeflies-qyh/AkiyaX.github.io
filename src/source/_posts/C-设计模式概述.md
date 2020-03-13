---
title: 'C#设计模式概述'
date: 2020-03-14 02:20:58
category: 设计模式
tags: .NET
id: csharp-design-pattern
---

# 前言

工作一段时间后才发现设计模式的重要性，实现同样功能的代码，人家的代码看着如此舒适，却又说不出好在哪里😟，我想就应该是差在内功了。大三准备面试时也粗略学过一段时间设计模式，但因为缺乏工程经验，没有深切体会，现在重新捡起温习。

本系列博客主要参考刘伟博士著作的《C#设计模式》一书👍，结合本人的实践与思考而写成，同时参阅网络上各位大佬的总结，不再列出。

🍺源码汇总：https://github.com/AkiyaX/CSharpDesignPattern

![《C#设计模式》 - 封面](https://img-blog.csdn.net/20180318164255870)

# 概览

最早将模式思想引入软件工程方法学的是Gang of Four（GOF）自称的四位软件工程学者，分别是Erich Gamma、Richard Helm、Ralph Johnson和John Vlissides，他们在1994年归纳发表了23种在软件开发领域较为常用的设计模式。GOF对设计模式的定义：

>**设计模式**是在特定环境下为解决某一通用软件设计问题提供的一套定制解决方案，该方案描述了类和对象之间的相互作用。
>**Design patterns** are desriptions of communicating objects and classes that are custormized to solve a general design problem in a particular context.

## 创建型模式

[**抽象工厂模式**](#)（Abstract Fatory Pattern）：提供一个创建一系列相关或互相依赖对象的接口，而无须指定它们具体的类。

[**建造者模式**]()（Builder Pattern）：将一个复杂对象的构建与它的表示分离，使得同样的构造过程可以创建不同的表示。

**工厂方法模式**（Factory Method Pattern）：定义一个用于创建对象的接口，但是让子类决定将哪一个类实例化。工厂方法模式让一个类的实例化延迟到子类。

**原型模式**（Prototype Pattern）：使用原型实例指定待创建对象的类型，并且通过复制这个原型来创建新的对象。

**单例模式**（Singleton Pattern）：确保一个类只有一个实例，并提供一个全局访问点来访问这个唯一实例。

## 结构型模式

**适配器模式**（Adapter Pattern）：将一个类的接口转换成客户希望看到的另一个接口，适配器模式让那些接口不兼容的类可以一起工作。

**桥接模式**（Bridge Pattern）：将抽象部分与它的实现部分解耦，使得两者都能够独立变化。

**组合模式**（Composite Pattern）：组合多个对象形成树形结构以表示具有部分——整体关系的层次结构，组合模式让客户端可以统一对待单个对象和组合对象。

**装饰模式**（Decorator Pattern）：动态地给一个对象增加一个
