# scss
html/scss 


/ variable $main-font-family: Arial, 'sans-serif' 
$main-font-size: 1.4rem 
$main-font-color: #444 
$font-size-e: 1.8rem

$main-width: 640px 
$main-padding: 1.5rem

$content-sub-w: 208px 
$content-img-w: 96px 
$content-list-h: 96px

// normalize //
@import 'normalize'

// mixin 
@mixin clearfix 
&::after content: '' 
display: block 
clear: both 
@mixin text-ellipsis text-overflow: ellipsis white-space: nowrap overflow: hidden 
@mixin center-content($set-width) width: $set-width margin: 0 auto 
@mixin circle-obj($set-width) 
width: $set-width
 height: $set-width 
 line-height: $set-width 
 text-align: center 
 overflow: hidden 
 border-radius: 50rem
