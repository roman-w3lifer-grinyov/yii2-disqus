# yii2-disqus

- [Installation](#installation)
- [Usage](#usage)

## Installation

``` shell
composer require w3lifer/yii2-disqus
```

## Usage

Note, that the number of comments and settings related to comments (https://disqus.com/admin/settings/community) are updated approximately every 20 minutes.

``` php
/**
 * @var $this \yii\web\View
 */

use w3lifer\yii2\Disqus;

// Widget

echo Disqus::widget([
    'shortName' => '<short name>', // Required
    'pageUrl' => '<page url>', // Optional
    'pageIdentifier' => '<page identifier>', // Optional
    'language' => '<language>', // Optional; default `Yii::$app->language`
]);

// Number of comments (since 1.1.0)

Disqus::widget([
    'shortName' => '<short name>', // Required
    'onlyCountComments' => true,
]);
```
