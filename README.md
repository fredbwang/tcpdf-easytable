# tcpdf-easytable

This is a tcpdf compatible easy-table.

Original code is from [fpdf-easytable](https://github.com/fpdf-easytable/fpdf-easytable) 

## Usage

Usage are almost the same, except that you need to modify the fonts file in font folder.
simply change the $cw keys from real characters to ascii code or unicode instead.

original your-font.php is like
```php
// some config

$cw = chr(0)=>278,chr(1)=>278,chr(2)=>278,chr(3)=>278,chr(4)=>278,chr(5)=>278, ...

```
modified:
```php

// some config

$cw = 0=>278,1=>278,2=>278,3=>278,4=>278,5=>278, ...

```

If you want to use other font file of ttf format as your font, simply use 
```php
TCPDF_FONTS::addTTFfont('path/to/your/ttf/file', 'TrueTypeUnicode');
```
see details at [TCPDF_FONT DOC](https://tcpdf.org/docs/srcdoc/TCPDF/class-TCPDF_FONTS/)
