# TBKB BabyBot

## Tài liệu hỗ trợ:

###Danh sách lệnh:

#### list_issue

Liệt kê tất cả các issues (đang mở) trong một repository

> list_issue repo_name

#### today_issue

Liệt kê tất cả các issues (đang mở) trong một repository, được tạo hôm nay

> today_issue repo_name

#### yesterday_issue

Liệt kê tất cả các issues (đang mở) trong một repository, được tạo trước hôm nay

> yesterday_issue repo_name

#### list_label

Liệt kê các label trong một repository, dùng để tạo issue sau đó (add_issue hoặc là save_chat)

> list_label repo_name

#### list_assignee

Liệt kê các assignee (username) trong một repository, dùng để tạo issue sau đó (add_issue)

> list_assignee repo_name

#### add_issue

Tạo một isssue trong một repository, có thể đặt label và assignee

> add_issue_label repo_name assignee title

>  nội dung dòng 1

>  nội dung dòng 2

>  nội dung dòng 3(cho phép nhiều dòng)

Tạo một issue và gán label cho nó.

Vd: tạo 1 issue label 'documentation', trong repo 'big_project', assign cho 'hardwarelayer', title 'Hello, World Task'

> add_issue_documentation big_project hardwarelayer Hello, World Task

> dòng 1 của content

> dòng 2 của content

> dòng 3 của content

> dòng 4 của content

> dòng 5 của content

Chú ý: label và assignee phải tồn tại trong repo!

#### save_chat

Tạo một issue trong repository với nội dung là các dòng chat mới được gửi vào group chat hiện tại.

Vd: 

> save_chat repo_name title line_count

Hoặc là

> save_chat_label repo_name title line_count

Ví dụ:

1. Tạo một issue với repo tên là: big_project, tiêu đề là: 'Hello, World', nội dung là 12 dòng chat gần nhất.

> save_chat big_project Hello, World 12

2. Tạo một issue với label là **bug** trong repo tên là: big_project, với tiêu đề là: 'Hello, World', nội dung là 2 dòng chat gần nhất

> save_chat_bug big_project Hello, World 2

#### trans

Dịch một đoạn text ra tiếng Anh

Vd:

> trans だいじょうぶです


#### trans_chat

Dịch các message chat vừa xong trong chat group hiện tại ra tiếng Anh.

vd: Dịch 2 dòng vừa xong ra tiếng Anh

> trans_chat 2

#### load_month_worktime

trả về các message có thể liên quan tới thời gian làm việc: đi trễ, về sớm, nghỉ nửa ngày, 1 ngày ... trong tháng

Chú ý 1: Lệnh này tốn tài nguyên, không nên dùng nhiều

Chú ý 2: Có thể trả về rất nhiều message, đừng dùng trong nhóm chat mà hãy chat trực tiếp với bot

#### load_month_task

Trả về tất cả các message trong tháng có thể liên quan tới assign task

Chú ý 1: Lệnh này tốn tài nguyên, không nên dùng nhiều

Chú ý 2: Có thể trả về rất nhiều message, đừng dùng trong nhóm chat mà hãy chat trực tiếp với bot

#### who are you

#### what you do

Test commands

#### bot_help

Lead to this page


### Chú ý:

TBKBBB chỉ làm việc với các group và user được cấu hình từ trước!


