

.. _Gantt-Chart_Gantt_Chart_Properties_-_Bars:


Bars
====

**Description** 

The Bars tab of the Gantt Chart properties offers properties to tune where and how the bars of in the chart are displayed.







**Multiply default bar height with factor** 

By default, the height of a bar in the chart is determined by the current font metrics: the height of the font fits in the bar height. 

Here you can specify a factor with which this default height should be increased. Any value in the range [1.0, 3.0] is valid.

If you specify a scalar parameter and this parameter has a value outside this range, then the nearest value in the range is used instead.



**Spacing between rows as fraction of default bar height** 

By default, the spacing between the bars in subsequent rows is a small number of pixels. With this option you can overrule this default, and specify this spacing as a fraction of the default bar height (i.e. the height prior to applying the multiplication factor described above). Any value in the range [0.0, 3.0] is valid.

If you specify a scalar parameter and this parameter has a value outside this range, then the nearest value in the range is used instead.

Note that an explicit value of '0' is different than leaving the entry empty: '0' will result in no spacing at all, while empty falls back to the default spacing.



**Show overlapping bar with a different vertical offset** 

If the Gantt chart contains overlapping bars on the same row (like the tasks for either machine 2 or machine 4 in the picture above), you can use this option to visualize these bars more clearly.

In the picture above, without this option checked, the two tasks for machine 2 and machine 4 would be displayed on top of each other with only a different horizontal position. When checked,

a bar that overlaps with one or more previous bars will be drawn a fraction lower. In the picture above 'task 4' overlaps with 'task2' in the same row, and thus is displayed a fraction below its normal position.



**Offset as fraction of bar height** 

This option determines how much lower an overlapping bar is displayed. By default this is 0.5 (which is the value used in the picture above), but you can specify any value in the range [0.0, 2.0]. You can specify this value via a numeric parameter, which may be indexed of the indices that are used as row domain. For example, in the example of the picture above, you can specify a parameter X indexed over machines where X('machine 2') = 0.5 and X('machine 4') = 0.0 (the latter will result in 'task 5' being displayed at same position as 'task 2').



**All rows have same height** 

If this option is checked, all rows will get the same height which is determined by the maximum height of all rows. In the picture above, this option is not checked, resulting in the situation that the rows for 'machine 1' and 'machine 3' do not have the same height as the rows for 'machine 2' and 'machine 4'.



**Draw border around bars** 

By default, each bar is drawn with a small border line with the same color as the text. If you uncheck this option, this border is omitted. 



