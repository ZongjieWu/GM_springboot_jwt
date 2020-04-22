
<a name="definitions"></a>
## 定义

<a name="result"></a>
### Result
返回的数据


|名称|说明|类型|
|---|---|---|
|**code**  <br>*可选*|返回码  <br>**样例** : `0`|integer (int32)|
|**count**  <br>*可选*|数据的总条数(此字段用于分页的时候用)  <br>**样例** : `0`|integer (int64)|
|**data**  <br>*可选*|返回数据  <br>**样例** : `"object"`|object|
|**msg**  <br>*可选*|返回消息  <br>**样例** : `"string"`|string|


<a name="d81602790788bd27cb5a976bd576dfb6"></a>
### Result«List«SaasUserBaseInfoResponseVo»»
返回的数据


|名称|说明|类型|
|---|---|---|
|**code**  <br>*可选*|返回码  <br>**样例** : `0`|integer (int32)|
|**count**  <br>*可选*|数据的总条数(此字段用于分页的时候用)  <br>**样例** : `0`|integer (int64)|
|**data**  <br>*可选*|返回数据  <br>**样例** : `[ "[saasuserbaseinforesponsevo](#saasuserbaseinforesponsevo)" ]`|< [SaasUserBaseInfoResponseVo](#saasuserbaseinforesponsevo) > array|
|**msg**  <br>*可选*|返回消息  <br>**样例** : `"string"`|string|


<a name="bd8b051e5e5da36fa4aa5fde2ed82304"></a>
### Result«List«SaasUserPermissionList»»
返回的数据


|名称|说明|类型|
|---|---|---|
|**code**  <br>*可选*|返回码  <br>**样例** : `0`|integer (int32)|
|**count**  <br>*可选*|数据的总条数(此字段用于分页的时候用)  <br>**样例** : `0`|integer (int64)|
|**data**  <br>*可选*|返回数据  <br>**样例** : `[ "[saasuserpermissionlist](#saasuserpermissionlist)" ]`|< [SaasUserPermissionList](#saasuserpermissionlist) > array|
|**msg**  <br>*可选*|返回消息  <br>**样例** : `"string"`|string|


<a name="4ac26851a62c3f174fa06f2974ee94d6"></a>
### Result«List«SaasUserRoleType»»
返回的数据


|名称|说明|类型|
|---|---|---|
|**code**  <br>*可选*|返回码  <br>**样例** : `0`|integer (int32)|
|**count**  <br>*可选*|数据的总条数(此字段用于分页的时候用)  <br>**样例** : `0`|integer (int64)|
|**data**  <br>*可选*|返回数据  <br>**样例** : `[ "[saasuserroletype](#saasuserroletype)" ]`|< [SaasUserRoleType](#saasuserroletype) > array|
|**msg**  <br>*可选*|返回消息  <br>**样例** : `"string"`|string|


<a name="6808aa882c818db47bc2ed70acfe3dbd"></a>
### Result«SaasUserBaseInfoResponseVo»
返回的数据


|名称|说明|类型|
|---|---|---|
|**code**  <br>*可选*|返回码  <br>**样例** : `0`|integer (int32)|
|**count**  <br>*可选*|数据的总条数(此字段用于分页的时候用)  <br>**样例** : `0`|integer (int64)|
|**data**  <br>*可选*|返回数据  <br>**样例** : `"[saasuserbaseinforesponsevo](#saasuserbaseinforesponsevo)"`|[SaasUserBaseInfoResponseVo](#saasuserbaseinforesponsevo)|
|**msg**  <br>*可选*|返回消息  <br>**样例** : `"string"`|string|


<a name="0da2f56c139f0adac96edef56e911548"></a>
### Result«SaasUserRolePermission»
返回的数据


|名称|说明|类型|
|---|---|---|
|**code**  <br>*可选*|返回码  <br>**样例** : `0`|integer (int32)|
|**count**  <br>*可选*|数据的总条数(此字段用于分页的时候用)  <br>**样例** : `0`|integer (int64)|
|**data**  <br>*可选*|返回数据  <br>**样例** : `"[saasuserrolepermission](#saasuserrolepermission)"`|[SaasUserRolePermission](#saasuserrolepermission)|
|**msg**  <br>*可选*|返回消息  <br>**样例** : `"string"`|string|


<a name="saasuser"></a>
### SaasUser

|名称|说明|类型|
|---|---|---|
|**addTime**  <br>*可选*|**样例** : `"string"`|string (date-time)|
|**addr**  <br>*可选*|**样例** : `"string"`|string|
|**email**  <br>*可选*|**样例** : `"string"`|string|
|**headImg**  <br>*可选*|**样例** : `"string"`|string|
|**id**  <br>*可选*|**样例** : `0`|integer (int64)|
|**idCard**  <br>*可选*|**样例** : `"string"`|string|
|**modifyTime**  <br>*可选*|**样例** : `"string"`|string (date-time)|
|**name**  <br>*可选*|**样例** : `"string"`|string|
|**phone**  <br>*可选*|**样例** : `"string"`|string|
|**pwd**  <br>*可选*|**样例** : `"string"`|string|
|**saasUserPermissionList**  <br>*可选*|**样例** : `[ "[saasuserpermissionlist](#saasuserpermissionlist)" ]`|< [SaasUserPermissionList](#saasuserpermissionlist) > array|
|**saasUserRoleId**  <br>*可选*|**样例** : `0`|integer (int64)|
|**saasUserRoleName**  <br>*可选*|**样例** : `"string"`|string|
|**status**  <br>*可选*|**样例** : `0`|integer (int32)|


<a name="saasuserbaseinforesponsevo"></a>
### SaasUserBaseInfoResponseVo
后台管理员基本信息实体响应数据


|名称|说明|类型|
|---|---|---|
|**addTime**  <br>*可选*|添加时间  <br>**样例** : `"string"`|string (date-time)|
|**addr**  <br>*可选*|联系地址  <br>**样例** : `"string"`|string|
|**email**  <br>*可选*|邮箱  <br>**样例** : `"string"`|string|
|**headImg**  <br>*可选*|头像  <br>**样例** : `"string"`|string|
|**id**  <br>*可选*|平台管理员表id  <br>**样例** : `0`|integer (int64)|
|**idCard**  <br>*可选*|身份证  <br>**样例** : `"string"`|string|
|**modifyTime**  <br>*可选*|修改时间  <br>**样例** : `"string"`|string (date-time)|
|**name**  <br>*可选*|名称  <br>**样例** : `"string"`|string|
|**phone**  <br>*可选*|电话  <br>**样例** : `"string"`|string|
|**saasUserPermissionList**  <br>*可选*|**样例** : `[ "[saasuserpermissionlist](#saasuserpermissionlist)" ]`|< [SaasUserPermissionList](#saasuserpermissionlist) > array|
|**saasUserRoleId**  <br>*可选*|管理员角色id  <br>**样例** : `0`|integer (int64)|
|**saasUserRoleName**  <br>*可选*|**样例** : `"string"`|string|
|**token**  <br>*可选*|**样例** : `"string"`|string|


<a name="saasuserpermissionlist"></a>
### SaasUserPermissionList

|名称|说明|类型|
|---|---|---|
|**addTime**  <br>*可选*|**样例** : `"string"`|string (date-time)|
|**descript**  <br>*可选*|**样例** : `"string"`|string|
|**iconPath**  <br>*可选*|**样例** : `"string"`|string|
|**id**  <br>*可选*|**样例** : `0`|integer (int64)|
|**modifyTime**  <br>*可选*|**样例** : `"string"`|string (date-time)|
|**name**  <br>*可选*|**样例** : `"string"`|string|
|**parentId**  <br>*可选*|**样例** : `0`|integer (int64)|
|**requestPath**  <br>*可选*|**样例** : `"string"`|string|
|**saasUserPermissionList**  <br>*可选*|**样例** : `[ "[saasuserpermissionlist](#saasuserpermissionlist)" ]`|< [SaasUserPermissionList](#saasuserpermissionlist) > array|
|**sort**  <br>*可选*|**样例** : `0`|integer (int32)|


<a name="saasuserrolepermission"></a>
### SaasUserRolePermission

|名称|说明|类型|
|---|---|---|
|**addTime**  <br>*可选*|**样例** : `"string"`|string (date-time)|
|**id**  <br>*可选*|**样例** : `0`|integer (int64)|
|**modifyTime**  <br>*可选*|**样例** : `"string"`|string (date-time)|
|**saasUserPermissionId**  <br>*可选*|**样例** : `0`|integer (int64)|
|**saasUserRoleId**  <br>*可选*|**样例** : `0`|integer (int64)|


<a name="saasuserroletype"></a>
### SaasUserRoleType

|名称|说明|类型|
|---|---|---|
|**addTime**  <br>*可选*|**样例** : `"string"`|string (date-time)|
|**descript**  <br>*可选*|**样例** : `"string"`|string|
|**id**  <br>*可选*|**样例** : `0`|integer (int64)|
|**modifyTime**  <br>*可选*|**样例** : `"string"`|string (date-time)|
|**name**  <br>*可选*|**样例** : `"string"`|string|



