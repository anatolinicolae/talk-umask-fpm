## AI is my best friend

<v-clicks>

- "Chiediamo a Grok, tanto è free"—cit
- "You're absolutely right, lancia questo comando:"
- ```bash
  root@web3:~# grep -r "listen = " /etc/php/ 
  /etc/php/7.2/fpm/pool.d/default.conf:listen = 127.0.0.1:12000
  /etc/php/7.3/fpm/pool.d/default.conf:listen = 127.0.0.1:13000
  /etc/php/7.4/fpm/pool.d/default.conf:listen = 127.0.0.1:14000
  /etc/php/8.2/fpm/pool.d/default.conf:listen = 127.0.0.1:17000
  /etc/php/8.3/fpm/pool.d/default.conf:listen = 127.0.0.1:18000
  /etc/php/8.3/fpm/pool.d/domain3.com.conf:listen = 127.0.0.1:18001
  /etc/php/8.3/fpm/pool.d/domain4.com.conf:listen = 127.0.0.1:18001
  /etc/php/8.4/fpm/pool.d/default.conf:listen = 127.0.0.1:19000
  /etc/php/8.4/fpm/pool.d/domain1.com.conf:listen = 127.0.0.1:19001
  /etc/php/8.4/fpm/pool.d/domain2.com.conf:listen = 127.0.0.1:19002
  ```
- ```bash
  root@web3:~# sqlite3 /home/clp/htdocs/app/data/db.sq3 "SELECT s.domain_name, ps.php_version, ps.pool_port FROM site s LEFT JOIN php_settings ps ON s.php_settings_id = ps.id WHERE s.php_settings_id IS NOT NULL;"
  domain1.com|8.4|19001
  domain2.com|8.4|19002
  domain3.com|8.3|18001
  domain4.com|8.3|18001
  ```
</v-clicks>
