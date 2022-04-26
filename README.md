# Includer

一个便捷的include的wrapper封装

## 安装

``` bash
composer require diggphp/includer
```

## 用例

### 方式一

``` php
<?php
$phpcode='hello <?php echo $name;?>';
$name='xiaoming';
include \DiggPHP\Includer\Wrapper::write($phpcode);
```

### 方式二

``` php
<?php
$phpcode='hello <?php echo $name;?>';
\DiggPHP\Includer\Wrapper::load($phpcode, ['name'=>'xiaoming']);
```
