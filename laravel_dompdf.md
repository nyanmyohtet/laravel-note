# laravel-dompdf

GitHub Repo: https://github.com/barryvdh/laravel-dompdf

## Installation

`composer require barryvdh/laravel-dompdf`

## Setup

Add the ServiceProvider to the providers array in `config/app.php`

`Barryvdh\DomPDF\ServiceProvider::class,`

You can optionally use the facade for shorter code. Add this to your facades:

`'PDF' => Barryvdh\DomPDF\Facade::class,`

## Usage

You can create a new DOMPDF instance and load a HTML string, file or view name. You can save it to a file, or stream (show in browser) or download.

```php
$pdf = App::make('dompdf.wrapper');
$pdf->loadHTML('<h1>Test</h1>');
return $pdf->stream();
```

Or use the facade:

```php
$pdf = PDF::loadView('pdf.invoice', $data);
return $pdf->download('invoice.pdf');
```

## Setting PDF Resolution

dpi: 96 (available in config/dompdf.php)
