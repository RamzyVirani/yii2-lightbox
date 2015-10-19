Lightbox Widget for Yii 2
=========
- Lightbox widget based on Lightbox2 extension http://lokeshdhakar.com/projects/lightbox2/

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist ramzyvirani/yii2-lightbox "*"
```

or add

```json
"ramzyvirani/yii2-lightbox": "*"
```

to the require section of your composer.json.

Usage
------------
Once the extension is installed, simply add widget to your page as follows:

```php
echo Lightbox::widget([
    'files' => [
        [
            'thumb' => 'url/to/thumb.ext',
            'original' => 'url/to/original.ext',
            'title' => 'optional title',
        ],
    ]
]);
```

To add html options you can use below syntax

```php
echo Lightbox::widget([
    'files' => [
        [
            'thumb' => [
                'src'=>'url/to/thumb.ext',
                'htmlOptions' => ['class'=>'col-md-12', 'alt'=>'Alternate Text'] // These options will be applied to Image tag.
            ],
            'original' => [
                'src' => 'url/to/original.ext',
            ]
            'title' => 'optional title',
        ],
    ]
]);
```

