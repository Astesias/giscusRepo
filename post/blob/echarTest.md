# ECharts 图表测试

## 折线图

```echarts
{
  "xAxis": {
    "type": "category",
    "data": ["周一", "周二", "周三", "周四", "周五", "周六", "周日"]
  },
  "yAxis": {
    "type": "value"
  },
  "series": [
    {
      "data": [150, 230, 224, 218, 135, 147, 260],
      "type": "line",
      "smooth": true
    }
  ]
}
```

## 柱状图

```echarts
{
  "xAxis": {
    "type": "category",
    "data": ["项目A", "项目B", "项目C", "项目D", "项目E"]
  },
  "yAxis": {
    "type": "value"
  },
  "series": [
    {
      "data": [120, 200, 150, 80, 70],
      "type": "bar",
      "itemStyle": {
        "color": "#5470C6"
      }
    }
  ]
}
```

## 饼图

```echarts
{
  "series": [
    {
      "type": "pie",
      "data": [
        { "value": 1048, "name": "搜索引擎" },
        { "value": 735, "name": "直接访问" },
        { "value": 580, "name": "邮件营销" },
        { "value": 484, "name": "联盟广告" },
        { "value": 300, "name": "视频广告" }
      ],
      "radius": ["40%", "70%"]
    }
  ]
}
```

## 散点图

```echarts
{
  "xAxis": {
    "type": "value"
  },
  "yAxis": {
    "type": "value"
  },
  "series": [
    {
      "type": "scatter",
      "data": [
        [10, 5], [20, 15], [30, 25], [40, 35],
        [50, 45], [60, 55], [70, 65], [80, 75],
        [15, 10], [25, 20], [35, 30], [45, 40]
      ]
    }
  ]
}
```
