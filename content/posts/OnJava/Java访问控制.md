---
title: "On Java读书笔记--访问控制"
date: 2022-06-04T23:57:25+08:00
description: Java访问控制
menu:
  sidebar:
    name: Java访问控制
    identifier: Java访问控制
    weight: 10
hero: fernand-de-canne-Unl-fQ1_P5Q-unsplash.jpg
tags: ["Basic", "Multi-lingual"]
categories: ["Basic"]
---

# On Java读书笔记--访问控制

## 访问修饰符
Java提供了3个显式关键字来完成访问控制，即`public`、`private`以及`protected`。

- `public`，表示定义的内容可以被所有人访问
- `private`，表示定义的内容只能被雷的创建者通过该类自身的方法访问，而其他任何人都无法访问
- `protected`，类似于`private`，区别在于**继承**的子类可以访问`protected`成员，但不可以访问`private`成员

## 包访问
如果不使用上述[访问修饰符](#访问修饰符)，Java会提供一种“默认”访问权限，通常叫作“包访问”。
- `包访问`，一个类可以访问同一个包里的其他类；但是如果从包外部访问这些类的话，它们就像private内容一样不可访问。
  
