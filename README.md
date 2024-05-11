# SchoolManager
------------------------------------
با صحبتی که با یکی از مدارس شیراز داشتیم ، قرار شد سیستم مدیریت معلمین و دانش آموزان را برای این مدرسه پایه ریزی کنیم . طبقه گفتگو با مدیر مدرسه چیزی که مدیر در لحظه اول میخواهد این است : 
1. مدیریت دانش آموزان :
     - نام
     - نام خانوادگی
     - کد ملی
     - تلفن
     - نام پدر
     - تلفن پدر
     - آدرس
3. مدیریت معلمین
4. مدیریت دروس
5. وارد کردن نمرات دانش آموزان
6. وارد کردن ورود و خروج معلمین
7. صادر کردن کارنامه دانش آموزان
8. دیدن برنامه کلاسی به نسبت هر درس یا هر کلاس یا هر معلم

## در قدم اول شما به عنوان شخص فنی باید بتوانید داده های مورد نظر هر بخش را تحلیل کرده و سیستم مورد نیاز برای هر بخش درست کنید . 

----------------------------------------------------
## Instructions :  
### 1. Manage students : 
- Entity Student :
  - Name
  - Family
  - Nationnal Id
  - Cell-Phone
  - Phone
  - Address
  - FatherName
  - Father-Phone
- Api Student :
    - Get by Id
    - Get by national id
    - Gets by filter
        - if empty filter then get all students base pagination
    - Add a new student
    - Update a new student
    - Delete a new Student
- Test Student :
    - Write some integration test for APIS
---------------------------------------------------------------------------
### 2. Manage Teachers : 
- Entity Teacher :
    - Name
    - Family
    - National Code
    - Cell-Phone
    - Phone
    - BirthDate
    - Address
- Api Student :
    - Get by Id
    - Get by national code
    - Get by filter
        { optinal name,optional family,optional birthdate, optional nationalId}
    - Add new teacher
    - Update a teacher
    - Delete a teacher
- Test Teacher :
    - write some integration tests for APIS
----------------------------------------------------------------------------
### 4. Manage Course :
- Entity Course :
    - Name
    - Code
- Api Course :
    - Get by Id
    - Get by code
    - Get by name
    - Get by filter {optional Id,optional name,optional code}
    - Add new course
    - update a course
    - delete a course
    - delete all course
- Test course Api :
    - Write some integration tests for APIS
--------------------------------------------------------------------------------
### 5. Manage Authentication and Authorization
- JWT token without refresh token .
- Custom manage authorization
- Check authentication and authorization on each api
---------------------------------------------------------------------------------
### 6. Report Section : 
-  دریافت برنامه کلاسی
    - بر اساس دانش آموز
      - بر اساس معلم
      - بر اساس کلاس
      - بر اساس درس

- دریافت کارنامه شخص
  
