README

### Installation
1. Run `composer require arvin/toastr-for-laravel`
2. Add `Arvin\Toastr\ToastrServiceProvider::class`, to **providers** in `config/app.php`
3. Add `'Toastr' => Arvin\Toastr\Facades\Toastr::class`, to **aliases** in `config/app.php`
4. Run `php artisan vendor:publish`

### Usage

Just add this code to your blade template file:

```php
{!! Toastr::render() !!}
```
Use these methods in controllers:

```php
Toastr::warning($message, $title = null, $options = []) 
Toastr::error($message, $title = null, $options = []) 
Toastr::info($message, $title = null, $options = [])
Toastr::success($message, $title = null, $options = [])
Toastr::clear() 
```

#### Config

set the toaster options in `config/toastr.php` , available options => [toastr.js demo](http://codeseven.github.io/toastr/demo.html)
