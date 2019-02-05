Yii2-select2
========

[Select2](https://select2.github.io/) gives you a customizable select box with support for searching, tagging, remote
data sets, infinite scrolling, and many other highly used options.

##Installation

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
$ php composer.phar require pcrt/yii2-select "*"
```

or add

```
"pcrt/yii2-select2": "*"
```

to the require section of your `composer.json` file.

## Usage

Once the extension is installed, modify your application configuration to include:

```php
use pcrt\widgets\select2\Select2:


// with \yii\bootstrap\ActiveForm;
echo $form
    ->field($model, 'attribute')
    ->widget(
        Select2::class, 
        [
            'items' => $data, // $data should be the same as the items provided to a regular yii2 dropdownlist
        ]
    );

// as widget
echo Select2::widget([
    'name' => 'my-name',
    'value' => 'my-value',
    'clientOptions' => [
        'maximumInputLength' => 20
    ]
]);
```

## License

Yii2-select2 is released under the BSD-3 License. See the bundled `LICENSE.md` for details.

Enjoy!
