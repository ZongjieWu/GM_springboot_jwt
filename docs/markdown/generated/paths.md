
<a name="paths"></a>
## 资源

<a name="a0f4ddd0959e74f4ba2f0428d3569a3c"></a>
### 1.平台管理员
登入等接口


<a name="addusingpost_1"></a>
#### 登入
```
POST /admin/login
```


##### 说明
登入


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**token**  <br>*可选*|用户的认证标识|string|
|**Query**|**phone**  <br>*必填*|电话号码|string|
|**Query**|**pwd**  <br>*必填*|密码|string|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[Result«SaasUserBaseInfoResponseVo»](#6808aa882c818db47bc2ed70acfe3dbd)|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `\*/*`


##### HTTP请求示例

###### 请求 path
```
/admin/login?phone=string&pwd=string
```


###### 请求 header
```json
"string"
```


##### HTTP响应示例

###### 响应 200
```json
{
  "code" : 0,
  "count" : 0,
  "data" : {
    "addTime" : "string",
    "addr" : "string",
    "email" : "string",
    "headImg" : "string",
    "id" : 0,
    "idCard" : "string",
    "modifyTime" : "string",
    "name" : "string",
    "phone" : "string",
    "saasUserPermissionList" : [ {
      "addTime" : "string",
      "descript" : "string",
      "iconPath" : "string",
      "id" : 0,
      "modifyTime" : "string",
      "name" : "string",
      "parentId" : 0,
      "requestPath" : "string",
      "saasUserPermissionList" : [ {
        "addTime" : "string",
        "descript" : "string",
        "iconPath" : "string",
        "id" : 0,
        "modifyTime" : "string",
        "name" : "string",
        "parentId" : 0,
        "requestPath" : "string",
        "saasUserPermissionList" : [ "..." ],
        "sort" : 0
      } ],
      "sort" : 0
    } ],
    "saasUserRoleId" : 0,
    "saasUserRoleName" : "string",
    "token" : "string"
  },
  "msg" : "string"
}
```


<a name="ba9d2cb9f35a883b1436f7119b27ee96"></a>
### 2.平台管理员
添加、修改、删除、查询等接口


<a name="addusingpost"></a>
#### 管理员添加
```
POST /saasUser/add
```


##### 说明
管理员添加


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**token**  <br>*可选*|用户的认证标识|string|
|**Query**|**addTime**  <br>*可选*||string (date-time)|
|**Query**|**addr**  <br>*可选*||string|
|**Query**|**email**  <br>*可选*||string|
|**Query**|**headImg**  <br>*可选*||string|
|**Query**|**id**  <br>*可选*||integer (int64)|
|**Query**|**idCard**  <br>*可选*||string|
|**Query**|**modifyTime**  <br>*可选*||string (date-time)|
|**Query**|**name**  <br>*可选*||string|
|**Query**|**phone**  <br>*可选*||string|
|**Query**|**pwd**  <br>*可选*||string|
|**Query**|**saasUserPermissionList[0].addTime**  <br>*可选*||string (date-time)|
|**Query**|**saasUserPermissionList[0].descript**  <br>*可选*||string|
|**Query**|**saasUserPermissionList[0].iconPath**  <br>*可选*||string|
|**Query**|**saasUserPermissionList[0].id**  <br>*可选*||integer (int64)|
|**Query**|**saasUserPermissionList[0].modifyTime**  <br>*可选*||string (date-time)|
|**Query**|**saasUserPermissionList[0].name**  <br>*可选*||string|
|**Query**|**saasUserPermissionList[0].parentId**  <br>*可选*||integer (int64)|
|**Query**|**saasUserPermissionList[0].requestPath**  <br>*可选*||string|
|**Query**|**saasUserPermissionList[0].sort**  <br>*可选*||integer (int32)|
|**Query**|**saasUserRoleId**  <br>*可选*||integer (int64)|
|**Query**|**saasUserRoleName**  <br>*可选*||string|
|**Query**|**status**  <br>*可选*||integer (int32)|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[Result](#result)|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `\*/*`


##### HTTP请求示例

###### 请求 path
```
/saasUser/add
```


###### 请求 header
```json
"string"
```


##### HTTP响应示例

###### 响应 200
```json
{
  "code" : 0,
  "count" : 0,
  "data" : "object",
  "msg" : "string"
}
```


<a name="deleteusingpost"></a>
#### 管理员删除
```
POST /saasUser/delete
```


##### 说明
管理员删除


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**token**  <br>*可选*|用户的认证标识|string|
|**Query**|**id**  <br>*必填*|管理员表id|integer (int32)|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[Result](#result)|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `\*/*`


##### HTTP请求示例

###### 请求 path
```
/saasUser/delete?id=0
```


###### 请求 header
```json
"string"
```


##### HTTP响应示例

###### 响应 200
```json
{
  "code" : 0,
  "count" : 0,
  "data" : "object",
  "msg" : "string"
}
```


<a name="detailusingget"></a>
#### detail
```
GET /saasUser/detail
```


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**token**  <br>*可选*|用户的认证标识|string|
|**Query**|**id**  <br>*可选*|id|integer (int64)|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[SaasUser](#saasuser)|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 生成

* `\*/*`


##### HTTP请求示例

###### 请求 path
```
/saasUser/detail
```


###### 请求 header
```json
"string"
```


##### HTTP响应示例

###### 响应 200
```json
{
  "addTime" : "string",
  "addr" : "string",
  "email" : "string",
  "headImg" : "string",
  "id" : 0,
  "idCard" : "string",
  "modifyTime" : "string",
  "name" : "string",
  "phone" : "string",
  "pwd" : "string",
  "saasUserPermissionList" : [ {
    "addTime" : "string",
    "descript" : "string",
    "iconPath" : "string",
    "id" : 0,
    "modifyTime" : "string",
    "name" : "string",
    "parentId" : 0,
    "requestPath" : "string",
    "saasUserPermissionList" : [ {
      "addTime" : "string",
      "descript" : "string",
      "iconPath" : "string",
      "id" : 0,
      "modifyTime" : "string",
      "name" : "string",
      "parentId" : 0,
      "requestPath" : "string",
      "saasUserPermissionList" : [ "..." ],
      "sort" : 0
    } ],
    "sort" : 0
  } ],
  "saasUserRoleId" : 0,
  "saasUserRoleName" : "string",
  "status" : 0
}
```


<a name="pagingusingpost"></a>
#### 分页查询管理员
```
POST /saasUser/paging
```


##### 说明
分页查询管理员


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**token**  <br>*可选*|用户的认证标识|string|
|**Query**|**keywords**  <br>*可选*|关键词|string|
|**Query**|**limit**  <br>*必填*|每页的条数|integer (int32)|
|**Query**|**page**  <br>*必填*|当前页|integer (int32)|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[Result«List«SaasUserBaseInfoResponseVo»»](#d81602790788bd27cb5a976bd576dfb6)|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `\*/*`


##### HTTP请求示例

###### 请求 path
```
/saasUser/paging?limit=0&page=0
```


###### 请求 header
```json
"string"
```


##### HTTP响应示例

###### 响应 200
```json
{
  "code" : 0,
  "count" : 0,
  "data" : [ {
    "addTime" : "string",
    "addr" : "string",
    "email" : "string",
    "headImg" : "string",
    "id" : 0,
    "idCard" : "string",
    "modifyTime" : "string",
    "name" : "string",
    "phone" : "string",
    "saasUserPermissionList" : [ {
      "addTime" : "string",
      "descript" : "string",
      "iconPath" : "string",
      "id" : 0,
      "modifyTime" : "string",
      "name" : "string",
      "parentId" : 0,
      "requestPath" : "string",
      "saasUserPermissionList" : [ {
        "addTime" : "string",
        "descript" : "string",
        "iconPath" : "string",
        "id" : 0,
        "modifyTime" : "string",
        "name" : "string",
        "parentId" : 0,
        "requestPath" : "string",
        "saasUserPermissionList" : [ "..." ],
        "sort" : 0
      } ],
      "sort" : 0
    } ],
    "saasUserRoleId" : 0,
    "saasUserRoleName" : "string",
    "token" : "string"
  } ],
  "msg" : "string"
}
```


<a name="updateusingpost"></a>
#### 管理员修改
```
POST /saasUser/update
```


##### 说明
管理员修改


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**token**  <br>*可选*|用户的认证标识|string|
|**Query**|**addr**  <br>*可选*|联系地址|string|
|**Query**|**email**  <br>*可选*|邮箱|string|
|**Query**|**headImg**  <br>*可选*|头像|string|
|**Query**|**id**  <br>*必填*|平台管理员的表id|integer (int64)|
|**Query**|**idCard**  <br>*可选*|身份证|string|
|**Query**|**name**  <br>*可选*|名称|string|
|**Query**|**phone**  <br>*必填*|电话|string|
|**Query**|**pwd**  <br>*必填*|密码|string|
|**Query**|**saasUserRoleId**  <br>*必填*|角色id|integer (int64)|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[Result](#result)|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `\*/*`


##### HTTP请求示例

###### 请求 path
```
/saasUser/update?id=0&phone=string&pwd=string&saasUserRoleId=0
```


###### 请求 header
```json
"string"
```


##### HTTP响应示例

###### 响应 200
```json
{
  "code" : 0,
  "count" : 0,
  "data" : "object",
  "msg" : "string"
}
```


<a name="dccfb2cb91afea230d50c03e8f66b98f"></a>
### 3.平台管理员角色
添加、修改、删除、查询等接口


<a name="addusingpost_4"></a>
#### 平台管理员角色添加
```
POST /saasUserRoleType/add
```


##### 说明
平台管理员角色添加


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**token**  <br>*可选*|用户的认证标识|string|
|**Query**|**descript**  <br>*可选*|描述|string|
|**Query**|**name**  <br>*必填*|名称|string|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[Result](#result)|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `\*/*`


##### HTTP请求示例

###### 请求 path
```
/saasUserRoleType/add?name=string
```


###### 请求 header
```json
"string"
```


##### HTTP响应示例

###### 响应 200
```json
{
  "code" : 0,
  "count" : 0,
  "data" : "object",
  "msg" : "string"
}
```


<a name="deleteusingpost_3"></a>
#### 平台管理员角色的删除
```
POST /saasUserRoleType/delete
```


##### 说明
平台管理员角色的删除


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**token**  <br>*可选*|用户的认证标识|string|
|**Query**|**id**  <br>*必填*|平台管理员角色表id|integer (int32)|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[Result](#result)|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `\*/*`


##### HTTP请求示例

###### 请求 path
```
/saasUserRoleType/delete?id=0
```


###### 请求 header
```json
"string"
```


##### HTTP响应示例

###### 响应 200
```json
{
  "code" : 0,
  "count" : 0,
  "data" : "object",
  "msg" : "string"
}
```


<a name="listusingget"></a>
#### 获取角色列表
```
GET /saasUserRoleType/list
```


##### 说明
获取角色列表


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**token**  <br>*可选*|用户的认证标识|string|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[Result«List«SaasUserRoleType»»](#4ac26851a62c3f174fa06f2974ee94d6)|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 生成

* `\*/*`


##### HTTP请求示例

###### 请求 path
```
/saasUserRoleType/list
```


###### 请求 header
```json
"string"
```


##### HTTP响应示例

###### 响应 200
```json
{
  "code" : 0,
  "count" : 0,
  "data" : [ {
    "addTime" : "string",
    "descript" : "string",
    "id" : 0,
    "modifyTime" : "string",
    "name" : "string"
  } ],
  "msg" : "string"
}
```


<a name="updateusingpost_3"></a>
#### 平台管理员角色修改
```
POST /saasUserRoleType/update
```


##### 说明
平台管理员角色修改


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**token**  <br>*可选*|用户的认证标识|string|
|**Query**|**descript**  <br>*可选*|描述|string|
|**Query**|**id**  <br>*必填*|角色表id|integer (int64)|
|**Query**|**name**  <br>*必填*|名称|string|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[Result](#result)|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `\*/*`


##### HTTP请求示例

###### 请求 path
```
/saasUserRoleType/update?id=0&name=string
```


###### 请求 header
```json
"string"
```


##### HTTP响应示例

###### 响应 200
```json
{
  "code" : 0,
  "count" : 0,
  "data" : "object",
  "msg" : "string"
}
```


<a name="updatepermissionusingpost"></a>
#### 平台管理员角色权限的修改
```
POST /saasUserRoleType/updatePermission
```


##### 说明
平台管理员角色权限的修改


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**token**  <br>*可选*|用户的认证标识|string|
|**Query**|**authids**  <br>*必填*|权限id字符串,用逗号(,)隔开|string|
|**Query**|**rid**  <br>*必填*|角色id|integer (int32)|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[Result](#result)|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `\*/*`


##### HTTP请求示例

###### 请求 path
```
/saasUserRoleType/updatePermission?authids=string&rid=0
```


###### 请求 header
```json
"string"
```


##### HTTP响应示例

###### 响应 200
```json
{
  "code" : 0,
  "count" : 0,
  "data" : "object",
  "msg" : "string"
}
```


<a name="a00d1017f4f5439577f5ebbcc4590cd6"></a>
### 4.平台角色权限控制器
登入等接口


<a name="addusingpost_3"></a>
#### add
```
POST /saasUserRolePermission/add
```


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**token**  <br>*可选*|用户的认证标识|string|
|**Query**|**addTime**  <br>*可选*||string (date-time)|
|**Query**|**id**  <br>*可选*||integer (int64)|
|**Query**|**modifyTime**  <br>*可选*||string (date-time)|
|**Query**|**saasUserPermissionId**  <br>*可选*||integer (int64)|
|**Query**|**saasUserRoleId**  <br>*可选*||integer (int64)|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[Result](#result)|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `\*/*`


##### HTTP请求示例

###### 请求 path
```
/saasUserRolePermission/add
```


###### 请求 header
```json
"string"
```


##### HTTP响应示例

###### 响应 200
```json
{
  "code" : 0,
  "count" : 0,
  "data" : "object",
  "msg" : "string"
}
```


<a name="deleteusingpost_2"></a>
#### delete
```
POST /saasUserRolePermission/delete
```


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**token**  <br>*可选*|用户的认证标识|string|
|**Query**|**id**  <br>*必填*|id|integer (int64)|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[Result](#result)|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `\*/*`


##### HTTP请求示例

###### 请求 path
```
/saasUserRolePermission/delete?id=0
```


###### 请求 header
```json
"string"
```


##### HTTP响应示例

###### 响应 200
```json
{
  "code" : 0,
  "count" : 0,
  "data" : "object",
  "msg" : "string"
}
```


<a name="detailusingget_1"></a>
#### detail
```
GET /saasUserRolePermission/detail
```


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**token**  <br>*可选*|用户的认证标识|string|
|**Query**|**id**  <br>*必填*|id|integer (int64)|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[Result«SaasUserRolePermission»](#0da2f56c139f0adac96edef56e911548)|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 生成

* `\*/*`


##### HTTP请求示例

###### 请求 path
```
/saasUserRolePermission/detail?id=0
```


###### 请求 header
```json
"string"
```


##### HTTP响应示例

###### 响应 200
```json
{
  "code" : 0,
  "count" : 0,
  "data" : {
    "addTime" : "string",
    "id" : 0,
    "modifyTime" : "string",
    "saasUserPermissionId" : 0,
    "saasUserRoleId" : 0
  },
  "msg" : "string"
}
```


<a name="updateusingpost_2"></a>
#### update
```
POST /saasUserRolePermission/update
```


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**token**  <br>*可选*|用户的认证标识|string|
|**Query**|**addTime**  <br>*可选*||string (date-time)|
|**Query**|**id**  <br>*可选*||integer (int64)|
|**Query**|**modifyTime**  <br>*可选*||string (date-time)|
|**Query**|**saasUserPermissionId**  <br>*可选*||integer (int64)|
|**Query**|**saasUserRoleId**  <br>*可选*||integer (int64)|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[Result](#result)|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `\*/*`


##### HTTP请求示例

###### 请求 path
```
/saasUserRolePermission/update
```


###### 请求 header
```json
"string"
```


##### HTTP响应示例

###### 响应 200
```json
{
  "code" : 0,
  "count" : 0,
  "data" : "object",
  "msg" : "string"
}
```


<a name="c1bdd170b943b0426ff2c8f05fccc26b"></a>
### 5.平台管理员权限
添加、修改、删除、查询等接口


<a name="addusingpost_2"></a>
#### 添加权限
```
POST /saasUserPermissionList/add
```


##### 说明
添加权限


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**token**  <br>*可选*|用户的认证标识|string|
|**Query**|**descript**  <br>*必填*|描述|string|
|**Query**|**iconPath**  <br>*可选*|请求路径|string|
|**Query**|**name**  <br>*必填*|名称|string|
|**Query**|**parentId**  <br>*必填*|父级权限id|integer (int64)|
|**Query**|**requestPath**  <br>*可选*|请求路径|string|
|**Query**|**sort**  <br>*可选*|排序|integer (int32)|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[Result](#result)|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `\*/*`


##### HTTP请求示例

###### 请求 path
```
/saasUserPermissionList/add?descript=string&name=string&parentId=0
```


###### 请求 header
```json
"string"
```


##### HTTP响应示例

###### 响应 200
```json
{
  "code" : 0,
  "count" : 0,
  "data" : "object",
  "msg" : "string"
}
```


<a name="deleteusingpost_1"></a>
#### 删除权限
```
POST /saasUserPermissionList/delete
```


##### 说明
删除权限


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**token**  <br>*可选*|用户的认证标识|string|
|**Query**|**id**  <br>*必填*|权限表id|integer (int32)|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[Result](#result)|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `\*/*`


##### HTTP请求示例

###### 请求 path
```
/saasUserPermissionList/delete?id=0
```


###### 请求 header
```json
"string"
```


##### HTTP响应示例

###### 响应 200
```json
{
  "code" : 0,
  "count" : 0,
  "data" : "object",
  "msg" : "string"
}
```


<a name="listbyroleidusingpost"></a>
#### listByRoleId
```
POST /saasUserPermissionList/listByRoleId
```


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**token**  <br>*可选*|用户的认证标识|string|
|**Query**|**saasUserRoleId**  <br>*可选*|saasUserRoleId|integer (int64)|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|object|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `\*/*`


##### HTTP请求示例

###### 请求 path
```
/saasUserPermissionList/listByRoleId
```


###### 请求 header
```json
"string"
```


##### HTTP响应示例

###### 响应 200
```json
"object"
```


<a name="pagingusingpost_1"></a>
#### 分页查询管理员权限
```
POST /saasUserPermissionList/paging
```


##### 说明
分页查询管理员权限


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**token**  <br>*可选*|用户的认证标识|string|
|**Query**|**keywords**  <br>*可选*|搜索关键词|string|
|**Query**|**limit**  <br>*必填*|每页条数|integer (int32)|
|**Query**|**page**  <br>*必填*|当前页|integer (int32)|
|**Query**|**parentId**  <br>*必填*|父级权限id|integer (int64)|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[Result«List«SaasUserPermissionList»»](#bd8b051e5e5da36fa4aa5fde2ed82304)|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `\*/*`


##### HTTP请求示例

###### 请求 path
```
/saasUserPermissionList/paging?limit=0&page=0&parentId=0
```


###### 请求 header
```json
"string"
```


##### HTTP响应示例

###### 响应 200
```json
{
  "code" : 0,
  "count" : 0,
  "data" : [ {
    "addTime" : "string",
    "descript" : "string",
    "iconPath" : "string",
    "id" : 0,
    "modifyTime" : "string",
    "name" : "string",
    "parentId" : 0,
    "requestPath" : "string",
    "saasUserPermissionList" : [ {
      "addTime" : "string",
      "descript" : "string",
      "iconPath" : "string",
      "id" : 0,
      "modifyTime" : "string",
      "name" : "string",
      "parentId" : 0,
      "requestPath" : "string",
      "saasUserPermissionList" : [ "..." ],
      "sort" : 0
    } ],
    "sort" : 0
  } ],
  "msg" : "string"
}
```


<a name="updateusingpost_1"></a>
#### 修改权限
```
POST /saasUserPermissionList/update
```


##### 说明
修改权限


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Header**|**token**  <br>*可选*|用户的认证标识|string|
|**Query**|**descript**  <br>*必填*|描述|string|
|**Query**|**iconPath**  <br>*可选*|请求路径|string|
|**Query**|**id**  <br>*必填*|权限表id|integer (int64)|
|**Query**|**name**  <br>*必填*|名称|string|
|**Query**|**parentId**  <br>*必填*|父级权限id|integer (int64)|
|**Query**|**requestPath**  <br>*可选*|请求路径|string|
|**Query**|**sort**  <br>*可选*|排序|integer (int32)|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[Result](#result)|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `\*/*`


##### HTTP请求示例

###### 请求 path
```
/saasUserPermissionList/update?descript=string&id=0&name=string&parentId=0
```


###### 请求 header
```json
"string"
```


##### HTTP响应示例

###### 响应 200
```json
{
  "code" : 0,
  "count" : 0,
  "data" : "object",
  "msg" : "string"
}
```



