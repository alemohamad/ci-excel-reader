# CodeIgniter Library: Excel Reader

**ci-excel-reader**

## About this library

This CodeIgniter's Library is used to read XLS files and return an array with its info.

Its usage is recommended for CodeIgniter 2 or greater.

* The original code can be found in [PHP-ExcelReader](http://sourceforge.net/projects/phpexcelreader/) by Vadim Tkachenko.

## Usage

```php
// Load the spreadsheet reader library
$this->load->library('excel_reader');

// Read the spreadsheet via a relative path to the document
// for example $this->excel_reader->read('./uploads/file.xls');
$this->excel_reader->read('./uploads/file.xls');

// Get the contents of the first worksheet
$worksheet = $this->excel_reader->sheets[0];

$numRows = $worksheet['numRows']; // ex: 14
$numCols = $worksheet['numCols']; // ex: 4
$cells = $worksheet['cells']; // the 1st row are usually the field's name
```

![Ale Mohamad](http://alemohamad.com/github/logo2012am.png)