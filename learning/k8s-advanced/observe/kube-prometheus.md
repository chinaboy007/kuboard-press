---
# vssueId: 143
layout: LearningLayout
description: Kubernetes教程_本文介绍了 kube-prometheus 项目，用于监控 Kubernetes 集群。
meta:
  - name: keywords
    content: Kubernetes教程, Kubernetes监控
---

# kube-prometheus

本文向大家推荐一个基于 prometheus 的监控项目 [chinaboy007/kube-prometheus](https://github.com/chinaboy007/kube-prometheus)


## 概述

**很多地方提到Prometheus Operator是kubernetes集群监控的终极解决方案，但是目前Prometheus Operator已经不包含完整功能，完整的解决方案已经变为kube-prometheus。项目地址为：https://github.com/coreos/kube-prometheus
本项目基于最新kube-prometheus开发,解决了kube-prometheus安装部署后无法监控kube-controller kube-scheduse kube-etcd，无法告警、无法数据持久化等各种问题，为小白用户提供了极大便利。**




## 主要功能

- 1.支持数据持久化

- 2.支持kube-controller监控

- 3.支持kube-scheduse监控

- 4.支持kube-etcd监控

- 5.支持NodePort访问

- 6.支持ingress访问

- 7.支持离线安装

- 8.支持重复安装

- 9.支持一键卸载


## 部署在 Kubernetes
#### 前置要求
   
 - 支持kubeadm方式安装的k8s,二进制方式安装的未测试
 - 支持prometheus 2.15.2版本

#### 一键安装

```bash 
git clone https://github.com/chinaboy007/kube-prometheus.git
cd kube-prometheus/manifests
sh install.sh
```


#### 一键卸载

```bash
cd kube-prometheus/manifests
sh uninstall.sh
```
