## 获取小程序二维码

```
https://money.chinabanksoft.com/vendingmachine/trans/wms/relax_view/?id=SM0009&type=M
```

```
接口：https://money.chinabanksoft.com/vendingmachine/trans/wms/relax_view/
```

请求方式：get

请求参数：

| 字段 | 是否必填 | 说明              |
| ---- | -------- | ----------------- |
| id   | 是       | 设备code          |
| type | 是       | M：商城   R：补货 |

返回参考：

成功：

```
{
    "code": 200,
    "msg": "获取设备SM0001二维码成功",
    "img_addr": "https://money.chinabanksoft.com/vendingmachine/trans/files/uploads/applet_code/SM0001_mall.png"
}
```

失败：

```
{
    "code": 200,
    "state": 1,
    "msg": "设备编号不存在"
}
```



## 微信退款接口

请求方式：post

```
接口：pay/wx_refund/
```



| 字段           | 说明       | 是否必填 |
| -------------- | ---------- | -------- |
| transaction_id | 微信订单号 | 是       |
| out_trade_no   | 商户订单号 | 是       |
| refund_fee     | 退款金额   | 是       |

