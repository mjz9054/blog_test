---
layout: default
title: MutilpartResolver&PropertiesPlaceHolder
---

---

# Spring 文件上传

## MultipartResolver Spring中用于文件上传的解析器

```java
<bean id="multipartResolver"class="org.springframework.web.multipart.commons.CommonsMultipartResolver">
    <property name="maxUploadSize" value="10485760" />
</bean>
```
## html标签中需要制定文件类型，即entype="multipart/form-data"

```java
<form method="post" action="upload.html" enctype="multipart/form-data">
    <input type="file" name="paper" />
    <input type="text" name="name"/>
    <input type="submit"/>
</form>
```
---

# properties placeHolder

```java
<bean id="propertyConfigurer" class="org.springframework.beans.factory.config.PropertyPlaceHolderConfigurer">
    <property name="location" value="classpath:service.properties"/>
</bean>

properties文件中值的使用：value="${xxx.xxx}"
```