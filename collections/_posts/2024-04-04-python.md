---
layout: article
title: 🐍Chương trình quản lý nhân viên
abstract: Chương trình giúp quản lý và tính tiền lương hàng tháng của các nhân viên trong công ty. 𝄃𝄃𝄂𝄂𝄀𝄁𝄃𝄂𝄂𝄃 [ENG] ver. at Projects/Software
categories: Demo
tags: Python
eyeCatcher: https://img.rawpixel.com/s3fs-private/rawpixel_images/website_content/v430-adj-42-acrylictexture_2.jpg?w=800&dpr=1&fit=default&crop=default&q=65&vib=3&con=3&usm=15&bg=F4F4F3&ixlib=js-2.2.1&s=e283f157f1a5c95c4873022041295af0
---

---


**Quản lý và tính tiền lương hàng tháng nhân viên trong công ty**
=====================================

<div style="text-align: left;">

  <a href='https://github.com/PhuongFX/ButterFlySpace/blob/main/LICENSE'><img style='display: inline-block; margin: 0; padding: 0;' src='https://img.shields.io/badge/License-AGPL%203.0-blue.svg' alt='License: AGPL-3.0'></a>
  <a href='https://www.python.org/'><img style='display: inline-block; margin: 0; padding: 0;' src='https://img.shields.io/badge/Python-3.x-blue' alt='Python'></a>
  <a href='https://github.com/PhuongFX/python3'><img style='display: inline-block; margin: 0; padding: 0;' src='https://img.shields.io/badge/Open%20Source-%E2%9D%A4-green.svg' alt='Open Source'></a>
  
</div>


<p align='center'>
  <img src="https://raw.githubusercontent.com/PhuongFX/python3/main/Screenshot%202024-09-05%20095431.jpg"/>
</p>


## `Tài nguyên`

[File thông tin thuế TNCN (XML)](https://firebasestorage.googleapis.com/v0/b/funix-way.appspot.com/o/xSeries%2FChung%20chi%20dieu%20kien%2FPYB101x_1.1%2FASM_Resources%2Ftax.xml?alt=media&token=f7a6f73d-9e6d-4807-bb14-efc6875442c7)

* min < lương chịu thuế <= max
  
~~~xml
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

~~~json
{
	"min": 0,
	"max": 3,
	"value": 20000
},
~~~

~~~python
late_comming_days * 20000
~~~


## `Class`

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


## `Menu chức năng`

* Có màn hình menu hiển thị tất cả các chức năng
* Có chức năng thêm/sửa/xóa nhân viên mới
* Có chức năng hiển thị lương của từng nhân viên

~~~
1. Hiển thị danh sách nhân viên.
2. Hiển thị danh sách bộ phận.
3. Thêm nhân viên mới.
4. Xóa nhân viên theo ID.
5. Xóa bộ phân theo ID
6. Hiển thị bảng lương.
7. Thoát.
Mời bạn nhập chức năng mong muốn:
~~~

> ### "Hiển thị danh sách nhân viên"

Với chức năng này, bạn sẽ in ra thông tin của các nhân viên được lưu trong hệ thống, theo format như sau:
~~~
----
Mã số: NV001
Mã bộ phận: SALE001
Chức vụ: Nhân viên
Họ và tên: Nguyễn Văn A
Hệ số lương: 200,000 (VND)
Số ngày làm việc: 26 (ngày)
Hệ số hiệu quả: 1
Thưởng: 500,000 (VND)
Số ngày đi muộn: 2
----
~~~

> ### "Hiển thị danh sách bộ phận"

Với chức năng này, bạn sẽ hiện thị danh sách tất cả các bộ phận đang có, theo format như sau:
~~~
----
Mã bộ phận: SALE01
Thưởng bộ phận: 500,000 (VND)
----
~~~

> ### "Thêm nhân viên mới"

Với chức năng này, người dùng sẽ được thêm một nhân viên mới vào danh sách. Người dùng sẽ được nhập liệu các thông tin cho nhân viên mới như sau:

~~~
----
Thêm nhân viên mới ...
Nhập mã số: 'NV002'
Nhập mã bộ phận: 'SALE002'
Nhập chức vụ (NV / QL): 'NV'
Nhập họ và tên: 'Nguyen Van B'
Nhập hệ sô lương: '300000'
Nhập số ngày làm việc: '25'
Nhập hệ số hiệu quả: '0.8'
Nhập thưởng: '0'
Nhập số ngày đi muộn: '0'
Đã thêm nhân viên mới ...
----
~~~
~~~
Mã bộ phận chưa tồn tại, tạo mới ...
Nhập thưởng bộ phận: 100000
Đã tạo bộ phận mới ...
Đã thêm nhân viên mới ...
~~~

> ### "Xóa nhân viên theo ID"

Với chức năng này, người dùng sẽ nhập ID của nhân viên muốn xóa và xóa nhân viên đó khỏi hệ thống. Ví dụ:

~~~
----
Nhập mã nhân viên muốn xóa: 'NV001'
Đã xóa thành công
----
~~~

> ### "Xóa bộ phận theo ID"

Tương tự với chức năng "Xóa nhân viên theo ID" nhưng là xóa bộ phận trên hệ thống.

> ### "Hiển thị bảng lương"

Với chức năng này, bạn hãy hiển thị bảng lương của tất cả nhân viên trong hệ thống, với format như sau:

~~~
----
Mã số: NV001
Thu nhập thực nhận: 4,961,880 (VND)
----
~~~

> ### "Thoát"

Với chức năng này, chương trình sẽ kết thúc.

> ### "Thêm chức năng chỉnh sửa nhân viên"

Người dùng sẽ nhập vào mã nhân viên muốn chỉnh sửa, sau đó là các trường muốn sửa và giá trị mới. Ví dụ:

~~~
----
Chỉnh sửa nhân viên
Nhập mã nhân viên: 'NV002'

Nhập họ và tên: ...
Nhập chức vụ (NV / QL): ...
Nhập hệ số lương: ...
Nhập số ngày làm việc: ...
Nhập hệ số hiệu quả: ...
Nhập thưởng: ...
Nhập số ngày đi muộn: ...

Đã hoàn tất chỉnh sửa
----
~~~
