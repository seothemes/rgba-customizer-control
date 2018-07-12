This is a fork of [https://github.com/BraadMartin/components](https://github.com/BraadMartin/components) which has been converted into a composer package.

## Installation

```shell
composer require seothemes/rgba-customizer-control
```

## Setup

RGBA Customizer Control uses PSR-4 autoloading.

To use in your theme or plugin, use the following namespace:

```shell
use SEOThemes\RgbaCustomizerControl\RgbaCustomizerControl;
```

Once the namespace has been imported you can simply call the class:

```php
new RgbaCustomizerControl;
```

Example:

```php
$wp_customize->add_control(
	new RgbaCustomizerControl (
		$wp_customize,
		$setting,
		array(
			'section'      => 'colors',
			'label'        => $label,
			'settings'     => $setting,
			'show_opacity' => true,
			'palette'      => true,
		)
	)
);
```
