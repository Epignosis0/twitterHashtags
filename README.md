Extracting Hashtags from a string in PHP
======================================
- This is a helper function with unicode support to extract the hashtags that exists in a string.

##To use this function
#### 1. Require the helper file in your project
 ```php
<?php
require_once('helper.php'); 
```

#### 2. Pass a string as an argument to the function:
 ```php 
$sometext = "I'm a #Persian #Programmer. \n My native language is #فارسی";
echo tagExtract($sometext); 
```  
 Output:
 <code>
 I'm a <a href="?lookfor=Persian">#Persian</a> <a href="?lookfor=Programmer">#Programmer</a>. <br> My native language is <a href="?lookfor=فارسی">#فارسی</a>
</code> 

##### Note: if you just need to export hashtags, pass the 'tagsOnly' argument :
 ```php 
$sometext = "I'm a #Persian #Programmer. \n My native language is #فارسی";
echo tagExtract($sometext,'tagsOnly'); 
```  
 Output:
 ```html 
#Persian #Programmer #فارسی
```  

 

## Copyright and license
#### Code released under MIT License 
