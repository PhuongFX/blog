---
layout: article
title: ⌖Chương trình quản lý nhân viên
abstract: Chương trình giúp quản lý và tính tiền lương hàng tháng của các nhân viên trong công ty
categories: Demo
tags: Python
eyeCatcher: https://img.rawpixel.com/s3fs-private/rawpixel_images/website_content/v430-adj-42-acrylictexture_2.jpg?w=800&dpr=1&fit=default&crop=default&q=65&vib=3&con=3&usm=15&bg=F4F4F3&ixlib=js-2.2.1&s=e283f157f1a5c95c4873022041295af0
---

---


**Quản lý và tính tiền lương hàng tháng nhân viên trong công ty**
=====================================

## `Tài nguyên`

[File thông tin thuế TNCN (XML)](https://firebasestorage.googleapis.com/v0/b/funix-way.appspot.com/o/xSeries%2FChung%20chi%20dieu%20kien%2FPYB101x_1.1%2FASM_Resources%2Ftax.xml?alt=media&token=f7a6f73d-9e6d-4807-bb14-efc6875442c7)

* min < lương chịu thuế <= max
~~~
<tax>
	<min>0</min>
	<max>5</max>
	<value>5</value>
</tax>
<tax>
	<min>5</min>
	<max>10</max>
	<value>10</value>
</tax>
...
~~~


[File thông tin mức phạt đi muộn (JSON)](https://firebasestorage.googleapis.com/v0/b/funix-way.appspot.com/o/xSeries%2FChung%20chi%20dieu%20kien%2FPYB101x_1.1%2FASM_Resources%2Flate_coming.json?alt=media&token=55246ee9-44fa-4642-aca2-dde101d705de)



## `Class`

| Department            | Nhân viên thường (Employee)      | Quản lý (Manager)                  |
|-----------------------|----------------------------------|------------------------------------|


> ### Employee, Manager
* id: Mã số nhân viên
* name: Họ và tên nhân viên
* salary_base: Hệ số lương cơ bản
* working_days: Số ngày làm việc trong tháng
* department: Mã bộ phận
* working_performance: Hệ số hiệu quả
* bonus: Thưởng
* late_comming_days: Số ngày đi muộn

> ### Department
* id: Mã bộ phận
* bonus_salary: Thưởng bộ phận




* Có màn hình menu hiển thị tất cả các chức năng
* Có chức năng thêm/sửa/xóa nhân viên mới
* Có chức năng hiển thị lương của từng nhân viên
