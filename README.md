# Yii2 Log Target for Datadog

INSTALL
=======
```
composer require "lfg\yii2-datadog-target"
```

USAGE
=====
Add new log target in application configuration: 
```
    'log'           => [
        'targets'    => [
            'datadog' => [
                'class' => 'lfg\DatadogCounter',
                'levels' => ['error', 'warning'],
                'tags' => ['tag1', 'tag2'], // optional
                'metricPrefix' => 'front', // required
            ],
        ],
    ],
```

### TODO

- Send events to Datadog 

### LINKS

- [Datadog](https://www.datadoghq.com/)
- [Yii2 log documentation](http://www.yiiframework.com/doc-2.0/guide-runtime-logging.html)