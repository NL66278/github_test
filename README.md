github_test
===========

Just testing how github works....
```
mermaid

graph TD;
id1((Widget to place membership in any position))-->id2[CLICK on BUY MEMBERSHIP ON ANY PAGE];
id2 --> idq1{Is the user logged in?};
idq1 --> |YES|id4[load form1 with prefilled email and only questions and IBAN];
idq1 --> |NO|id5[COMPILE EMAIL AND QUESTIONS, SUBMIT form];
id5 --> idq2{Is the email connected to a user?};
idq2 --> |YES|id6[Redirect to login page with precompiled email];
idq2 --> |NO|idq3{Is the email in the CRM contacts?};
idq3 --> |YES|id7[Create user, send confirmation email to customer];
id7 --> id8[user confirms email];
idq3 --> |NO|id9[FORM 2 - insert new user data];
id9 --> id7;
id8 --> id10[CART WITH MEMBERSHIP TO BUY];
id6 --> id10;
id4 --> id10;
id10 --> id11((USER IS MEMBER));

```
