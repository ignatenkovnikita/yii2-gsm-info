Client for gsm info
===================
Client for gsm info

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist ignatenkovnikita/yii2-gsm-info "*"
```

or add

```
"ignatenkovnikita/yii2-gsm-info": "*"
```

to the require section of your `composer.json` file.


Usage
-----

Add this to your main configuration's components array:

```php
'gsmInfo' => [
            'class' =>  \ignatenkovnikita\refillmobile\ClientGsmInfo::className(),
            'url' => your_url,
            'user' => your_user,
            'pass' => your_pass,
        ],
```
Typical component usage
-----------------------
```php
Yii::$app->gsmInfo->getInfo(7 your_phone);
Yii::$app->gsmInfo->getRegion(7 your_phone);
```
