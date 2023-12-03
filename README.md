# Generate text watermark with canvas for dcat-admin

Add Generate Text  Watermark in dcat-admin web page.




## Install

```bash
composer require bilwy/watermark
```

## Configurations

Add `extensions` option in your `config/admin.php` configuration file:

```php
'extensions' => [
    'watermark' => [
        'enable' => true,
        'config' => [
            'content' => 'username', // Admin::user()->username, or Admin::user()->name or fixed value like 'internal info'
            'width' => '100px',
            'height' => '120px',
            'textAlign' => 'left',
            'textBaseline' => 'alphabetic',
            'font' => '15px Times New Roman',
            'fillStyle' => 'rgba(204,204,204,0.4)',
            'rotate' => 30,
            'zIndex' => 1000,
        ]
    ]
]
```

