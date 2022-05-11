# RUBY MENU

RubyMenu là plugin về menu sử dụng thư viện jQuery.

Hỗ trợ 2 loại menu
+ Menu hanger
+ Menu drawer


## SETUP

Thiết lập trên html

``` html
<!-- Thiết lập class và options trên html -->
<nav class="rm01" data-menu='{
  "widthOffCanvas": [0, 767],
  "selectorToggle": null,
}'>
  <ul class="rm01menu">
    <li><a href="/link-1a">Link level 1 - a</a></li>
    <li>
      <a href="/link-1b">Link level 1 - b</a>
      <ul class="rm01menu">
        <li><a href="/link-2a">Link level 2 - a</a></li>
        <li><a href="/link-2b">Link level 2 - b</a></li>
      </ul>
    </li>
    <li><a href="/link-1c">Link level 1 - c</a></li>
  </ul>
</nav>
```


Menu-toggle sẽ tự động render trong RubyMenu.
Trường hợp custom menu-toggle, thiết lập selector để RubyMenu biết chọn đúng menu-toggle.

``` html
<nav class="rm01" data-menu='{
  "selectorToggle": ".menu-toggle",
}'>
  <a class="menu-toggle" href="#">
    <span class="menu-toggle-line"></span>
  </a>
  <ul>...</ul>
</nav>
```