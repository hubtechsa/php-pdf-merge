# PDF Merge for PHP

PDF Merge library for PHP.

Install with composer:

`composer require hubdesksa/pdf-merge`

Should add dependency:

```json
"hubdesksa/pdf-merge": "^2.0"
```

## Highlights

Pdf merging with modes portrait/landscape.

## Usage

```php
// Autoload composer classses...

// and now we can use library
$pdf = new \Jurosh\PDFMerge\PDFMerger;

// add as many pdfs as you want
$pdf->addPDF('path/to/source/file.pdf', 'all', 'vertical')
  ->addPDF('path/to/source/file1.pdf', 'all')
  ->addPDF('path/to/source/file2.pdf', 'all', 'horizontal');

// call merge, output format `file`
$pdf->merge('file', 'path/to/export/dir/file.pdf');
```

That's it!

Enjoy and leave star if you like it :)
