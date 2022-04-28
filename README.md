# JavaScript convert string to URL slug with Persian support (تولید اسلاگ مناسب URL با پشتیبانی از زبان فارسی)

## Introduction

> if you want to convert string to slug and make a slugify URL with Persian support you could use this function

> به کمک تابع زیر میتوانید رشته خود را به یک متن اسلاگ تبدیل کنید که برای تولید لینک ها بسیار کاربردی است این تابع زبان فارسی را نیز پشتیبانی میکند

## Code Samples

>     
     function slug(titleStr){
            titleStr = titleStr.replace(/^\s+|\s+$/g, '');
            titleStr = titleStr.toLowerCase();
           //persian support
            titleStr = titleStr.replace(/[^a-z0-9_\s-ءاأإآؤئبتثجحخدذرزسشصضطظعغفقكلمنهويةى]#u/, '') 
            // Collapse whitespace and replace by -
                .replace(/\s+/g, '-')
                // Collapse dashes
                .replace(/-+/g, '-');
            return titleStr;       
    }

## Installation

> use this function at the end of your scripts and call it everywhere you want, so your string converts to slug and you could use that for creating links and URLs
