bootstrap-paginator
===================

A bootstrap style paginator, implemented by javascript.

**live demo**: 
http://harttle.github.io/bootstrap-paginator/


### Requirements

* bootstrap 3
* jquery


### Usage

```html
<!-- load paginator.js -->
<script src="./assets/bootstrap-paginator.js"></script>

<script>
    //callback when page_id clicked
    function callback(page_id) {
        alert( 'To page: ' + page_id );
    }
  
    $(function(){
        //init paginator
        $('.pagination').paginator({current_page: 1, page_count: 15, button_number:5, pager_click: callback });
        
        //optional: enable paginator tooltips
        $('[data-toggle="tooltip"]').tooltip();
    });
</script>
```


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
