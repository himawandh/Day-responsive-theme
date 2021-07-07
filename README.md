# Day plugin for CakePHP

## Installation

You can install this plugin into your CakePHP application using [composer](https://getcomposer.org).

The recommended way to install composer packages is:

```
composer require day-responsive-theme/day
```
```php
// src/Controller/AppController.php
use Cake\Event\EventInterface;

public function beforeRender(EventInterface  $event)
{
    $this->viewBuilder()->setTheme('Day');
}

//src/Application.php
public function bootstrap(): void
{
  $this->addPlugin('Day');
}

//config/paths.php
/***email setup *****/
define('EMAIL_TRANSPORTS','your email transport');
define('EMAIL_CAPTION','your email caption');
define('EMAIL_HOST','your email host');
define('EMAIL_PORT','your email port');
define('EMAIL_ADDRESS','your email address');
define('EMAIL_PASSWORD','your email password');
/**Company Setup***/
define('SITES_CODE','your site code');
define('COMPANY_NAME','your company name');
define('COMPANY_CODE','your company code');
define('COMPANY_ADDRESS','your company code');
define('COMPANY_PHONE','your company phone');
define('COMPANY_FAX','your company fax');
define('COMPANY_EMAIL','your company email');
define('COMPANY_REMARKS','your company remark');
define('COMPANY_SITES','your company sites');
define('COMPANY_INITIALS_FIRST','your first company initial');
define('COMPANY_INITIALS_LAST','your last company initial');
/* meta tag */
define('TAG_TITLE','your tag title');
define('TAG_DESCRIPTION','your tag description');
define('TAG_KEYWORD','your tag keyword');
define('TAG_AUTHOR','your tag author');
