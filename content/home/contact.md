+++
# Contact widget.
widget = "contact"
active = true
date = 2016-04-20T00:00:00

title = "和我联系"
subtitle = ""

# Order that this section will appear in.
weight = 70

# Automatically link email and phone?
autolink = true

# Email form provider
#   0: Disable email form
#   1: Netlify (requires that the site is hosted by Netlify)
#   2: formspree.io
email_form = 0
+++

<!--  -->
<script type="text/javascript" src="http://api.map.baidu.com/api?v=2.0&ak=GEbowcucx4hvPsG8GwvzCBUIDQzmMmOH"></script>
<div id="allmap">
<script type="text/javascript">
	// 百度地图API功能
	var map = new BMap.Map("allmap");
	var point = new BMap.Point(117.9431460000, 28.4575310000);
	var marker = new BMap.Marker(point);  // 创建标注
	map.addOverlay(marker);              // 将标注添加到地图中
	map.centerAndZoom(point, 15);
	var opts = {
	  width : 50,     // 信息窗口宽度
	  height: 50,     // 信息窗口高度
	}
	var infoWindow = new BMap.InfoWindow("地址：上饶市信州区广信大厦A座3楼", opts);  // 创建信息窗口对象 
	marker.addEventListener("click", function(){          
		map.openInfoWindow(infoWindow,point); //开启信息窗口
	});
</script>


</div> 
 <!-- baiduMap -->

<style type="text/css">
    #allmap {width: 100%;height: 100%;overflow: hidden;margin:0px 20px 30px 0px;font-family:"微软雅黑";}
</style>
