# TBKB BabyBot

## Help page

###List of commands:

#### list_issue

List all issues of a repository.

> list_issue repo_name

#### today_issue

List all issues which were created today.

> today_issue repo_name

#### yesterday_issue

List all issues which were created BEFORE today.

> yesterday_issue repo_name

#### list_label

List labels of a repository, for creating issue later

> list_label repo_name

#### list_assignee

List assignee of a repository, for creating issue later

> list_assignee repo_name

#### add_issue

Add an issue to one repository, can set label and assignee

> add_issue_<label> <repo> <assignee> title
>  nội dung dòng 1
>  nội dung dòng 2
>  nội dung dòng 3(cho phép nhiều dòng)

Tạo một issue thuộc <label>.

#### trans

Translate the text into english

Example:

> trans だいじょうぶです


#### trans_chat

Translate the last messages text into english

Example: 

> trans_chat 2

#### save_chat

Create an issue in github with the last chat messages

Format: 
> save_chat <repo> <title> <line_count>
Or
> save_chat_label <repo> <title> <line_count>

Example:

1. Create an issue in github repo name: big_project, with title: Hello, World, content is 12 last chat messages.

> save_chat big_project Hello, World 12

2. Create an issue with label **bug** in github repo name: big_project, with title: Hello, World, content is 12 last chat messages

> save_chat_bug big_project Hello, World 12

#### load_month_worktime

return all messages which can be related to worktime

Note 1: resource consuming command, limit the usage to save bot resource.

Note 2: multiple responses, don't use on group, should directly chat to the bot.

#### load_month_task

return all messages which can be related to tasks

Note 1: resource consuming command, limit the usage to save bot resource.

Note 2: multiple responses, don't use on group, should directly chat to the bot.

#### who are you

#### what you do

Test commands

#### bot_help

Lead to this page
