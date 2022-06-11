---
title: 容器镜像
status: Feedback Appreciated
category: 概念
---

## 是什么

容器镜像是一个不可改变的静态文件，包含创建容器的依赖性。
这些依赖可能包括一个可执行的二进制文件、系统库、系统工具、环境变量和其他必要的平台设置。
容器镜像是应用程序容器化的结果，通常存储在容器注册表中，在那里可以下载并使用容器运行时接口（CRI）作为一个孤立的进程运行。
容器镜像框架必须遵循开放容器倡议（OCI）定义的标准模式。

## 解决的问题

传统上，应用服务器是按环境配置的，而应用则被部署到这些环境中。
环境之间的任何错误配置都是有问题的，常常导致停机或部署失败。
一个应用程序的环境需要是可重复的和定义明确的；否则，与环境有关的错误的机会就会增加。
当应用程序的环境定义不足或不准确时，应用程序的横向和纵向伸缩就会成为挑战。

## 如何帮助

容器镜像将一个应用程序与它的任何运行时的依赖性捆绑在一起，例如一个应用程序服务器。
这提供了所有环境的一致性，包括开发人员的机器。
容器镜像可用于实例化所需的多个容器，允许更大的可伸缩性。
