# reveal-Modal
this is reveal-modal
#模态窗口
```
可以兼容到IE6，其中包括了多种类型，比如 两个嵌套 、单个、一个按钮和两个按钮、提示框、警示框
```
#####参考demo地址：[http://192.168.14.97:8080/acc/plugin/reveal-Modal/index.html](http://192.168.14.97:8080/acc/plugin/reveal-Modal/index.html)
##样例
####1、使用步骤
####（1）导入样式文件
```
<link href="style/popup.css" rel="stylesheet" type="text/css" />
```
####（2）导入外部JS文件
```
<script src="javascript/jquery-1.9.1.min.js"></script>
<script src="javascript/reveal-model.js"></script>
```
####（3）页面使用代码
```
<a href="#" reveal-model-id="showbox1" class="click-block">点击按钮弹出模态窗口(底部2个按钮)</a>

<div class="box-content large noClick" id="showbox1" style="display: block; left: 248.5px; top: -111.55px;">
    <h2>请选1择<a href="#" class="close-reveal-modal">×</a></h2>
    <div class="mainlist">
        <form data-abide="">
            <div class="modal_wrap">
              内容
            </div>
          </form>
        <div class="btn-grop clearfix"> <a class="reveal-button right sure">提交</a>
        <a class="reveal-button close-reveal-modal right margin-r" aria-label="Close">取消</a>
        </div>
    </div>
</div>
```
####（4）方法和API
 #####（1）方法
```
//模态窗口配置
<script type="text/javascript">
    $(document).ready(function(){
        $('#showbox1').mask().noClick();//配置对象#showbox1遮罩层不能点击
    });
</script>

//提示框和警示框
$('.success-click').click(function(){
    loading("success","发布成功");
});
$('.alert-click').click(function(){
    loading("alert","发布的内容不能为空");
});
```
#####API
```
    无
```
#参数说明：
```
loading("success","发布成功");//提示框路口
loading("alert","发布的内容不能为空");//警示框路口
```
#更新日志
```
无
```
