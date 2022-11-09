## Search
<hr>
<script>
    function goBing(){
        $('#form1').attr('action',"https://bing.com/search");
        $('#form1').submit();
    }
    function goBaidu(){
        $('#wd').val($('#q').val());
        $('#form1').attr('action',"https://www.baidu.com/s");
    }
    function goGoogle(){
        $('#form1').attr('action',"https://www.google.com/search");
        $('#form1').submit();
    }
</script>

<div>

<form action="https://www.baidu.com/s" id="form1" target="_blank"  >
    <div class="form-group">
    <input type="hidden" name="wd" id="wd" >
        <input type="text"  class="form-control-lg form-control" name="q" id="q" placeholder="Search here" > <br/>
       <input type="submit" class="btn btn-default" value="Baidu" onclick="goBaidu()">
        <input type="submit" class="btn btn-default" value="Bing" onclick="goBing();return false;">
        <input type="submit" class="btn btn-default" value="Google" onclick="goGoogle();return false;">
    </div>
</form>
</div>

<div class="my-definition">a</div>
## Links
<hr>
[Mac](./mac.md)
[Windows](./windows.md)

## Online tools
[Tools](https://c.runoob.com/)
[Tools](https://c.runoob.com/)
## Softwares



