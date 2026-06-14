合家云项目接口文档
社区资产模块
小区管理
获取小区信息
接口地址: http://localhost:8888/hejiayun/community/list?pageNum=1&pageSize=10&communityName=宏福苑&communityCode=COMMUNITY_1675945745985

请求方式: GET

接口描述: 获取小区信息

请求参数说明

参数名称	参数说明
pageNum	当前页
pageSize	每页显示条数
communityCode	小区编码
communityName	小区名称
响应结果说明

参数名称	参数说明
code	状态码
msg	查询成功/查询失败
total	总条数
rows	小区数据信息集合
响应结果示例:

{
"total": 1,
"rows": [{
"searchValue": null,
"createBy": "admin",
"createTime": "2023-02-09 20:29:06",
"updateBy": "admin",
"updateTime": "2023-02-09 20:29:06",
"remark": null,
"params": {

		},
		"communityId": "1623660256618201090",
		"communityName": "宏福苑小区",
		"communityCode": "COMMUNITY_1675945745985",
		"communityProvenceCode": "1",
		"communityProvenceName": "北京市",
		"communityCityCode": "10",
		"communityCityName": "北京市",
		"communityTownCode": "1010",
		"communityTownName": "昌平区",
		"communityDetailedAddress": "北京市昌平区宏福苑",
		"communityLongitude": null,
		"communityLatitude": null,
		"deptId": 103,
		"communitySort": null
	}],
	"code": 200,
	"msg": "查询成功"
}
新增小区
接口地址: http://localhost:8888/hejiayun/community

请求方式: POST

接口描述: 新增小区信息

请求参数说明

参数名称	参数说明
communityId	小区id
communityName	小区名称
communityCode	小区编码
communityProvenceCode	省区划码
communityCityCode	市区划码
communityTownCode	区县区划码
communityDetailedAddress	详细地址
longitude	经度
latitude	纬度
deptId	物业id
remark	备注
selected	省市区划代码
请求参数示例

{
"communityId": null,
"communityName": "清水园小区",
"communityCode": null,
"communityProvenceCode": 1,
"communityCityCode": 10,
"communityTownCode": 1010,
"longitude": null,
"latitude": null,
"deptId": null,
"sort": null,
"createBy": null,
"createTime": null,
"updateBy": null,
"updateTime": null,
"selected": [1,
10,
1010],
"remark": null,
"communityDetailedAddress": "北京市昌平区陈家营"
}
响应结果示例

{
"code": "200",
"message": "操作成功",
"data": 1
}
修改小区
接口1 地址: http://localhost:9999/hejiayun/community/1623660256618201090

请求方式: GET

接口描述: 根据小区id，回显数据

请求参数说明

参数名称	参数说明
communityId	状态码
响应结果示例

{
"code": "200",
"message": "操作成功",
"data": {
"searchValue": null,
"createBy": "admin",
"createTime": "2023-02-09 12:29:06",
"updateBy": "admin",
"updateTime": "2023-02-09 12:29:06",
"remark": null,
"params": {},
"communityId": "1623660256618201090",
"communityName": "宏福苑小区",
"communityCode": "COMMUNITY_1675945745985",
"communityProvenceCode": "1",
"communityCityCode": "10",
"communityTownCode": "1010",
"communityDetailedAddress": "北京市昌平区宏福苑",
"communityLongitude": null,
"communityLatitude": null,
"deptId": "103",
"communitySort": null
}
}
接口2 地址: http://localhost/dev-api/system/area/tree

请求方式: GET

接口描述: 获取省市区三级联动信息

响应结果示例

{
"code": 200,
"msg": "操作成功"，
"data": "区域信息省略。。。,
}
接口3 地址: http://localhost:9999/hejiayun/community

请求方式: PUT

接口描述: 修改小区信息

请求参数示例

{
"searchValue": null,
"createBy": "admin",
"createTime": "",
"updateBy": "admin",
"updateTime": "",
"remark": null,
"params": {

	},
	"communityId": "1631303717525716993",
	"communityName": "首付未来城小区",
	"communityCode": "COMMUNITY_1676015682766",
	"communityProvenceCode": 1,
	"communityCityCode": 10,
	"communityTownCode": 1010,
	"communityDetailedAddress": "北京市昌平区陈家营西路",
	"communityLongitude": null,
	"communityLatitude": null,
	"deptId": "103",
	"communitySort": null,
	"selected": [1,
	10,
	1010]
}
响应结果示例

{
"code": "200",
"message": "操作成功",
"data": 1
}
删除小区信息
接口地址:

http://localhost:9999/hejiayun/community/1623953592746811393
http://localhost:9999/hejiayun/community/1631558965133582338,1631559055512444929
请求方式: DELETE

接口描述: 删除小区信息

请求参数说明

参数名称	参数说明
communityId	状态码
响应结果示例

{
"code": "200",
"message": "操作成功",
"data": 2
}
更换小区物业
接口1地址: http://localhost/dev-api/system/dept/list

请求方式: GET

接口描述: 获取物业公司信息

响应结果说明

{
"code": 200,
"success": true,
"msg": "操作成功"，
"data": "sys_dept部门表数据，省略。。。"
}
获取小区下拉列表
接口地址: http://localhost/dev-api/community/community/queryPullDown

请求方式: GET

接口描述: 获取首页右上角的小区下拉列表

请求参数说明

参数名称	参数说明
communityId	状态码
响应结果示例

{
"code": 200,
"success": true,
"data": [{
"searchValue": null,
"createBy": "admin",
"createTime": "2023-02-09 20:29:06",
"updateBy": "admin",
"updateTime": "2023-02-09 20:29:06",
"remark": null,
"params": {

		},
		"communityId": "1623660256618201090",
		"communityName": "宏福苑小区",
		"communityCode": "COMMUNITY_1675945745985",
		"communityProvenceCode": "1",
		"communityProvenceName": "北京市",
		"communityCityCode": "10",
		"communityCityName": "北京市",
		"communityTownCode": "1010",
		"communityTownName": "昌平区",
		"communityDetailedAddress": "北京市昌平区宏福苑",
		"communityLongitude": null,
		"communityLatitude": null,
		"deptId": 103,
		"communitySort": null
	}],
	"msg": "操作成功"
}
小区数据导出功能
**接口地址：**http://localhost/dev-api/community/community/export?pageNum=1&pageSize=10

请求方式: GET

接口描述: 导出小区数据

楼栋管理
获取楼栋信息接口
接口地址: http://localhost/dev-api/system/building/list?pageNum=1&pageSize=10&buildingName=1&buildingCode=1

接口地址: http://localhost/dev-api/system/building/list?pageNum=1&pageSize=10

请求方式: GET

接口描述: 获取楼栋信息

请求信息说明

参数名称	参数说明
pageNum	当前页
pageSize	每页显示条数
buildingName	楼栋名称
buildingCode	楼栋编码
响应结果说明

参数名称	参数说明
code	状态码
msg	查询成功/查询失败
total	总条数
rows	楼栋数据信息集合
响应结果示例:

{
"total": 2,
"rows": [{
"searchValue": null,
"createBy": "admin",
"createTime": "2023-02-09 20:26:02",
"updateBy": "admin",
"updateTime": "2023-02-09 20:26:44",
"remark": null,
"params": {

		},
		"buildingId": "1623659483150794753",
		"buildingName": "南一区1号楼",
		"buildingCode": "BUILDING_1675945561579",
		"buildingAcreage": 120.0000000000,
		"communityId": 1623660256618201090,
		"communityName": "宏福苑小区",
		"list": []
	},
	{
		"searchValue": null,
		"createBy": "admin",
		"createTime": "2023-02-09 20:28:27",
		"updateBy": "admin",
		"updateTime": "2023-02-09 20:28:27",
		"remark": null,
		"params": {
			
		},
		"buildingId": "1623660091043856386",
		"buildingName": "南一区2号楼",
		"buildingCode": "BUILDING_1675945706515",
		"buildingAcreage": 99.0000000000,
		"communityId": 1623660256618201090,
		"communityName": "宏福苑小区",
		"list": []
	}],
	"code": 200,
	"msg": "查询成功"
}
获取楼栋下拉列表
接口地址: http://localhost/dev-api/system/building/queryPullDown

请求方式: GET

接口描述: 获取楼栋下拉列表

请求参数说明

参数名称	参数说明
propertyId（CommunityId）	小区id
响应结果示例

{
"code": 200,
"success": true,
"data": [{
"searchValue": null,
"createBy": "admin",
"createTime": "2023-02-09 20:26:02",
"updateBy": "admin",
"updateTime": "2023-02-09 20:26:44",
"remark": null,
"params": {

		},
		"buildingId": "1623659483150794753",
		"buildingName": "南一区1号楼",
		"buildingCode": "BUILDING_1675945561579",
		"buildingAcreage": 120.0000000000,
		"communityId": 1623660256618201090,
		"communityName": "宏福苑小区",
		"list": []
	},
	{
		"searchValue": null,
		"createBy": "admin",
		"createTime": "2023-02-09 20:28:27",
		"updateBy": "admin",
		"updateTime": "2023-02-09 20:28:27",
		"remark": null,
		"params": {
			
		},
		"buildingId": "1623660091043856386",
		"buildingName": "南一区2号楼",
		"buildingCode": "BUILDING_1675945706515",
		"buildingAcreage": 99.0000000000,
		"communityId": 1623660256618201090,
		"communityName": "宏福苑小区",
		"list": []
	}],
	"msg": "操作成功"
}
