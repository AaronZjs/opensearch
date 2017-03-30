# opensearch

阿里云开发搜索composer包

阿里文档:https://help.aliyun.com/product/29102.html

封装阿里云 open search sdk 版本v2.0.6 (2015-07)

使用方法:


use Aliyun\opensearch as search;



$access_key = "your key";

$secret = "your secret";

//杭州公网API地址：http://opensearch-cn-hangzhou.aliyuncs.com

//北京公网API地址：http://opensearch-cn-beijing.aliyuncs.com 

$host = "http://opensearch-cn-beijing.aliyuncs.com";//根据自己的应用区域选择API

$key_type = "aliyun";  //固定值，不必修改

$opts = array('host'=>$host);



// 实例化一个SDK客户端client

$client = new search\CloudsearchClient($access_key,$secret,$opts,$key_type);
