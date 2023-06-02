---
title:  "Spring vault"
date:   2023-06-02 16:15:25 +0700
categories: java spring
tags: java spring
---

# Spring Cloud Vault
## Overview
[Spring Cloud Vault](https://cloud.spring.io/spring-cloud-vault/reference/html/#vault.config.authentication.vault-agent)

[Kubernetes Auth Method](https://www.vaultproject.io/docs/auth/kubernetes)

## Dependencies
pom.xml
```xml
<dependency>  
   <groupId>org.springframework.cloud</groupId>  
   <artifactId>spring-cloud-starter-vault-config</artifactId>  
</dependency>
```

## Bootstrap config
bootstrap.yml
```yml
spring:  
  cloud:  
    vault:  
      enabled: false # on/off load config from vault 
      uri: http://localhost:8200  
      connection-timeout: 5000  
      read-timeout: 15000  
      authentication: token # tren k8s se dung kubernetes 
      token: token  
      generic:  
        enabled: false  
      kv:  
        application-name: tablet-checkin-tablet-service # ten secret tren vault  
        enabled: false  
        backend-version: 2  
        profile-separator: /  
        backend: checkin-dev # ten cua secret engine
```
