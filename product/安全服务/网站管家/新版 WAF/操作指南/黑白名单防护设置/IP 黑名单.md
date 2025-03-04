## 添加 IP 黑名单
#### 手动添加
1. 登录 [Web 应用防火墙控制台](https://console.cloud.tencent.com/guanjia/tea-iplist)，在左侧导航栏中，选择**配置中心** > **黑白名单**。
2. 在黑白名单页面，左上角选择需要防护的域名，单击 **IP 黑名单**。
![](https://qcloudimg.tencent-cloud.cn/raw/87b7e07391f926ee79bc5dbfc0420ba0.png)
3. 在 IP 黑名单页面，单击**添加地址**，进入添加黑名单页面。
4. 在添加黑名单页面，配置相关参数，单击**确定**。
![](https://qcloudimg.tencent-cloud.cn/raw/ebe06ba5a593d5073d4f919fec18bc2a.png)
**字段说明：**
 - **IP 地址：**支持任意 IP 地址，例如10.0.0.10或 FF05::B5；支持 CIDR 格式地址，例如10.0.0.0/16或 FF05:B5::/60，使用换行符进行分隔，一次最多添加20个。
>?
>- 选择域名为**全局**时，添加的 IP 地址或 IP 段为全局的黑白名单。
>- 各个版本每个域名规格限制为：高级版1000条/域名、企业版5000条/域名、旗舰版：20000条/域名，每个 IP 地址或者 IP 段占用一条额度。
 - **截止时间：**永久生效或限定日期。
 - **备注：**自定义，50个字符以内。

#### 导入数据
1. 在 [黑白名单页面](https://console.cloud.tencent.com/guanjia/tea-iplist)，左上角选择需要防护的域名，单击 **IP 黑名单**。
2. 在 IP 黑名单页面，单击**导入数据** > **导入**，解析成功后，单击**确认导入**即可。
![](https://qcloudimg.tencent-cloud.cn/raw/9d968c6a6f0aa7760f2d85dcb3a2d436.png)

## 编辑 IP 黑名单
1. 在 [黑白名单页面](https://console.cloud.tencent.com/guanjia/tea-iplist)，左上角选择需要防护的域名，单击 **IP 黑名单**。
2. 在 IP 黑名单页面，选择所需 IP 地址，单击操作列的**编辑**，修改截止时间和备注，单击**确定**保存。
![](https://qcloudimg.tencent-cloud.cn/raw/efecac233eea085b81db083b50366da4.png)

## 删除 IP 黑名单
1. 在 [黑白名单页面](https://console.cloud.tencent.com/guanjia/tea-iplist)，左上角选择需要防护的域名，单击 **IP 黑名单**。
2. 在 IP 黑名单页面，支持删除单个、部分、全部地址，具体操作如下：
 - 单个：选择单个 IP 地址，单击**删除地址**或操作列的**删除**，弹出“确认删除”弹窗。
>?删除后将无法恢复，重新添加才能生效。
>
![](https://qcloudimg.tencent-cloud.cn/raw/6d1c66cce48ce2e19392afaa365cbffa.png)
 - 部分：选择多个 IP 地址，单击**删除地址**，弹出“确认删除”弹窗。
>?删除后将无法恢复，重新添加才能生效。
>
 ![](https://qcloudimg.tencent-cloud.cn/raw/3fe416b393ea54ba8ff66c3066344c5b.png)
 - 全部：单击**全部删除**，弹出“确认删除”弹窗。
>!将清除当前域名下所有的 IP 黑白名单信息，请谨慎操作！删除后将无法恢复，重新添加才能生效。
3. 在“确认删除”弹窗中，单击**确定**，即可删除地址。



## 导出全部筛选结果
1. 在 [黑白名单页面](https://console.cloud.tencent.com/guanjia/tea-iplist)，左上角选择需要防护的域名，单击 **IP 黑名单**。
2. 在 IP 黑名单页面，单击搜索框通过 **IP 地址**对 IP 进行筛选，或单击**来源**根据来源分类对 IP 进行筛选。
![](https://qcloudimg.tencent-cloud.cn/raw/acf557ce82eb57d47e86daa7c858a07f.png)
3. 筛选完所需 IP 后，单击**导出全部筛选结果**，即可导出所需的 IP 筛选结果。
![](https://qcloudimg.tencent-cloud.cn/raw/d375d83269003b674aa75a71f126acfa.png)
