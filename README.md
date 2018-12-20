# Modal
依赖bootstrap的Modal控件，封装了一个包含confirm和alert两种类型的Modal控件，使用简单操作方便。


###使用说明

在页面声明控件占位代码

```html
<div id="qgy-alert" class="modal" data-width="500" style="display: none; width: 500px; padding-right: 17px; position: fixed; top: 10%; left: 38%; height: 100%;">
  <div>
    <div class="modal-content">
      <div class="modal-header">
        <button type="button" class="close" data-dismiss="modal"><span aria-hidden="true">×</span><span class="sr-only">Close</span></button>
        <h5 class="modal-title"><i class="fa fa-exclamation-circle"></i> [Title]</h5>
      </div>
      <div class="modal-body small">
        <p>[Message]</p>
      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-primary ok" data-dismiss="modal">OK</button>
        <button type="button" class="btn btn-default cancel" data-dismiss="modal">Cancel</button>
      </div>
    </div>
  </div>
</div>
```

然后在我们的js代码中调用

```js

confirm代码
Modal.confirm({ title: '我是标题', msg: '我是提示信息' }).on(function (e) {
  // TODO Something 
  // yes 
}, function (e) { 
  // no
});

alert代码
Modal.alert({ title: '我是标题', msg: '我是提示信息' }).on(function(){

});

```
