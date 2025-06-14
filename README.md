# 短剧api永久免费接口稳定性高，欢迎对接

## API接口文档





### 概述

> 本文档提供短剧搜索服务API的对接指南，包括API功能、请求参数、返回数据格式及示例。 本接口主要是用来存储夸克网盘资源，然后对接短剧机器人，来实现盈利。

### 功能描述：

> 短剧搜索服务API提供短剧名称的搜索功能，用户可通过API提交短剧名称关键字，获取相应的短剧信息列表。
>
> 短剧搜索服务API提供所有短剧列表查询功能
>
> 短剧搜索服务API提供今日短剧更新列表查询功能



### 全网夸克网盘短剧查询，每日更新：

> 接口地址： https://www.duanju.click/api/short/quark

> 请求参数说明：

| 名称  | 必填 | 类型   | 说明             | 请求示例                                                     |
| :---- | :--- | :----- | :--------------- | :----------------------------------------------------------- |
| text  | 是   | string | 搜索短剧名称     | [https://www.duanju.click/api/short/quark?text=好一个乖乖女](https://www.duanju.click/api/short/quark?text=%E5%A5%BD%E4%B8%80%E4%B8%AA%E4%B9%96%E4%B9%96%E5%A5%B3) |
| list  | 是   | string | 查询接口全部短剧 | [https://www.duanju.click/api/short/quark?list](https://www.duanju.click/api/short/quark?list) |
| today | 是   | string | 查询今日更新     | [https://www.duanju.click/api/short/quark?today](https://www.duanju.click/api/short/quark?today) |

> 返回参数说明：

| 名称 | 类型   | 说明     |
| :--- | :----- | :------- |
| name | string | 短剧名称 |
| link | string | 短剧链接 |
| time | string | 更新时间 |

> 返回示例

```json
{
  "code": 200,
  "msg": "搜索成功", //text时返回‘搜索成功’，list时返回‘列表获取成功’，today时返回‘今日更新’
  "data": [
    {
      "name": "29-好一个乖乖女（88集） 赵柯淳&余茵",
      "link": "https://pan.quark.cn/s/2a4dcdc77a1a",
      "time": "2025-02-04 01:08:10"
    }
  ]
}
```

------

### 全网百度网盘短剧查询，每日更新：

> 接口地址： https://www.duanju.click/api/short/baidu

> 请求参数说明：

| 名称  | 必填 | 类型   | 说明             | 请求示例                                                     |
| :---- | :--- | :----- | :--------------- | :----------------------------------------------------------- |
| today | 是   | string | 查询今日更新     | [https://www.duanju.click/api/short/baidu?today](https://www.duanju.click/api/short/baidu?today) |

> 返回参数说明：

| 名称 | 类型   | 说明     |
| :--- | :----- | :------- |
| name | string | 短剧名称 |
| link | string | 短剧链接 |
| time | string | 更新时间 |

> 返回示例

```json
{
  "code": 200,
  "msg": "今日更新短剧",
  "data": [
    {
      "name": "宁宴长欢（86集）权裴伦&彩彩云",
      "link": "https://pan.baidu.com/s/1PNzskabDxrI4Fq2LDDYg-w?pwd=8888",
      "time": "2025-06-14 00:30:28",
      "remarks": ""
    },
    {
      "name": "嗜她如命（77集）肖文宇",
      "link": "https://pan.baidu.com/s/1feEO_hB1k-4YLFawLqpylg?pwd=8888",
      "time": "2025-06-14 00:30:34",
      "remarks": ""
    }
}
```



------

声明: 如有问题请及时通过电子邮件(1371866419@qq.com)联系我。
