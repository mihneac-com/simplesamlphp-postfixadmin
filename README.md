# simplesamlphp-postfixadmin
Simplesamlphp module for postfixadmin user backend with md5-crypt

https://mihneac.com/saml/simplesaml_postfixadmin


authsources config:
<code php>
  'postfixadmin-sql' => [
     'postfixadmin:SQL',
     'dsn' => 'mysql:host=localhost;port=3306;dbname=simplesaml',     
     'username' => 'simplesaml',     
     'password' => 'yourpassword',    
     'append_domain' => 'yourdomain.com',    
],
</code>
Options:

 * dsn - mysql/pgsql connect url
 * username/password - database access credentials
 * append_domain (OPTIONAL) - will append @yourdomain.com if the username entered is not an email address. If parameter is not specified, username is left as is.
