
    
**简要描述：** 

- 交易

**请求URL：** 
- ` http://www.bitdot.io/submitOrder?AccessKey=e2xxxxxx-99xxxxxx-84xxxxxx-7xxxx&SignatureMethod=HmacSHA256&Timestamp=2017-05-11T15:19:30&Signature=s3sdfae46565 `
  
**请求方式：**
- POST 

**参数：** 

|参数名|必选|类型|说明|
|:----    |:---|:----- |-----   |
|type |是  |string |卖或者是买，1买2卖（放在请求体内）   |
|symbol |是  |string | 交易对，如eth_btc （放在请求体内）   |
|price     |否  |string | 价格 （放在请求体内）   |
|number     |是  |string | 数量 （放在请求体内）   |


 **请求示例**

``` 
  {
      "symbol":"ns_eth",
      "price":"0.70",
      "number":"1",
      "type":2
  }
```

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

- 
