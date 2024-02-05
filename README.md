## About Project

1. User can create new help tickets
2. Admin can reply on help tickets ,and he can resolve or reject ticket
3. User get the notification once admin updated the ticket
4. user can upload attachment to the ticket


## Database Structure
1. Ticket - 
   ticket_id {PK,int},
   title {string,req},
   description {text,req},
   status {tinyint, /[open(default),resolved,rejected)/],
   attachment{string, nullable},
   user_id {req},
   assigned_admin{varchar,nullable}

   2. Replies- 
   body {text,req}
   user_id {req}
   ticket_id {req}
