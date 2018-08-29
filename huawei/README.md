华为不提供服务端的 SDK。
文档也都没有 PDF 版的。

[华为推送接入文档](https://developer.huawei.com/consumer/cn/service/hms/catalog/huaweipush_agent.html?page=hmssdk_huaweipush_sdkdownload_agent)

华为推送服务的接入方只能通过 REST API 来访问华为推送服务的服务端接口。华为推送服务的服务端接口主要有两个接口，分别是获得访问令牌和推送消息。

获得访问令牌接口的详细说明[文档](https://developer.huawei.com/consumer/cn/service/hms/catalog/huaweipush_agent.html?page=hmssdk_huaweipush_api_reference_agent_s1)。


## 消息回执

(1). 回执的安全
目前华为Push服务器和接收回执消息的 APP 服务器之间走的是HTTPS 协议，华为 Push 服务器会校验 APP 服务器提供证书的合法性，APP 服务器务必使用正式商用的HTTPS证书。

(2). 回执消息的开通
a). 开通Push服务后，发送邮件到 (developer@huawei.com)申请开通回执消息，邮件中需要提供应用的 AppId、接收回执消息的URL地址以及每天发送消息的总量。
b). 申请加入华为 Push 回执 QQ 群，便于后续联调功能以及沟通交流问题，QQ群号：224090622。

(3). 回执消息的API
回执消息发生在系统检测到客户端有应答返回，并且有 CP 订阅了该应答结果的场景。华为Push平台和CP接收回执消息服务器使用HTTPS协议。

详细的说明健[华为文档](https://developer.huawei.com/consumer/cn/service/hms/catalog/huaweipush_agent.html?page=hmssdk_huaweipush_devguide_server_agent#3.3 消息回执)。