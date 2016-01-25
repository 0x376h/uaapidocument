# 中文文档
接口地址:http://freeapi.ua.datatiny.com/api  
参数:无  
提示:修改http请求中的user-agent即可得到不同的内容
限制:一个ip每一秒3次  
返回结果:
<pre>
{
    "status": "success",
    "data": {
        "platform": "",
        "os": {
            "osname": "Android",
            "osverion": "4.2.1",
            "osplatformtype": 0
        },
        "appinfo": {
            "platform": "Android",
            "appname": "MicroMessenger",
            "appdesc": "微信",
            "appver": "6.3.7.65_r060a025.660"
        },
        "deviceinfo": [
            {
                "company": "OPPO",
                "devicename": "OPPO R823T（移动版）",
                "devicestr": "r823t"
            }
        ],
        "networkinfo": {
            "networkstatus": "WIFI",
            "networkdesc": ""
        }
    },
    "code": 1
}
</pre>
## status取值
* success :表示请求成功
* fail :表示请求失败

## data 描述
### platform: 平台类型,目前保留，  

### os  操作系统信息
  * osname:操作系统名:目前支持android,IOS,windows phone [查看支持所有的os](/osinfos.md)  
  * osverion:操作系统版本  
  * osplatformtype:保留  
 
### appinfo  应用信息
  * platform :app的平台，一般与osname相同  
  * appname : 应用名称 [查看支持所有的app](/appinfos.md)  
  * appdesc :应用描述，目前只有中文  
  * appver :应用版本  
 
### deviceinfo 设备信息  
  * company: 企业名称  
  * devicename: 设备名称  
  * devicestr: 设备特征  
  
### networkinfo 网络状态信息  
  * networkstatus : 网络状态  [查看支持所有的网络状态](/networkstatus.md)  
  * networkdesc :描述  
  
## code:
   1 - 成功 
 
## tips:
如果有问题，欢迎 [创建issue](https://github.com/0x376h/uaapidocument/issues/new)
 