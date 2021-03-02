# Some Prstashop technical issues I came across

#### 1. Prestashop logs me out immediately after logging in

Solution(MySQL query):

```
$ UPDATE ps_configuration SET value = 0 WHERE name='PS_COOKIE_CHECKIP';
```