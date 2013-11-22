---
layout: post
title: Bootstrap-paginator
subtitle: A bootstrap style paginator, implemented by javascript.
---


### HTML 代码：

```html
<!-- html element for pagination -->
<ul class="pagination"></ul>

<!-- load paginator.js -->
<script src="./assets/bootstrap-paginator.js"></script>

<script>
    //callback when page_id clicked
    function func1(page_id) {
        alert( 'To page: ' + page_id );
    }
  
    $(function(){
        //init paginator
        $('.pagination').paginator({current_page: 1, page_count: 15, button_number:5, pager_click: func1 });
        
        //optional: enable paginator tooltips
        $('[data-toggle="tooltip"]').tooltip();
    });
</script>
```

### 效果：

<ul class="pagination"></ul>



### 参数：

<dl class="dl-horizontal">
    <dt>current_page</dt>
    <dd>当前所在的页码</dd>
    <dt>page_count</dt>
    <dd>总页数</dd>
    <dt>button_number</dt>
    <dd>需要显示的页码数目</dd>
    <dt>pager_click</dt>
    <dd>回调函数</dd>
</dl>

<script>
  function func1(page_id) {
    alert( 'To page: ' + page_id );
  }
  
  $(function(){
    $('.pagination').paginator({current_page: 1, page_count: 15, button_number:5, pager_click: func1 });
    
    $('[data-toggle="tooltip"]').tooltip();
  });
</script>
