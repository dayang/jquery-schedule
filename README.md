# jquery-schedule
A jQuery plugin  to create a courses schedule.(Mainly used for one of my class projects)


####usage####

`<table id="schedule" class="table table-bordered">
</table>`

You can use like this
`
$('#schedule').createSchedule(data,{
	classNum : 10,
	th : ['时间','星期一','星期二','星期三','星期四','星期五'],
});`

#####data####
`[{  
	courseInfo : [数据结构','王老师'],  
	sksj : '一1-2'  
},{
	courseInfo : [],
	sksj : ''
}]`

*data* is an array of courses  
*couseInfo* is a string array that contains the infomation about the course that you want to display.  
*sksj* is a string represents the course time with a format like '一1-2' and you must put a whitespace between two times like '一1-2 三3-4',the chinese words 一,二,三,四,五 represent the weekdays of a week and 1-2 means the course begin at the first class of the day and 2 means the second.  

#####options####
`{
	classNum : 13,
	th : ['时间','周一','周二','周三','周四','周五'],
	firstCol : ['1','2','3','4','5','6','7','8','9','10','11','12','13']
};`

*classNum* is the class number of one day.  
*th* is the info that display in the table head  
*firstCol* is the info you want to display in the first column cells which means the classes' serial num.

![](https://github.com/dayang/jquery-schedule/edit/master/sample.png)
