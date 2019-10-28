# LCalendar移动端时间插件
#### 页面中引入input标签，通过自定义属性data-lcalendar控制最小日期和最大日期，id名称与调用时一致
   <input id="demo1" type="text" readonly="" placeholder="日期选择" data-lcalendar="2019-10-28,2019-10-28" />
##### 引入LCalendar.css和LCalendar.js
###### 初始化插件
   var calendar = new LCalendar();
       calendar.init({
          'trigger': '#demo1', //标签id
          'type': 'date', // 调出日期选择date;  调出日期时间选择datetime;  调出时间选择time;  调出年月选择ym。
          'minDate': '1970-1-1', //最小日期 注意：该值会覆盖标签内定义的日期范围
          'maxDate': '2050-1-1' //最大日期  注意：该值会覆盖标签内定义的日期范围
   });
