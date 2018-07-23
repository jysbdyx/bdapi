
    
**简要描述：** 

- 交易

**请求URL：** 
- ` https://newcoin.org/v1/order/setOrders?AccessKey=e2xxxxxx-99xxxxxx-84xxxxxx-7xxxx&Timestamp=2017-05-11T15:19:30&Signature=s3sdfae46565 `
  
**请求方式：**
- POST 

**参数：** 

|参数名|必选|类型|说明|
|:----    |:---|:----- |-----   |
|type |是  |string |卖或者是买，1买2卖   |
|symbol |是  |string | 交易对，如eth_btc    |
|price     |否  |string | 价格    |
|number     |否  |string | 数量    |


 **返回示例**

``` 
  {
    "errorCode": 0,
	"msg":"交易成功",
    "res":[]
  }
```

 **返回参数说明** 

|参数名|类型|说明|
|:-----  |:-----|-----                           |
|errorCode |int   |返回值状态，0代表处理成功，其他代表失败  |
|msg |string   |提示  |
|res |array   |数据  |

 **备注** 

- 无
