# scss
html/scss 
@import "variable";

@mixin container(){
  width: 1180px;
  margin: 0 auto;
  padding:0 15px;
}

@mixin fontfamily(){
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", "Microsoft JhengHei", Roboto, "Helvetica Neue", Arial, sans-serif
}
@mixin box-sizing(){
  box-sizing: border-box;
}
@mixin title-h($i,$size){
  @if($i == 1) {
    font-size: $fontSize * 2.5;
  }@else if($i == 2) {
    font-size: $fontSize * 2.0;
  }@else if($i == 3) {
    font-size: $fontSize * 1.75;
  }@else if($i == 4) {
    font-size: $fontSize * 1.5;
  }@else if($i == 5) {
    font-size: $fontSize * 1.25;
  }@else if($i == 6) {
    font-size: $fontSize;
  }@else if($i == 0 ){
    font-size: $fontSize * $size;
  }
}
@mixin title-x($size){
  font-size: $fontSize * $size;
}
@mixin img-fluid(){
  max-width: 100%;
  height: auto;
}
@mixin text-hide() {
  text-indent: 101%;
  overflow: hidden;
  white-space: nowrap;
}
@mixin d-flex(){
  display: flex;
}
@mixin justify-content-center(){
  justify-content: center;
}
@mixin justify-content-between(){
  justify-content: space-between;
}
@mixin align-items-center(){
  align-items: center;
}
@mixin text-border-none(){
  text-decoration: none;
}
@mixin courseList($htmlWidth,$gridNumber,$mr){
  display: inline-block;
  width: (($htmlWidth / $gridNumber)-$gridNumber)-$mr;
  margin-right: $mr;
  &:nth-child(#{$gridNumber}){
    margin-right: 0px;
  }
}
@mixin input-focus(){
  & input[type="text"]:focus,
  & input[type="tel"]:focus,
  & input[type="email"]:focus,
  & input[type="number"]:focus,
  & input[type="password"]:focus,
  & input[type="submit"]:focus, 
  & input[type="reset"]:focus,
  & input[type="search"]:focus{
      box-shadow: 0px 0px  10px $blue;
  }
}
