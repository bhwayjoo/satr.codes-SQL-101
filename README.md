# satr.codes-SQL-101
مشروع

باستخدام ماتعلمته خلال هذهِ الدورة قم بتطبيق الآتي: لنفترض أن هناك مدرسة باسم التميز للتعليم الثانوي، ونريد إنشاء قاعدة بيانات مركزية لتضم جميع معلومات المعلمين والطلاب والمواد، مع العلم أنه يجب تخزين المعلومات الآتية لكل طالب (الرقم التسلسلي للطالب، اسم الطالب، تاريخ الميلاد، جنس الطالب، تاريخ الالتحاق، البريد الإلكتروني للطالب، المستوى الدراسي، المسار، المعدل التراكمي للطالب) ومعلومات المعلمين كالآتي(الرقم التسلسلي للمعلم، اسم المعلم، تاريخ الميلاد، جنس المعلم، البريد الالكتروني للمعلم، رقم المكتب) ومعلومات المواد كالآتي (الرقم التسلسلي للمادة، اسم المادة).

المتطلبات:


استخدام التعليقات comments لتوضيح الأوامر.
إنشاء قاعدة البيانات.
إنشاء الجداول.
عرض الجداول المتاحة في قاعدة البيانات.
إدخال معلومات ٣٠ طالب كحد أدنى.
إدخال معلومات ١٠ معلمين كحد أدنى.
إدخال معلومات ٦ مواد كحد أدنى.
عرض محتويات جميع الجداول.
عرض محتويات جدول الطلاب مع ترتيب الصفوف تصاعديًا حسب اسم الطالب.
عرض محتويات جدول الطلاب مع إعطاء اسم مستعار لحقل “اسم الطالب” لاختصار اسم العمود أو جعله ذات معنى.
التعديل على البيانات.
التعديل على بيانات أحد الطلاب وتغيير البريد الالكتروني للطالب.
التعديل على بيانات أحد المعلمين وتغيير رقم المكتب الخاص به.
التعديل على الجداول.
تعديل اسم أحد الجداول.

ملاحظات:


الرقم التسلسلي هو id.
الجنس (F أو M).
المستوى الدراسي يتكون من ستة مستويات (1, 2, 3، 4, 5, 6).
المسار (علمي أو انساني).
المعدل التراكمي من 100














use ExcellenceForSecondaryEducation ;
create database ExcellenceForSecondaryEducation





use ExcellenceForSecondaryEducation ;
create table student( StudentSerialNumber int primary key,  StudentName varchar (255), BirthDay date ,  sex varchar (50),  EntryDay date ,  mail varchar (250) , study varchar (255))





use ExcellenceForSecondaryEducation ;
create table teacher( teacherSerialNumber int primary key,  teacherName varchar (255), BirthDay date ,  sex varchar (50),  EntryDay date , mail varchar (250) , officeNumber varchar(255))




use ExcellenceForSecondaryEducation ;
create table sbject ( SubjectSerialNumber int primary key,  sbjectName varchar (255))




use ExcellenceForSecondaryEducation ;
show tables




use ExcellenceForSecondaryEducation ;
insert into student values (2, 'John Clark', '2002-02-20','male',now(),'sfXXS5v1@gmail.com','pc'), (3, 'Bob Brown', '2009-07-07','male',now(),'6A7le7pz@outlook.com','pc'), (4, 'Michael Brown', '2012-01-23','male',now(),'Ed41nulM@gmail.com','svt'), (5, 'Olivia Davis', '2018-05-20','male',now(),'dnjEvwIM@gmail.com','pc'), (6, 'Eva Jones', '2013-12-21','male',now(),'wjqjh3MQ@yahoo.com','svt'), (7, 'Jane Davis', '2022-12-24','male',now(),'9vUjVJZB@example.com','math'), (8, 'David Johnson', '2003-03-18','male',now(),'uF08AIz7@gmail.com','svt'), (9, 'John Jones', '2022-04-17','male',now(),'eTTJszEU@example.com','math'), (10, 'Olivia Miller', '2004-04-01','male',now(),'X631s22h@example.com','math'), (11, 'Jane Jones', '2006-12-03','male',now(),'gpwnNfeB@example.com','svt'), (12, 'Jane Jones', '2014-02-26','male',now(),'ky1NLBy1@randommail.net','svt'), (13, 'Alice Jones', '2012-03-18','male',now(),'CtCh5dYB@randommail.net','pc'), (14, 'Bob Miller', '2012-01-27','male',now(),'6DI9Pfn1@outlook.com','svt'), (15, 'Alice Johnson', '2014-03-27','male',now(),'PHjHtDon@outlook.com','math'), (16, 'Olivia Johnson', '2005-05-04','male',now(),'ro8Qrqe0@gmail.com','math'), (17, 'Jane Brown', '2007-06-11','male',now(),'whNPG15D@gmail.com','svt'), (18, 'Alice Davis', '2003-03-02','male',now(),'hR6uRgva@yahoo.com','pc'), (19, 'Eva Johnson', '2007-10-10','male',now(),'qoFsmiIB@yahoo.com','svt'), (20, 'Alice Miller', '2003-11-19','male',now(),'7f9Ghksd@example.com','pc'), (21, 'Jane Wilson', '2011-10-01','male',now(),'5VWFAP1F@gmail.com','math'), (22, 'Bob Brown', '2010-10-18','male',now(),'RvITWiij@example.com','svt'), (23, 'Alice Smith', '2011-01-22','male',now(),'kaMgFAZK@randommail.net','math'), (24, 'Eva Jones', '2018-12-05','male',now(),'9cG11HHm@randommail.net','svt'), (25, 'Eva Davis', '2004-09-21','male',now(),'HKgTC9fH@randommail.net','math'), (26, 'David Miller', '2016-01-30','male',now(),'ht0LtL1w@gmail.com','math'), (27, 'David Smith', '2022-05-27','male',now(),'EfWN3UEX@gmail.com','pc'), (28, 'Jane Davis', '2020-10-27','male',now(),'thr6z5YH@yahoo.com','pc'), (29, 'Bob Jones', '2010-12-05','male',now(),'2b1i6Orq@yahoo.com','math'), (30, 'David Brown', '2016-12-05','male',now(),'nBQpO7D3@randommail.net','math'), (31, 'Olivia Miller', '2000-04-30','male',now(),'VlPNFdn4@gmail.com','math')



use ExcellenceForSecondaryEducation ;
insert into teacher values(1, 'Jane Johnson', '2010-05-30','male',now(),'G9DbNHCN@gmail.com','10'), (2, 'Alice Davis', '2012-01-07','male',now(),'a3968FNw@gmail.com','15'), (3, 'David Clark', '2014-09-17','male',now(),'wegWTBCk@gmail.com','20'), (4, 'Bob Davis', '2010-02-05','male',now(),'Jk68BibL@randommail.net','25'), (5, 'Michael Davis', '2013-09-24','male',now(),'RFEGF0Cy@outlook.com','30'), (6, 'Michael Wilson', '2007-02-22','male',now(),'WDl6ALYX@yahoo.com','35'), (7, 'Michael Miller', '2010-10-25','male',now(),'qJuf50wm@example.com','40'), (8, 'David Miller', '2014-08-24','male',now(),'9DZB5JwR@example.com','45'), (9, 'David Brown', '2014-04-16','male',now(),'FZP9mXnO@example.com','50'), (10, 'John Smith', '2021-11-18','male',now(),'Y7h609Ky@example.com','55'), (11, 'Eva Miller', '2013-10-06','male',now(),'XevwApOi@randommail.net','60'), (12, 'John Johnson', '2016-10-05','male',now(),'EZewOdfN@example.com','65'), (13, 'Olivia Davis', '2003-09-06','male',now(),'1ftyRBNL@gmail.com','70'), (14, 'David Miller', '2009-04-01','male',now(),'sppUM4qU@example.com','75'), (15, 'David Brown', '2019-04-07','male',now(),'CcWcH7zj@yahoo.com','80'), (16, 'Bob Davis', '2008-02-02','male',now(),'oijCuQ0c@yahoo.com','85'), (17, 'Michael Johnson', '2014-02-02','male',now(),'vGUo60yN@yahoo.com','90'), (18, 'David Clark', '2003-10-06','male',now(),'gWWbEHQ3@yahoo.com','95'), (19, 'Eva Smith', '2021-03-06','male',now(),'7A7ye595@yahoo.com','100'), (20, 'John Wilson', '2022-08-23','male',now(),'dptxoZKx@gmail.com','105'), (21, 'Bob Jones', '2022-03-21','male',now(),'AtRU36Ul@randommail.net','110'), (22, 'Jane Miller', '2006-05-18','male',now(),'rcV3DDfM@outlook.com','115'), (23, 'John Davis', '2018-07-13','male',now(),'av2NIY8z@example.com','120'), (24, 'David Wilson', '2015-06-25','male',now(),'vImsDwzh@yahoo.com','125'), (25, 'Olivia Clark', '2015-10-19','male',now(),'tHfQ1fMq@randommail.net','130'), (26, 'Bob Jones', '2021-03-23','male',now(),'AJ9efOim@example.com','135'), (27, 'Eva Johnson', '2011-01-21','male',now(),'FSsNGMBy@yahoo.com','140'), (28, 'Alice Davis', '2015-03-29','male',now(),'zkVAWjxl@example.com','145'), (29, 'John Wilson', '2013-06-06','male',now(),'q0O7h5sL@example.com','150'), (30, 'Jane Miller', '2009-04-10','male',now(),'w55QFlSY@example.com','155')






use ExcellenceForSecondaryEducation ;
insert into sbject values (1,'pc'), (2,'math'), (3,'ar'), (4,'fr'), (5,'eng'), (6,'sport'), (7,'S.V.T')






use ExcellenceForSecondaryEducation ;
insert into sbject
values (1,'pc'),
(2,'math'),
(3,'ar'),
(4,'fr'),
(5,'eng'),
(6,'sport'),
(7,'S.V.T');
select * from sbject;





use ExcellenceForSecondaryEducation ;
select * from sbject;
select * from student;
select * from teacher;


use ExcellenceForSecondaryEducation;
select * from student order by StudentName asc



use ExcellenceForSecondaryEducation;
SELECT StudentSerialNumber AS ID, StudentName AS SN, BirthDay, sex, EntryDay, mail,study FROM Student;










use ExcellenceForSecondaryEducation;
update student
set mail = 'gmail@gmail.com' where StudentSerialNumber=1;
select * from student 




use ExcellenceForSecondaryEducation;
update teacher
set officeNumber = 2 where teacherSerialNumber=1;
select * from teacher 





use ExcellenceForSecondaryEducation;
alter table sbject
rename to sbjectt
