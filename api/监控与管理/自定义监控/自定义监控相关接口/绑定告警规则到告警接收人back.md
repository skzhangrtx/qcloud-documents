## 1. 接口描述
域名:monitor.api.qcloud.com
接口名:BindAlarmRuleReceivers

为告警规则绑定接收组，目前一个告警规则只能绑定一个告警接受组

## 2. 输入参数
| 参数名称 | 必选  | 类型 | 描述 |来源|
|---------|---------|---------|---------|---------|
| Action | 是 | String | 操作接口名|系统规定参数，此处取值：BindAlarmRuleReceivers|
| alarmRuleId | 是 | String | 告警规则ID|调用<a href="/doc/api/255/查询告警规则" title="查询告警规则">查询告警规则</a>(DescribeAlarmRuleList)接口查询|
| receiversId | 是 | String | 接收组ID|用户自定义|


## 3. 输出参数
| 参数名称 | 类型 | 描述 |
|---------|---------|---------|
| code | Int | 错误码, 0: 成功, 其他值: 失败|
| message | String | 错误信息|


## 4. 示例
输入
```
https://monitor.api.qcloud.com/v2/index.php?Action=BindAlarmRuleReceivers
&alarmRuleId=policy-eqzqq79naz
&receiversId=1001
&COMMON_PARAMS
```
输出
```
{
    "code":"0",
    "message":""
}
```

