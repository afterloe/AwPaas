# AwPaas
> create by afterloe    

## Overview
AwPaas (afterloe workspace platform as a service) 个人专属开发平台，为支持多地各种产品线编写的统一的服务架构中心。采用jvm语言作为基层，采用spring boot 2.0 + webflux 组成

## Component list
* awpaas-repository     服务仓库      【负责服务注册、分发、调用】
* awpaas-route          路由服务      【对外进行代理，发布、总路口】
* awpaas-monitor        平台监控服务
* awpaas-collect-log    日志采集服务
* awpaas-manager        平台管理服务
* awpaas-oauth2         授权管理服务
