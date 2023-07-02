# Momo-Payment-API
Using Postman

# PROCESS FLOW

![image](https://github.com/fdat3/Momo-Payment-API/assets/92992993/8247bea8-fabb-415a-8080-728c4cea9a64)

# REQUEST BODY EXAMPLE

```json
{
  "partnerCode": "MOMO",
  "partnerName" : "Test",
  "storeId" : "MoMoTestStore",
  "requestType": "captureWallet",
  "ipnUrl": "https://momo.vn",
  "redirectUrl": "https://momo.vn",
  "orderId": "MM1540456472575",
  "amount": 150000,
  "lang":  "vi",
  "orderInfo": "SDK team.",
  "requestId": "MM1540456472575",
  "extraData": "eyJ1c2VybmFtZSI6ICJtb21vIn0=",
  "signature": "fd37abbee777e13eaa0d0690d184e4d7e2fb43977281ab0e20701721f07a0e07"
  "items": {
    "id": "204727",  
    "name": "YOMOST Bac Ha&Viet Quat 170ml",  
    "description": "YOMOST Sua Chua Uong Bac Ha&Viet Quat 170ml/1 Hop",
    "category": "beverage",
    "imageUrl":"https://momo.vn/uploads/product1.jpg",
    "manufacturer":"Vinamilk",
    "price": 11000,               
    "quantity": 5,
    "unit":"hộp",
    "totalPrice": 55000,
    "taxAmount":"200"
  }
  "userInfo": {
    "name": "Nguyen Van A",
    "phoneNumber": "0999888999",
    "email": "email_add@domain.com",
  }
  "deliveryInfo": {
    "deliveryAddress": "Phu My Hung Tower",
    "deliveryFee": "30000",
    "quantity": "2"
  }

}

```

# RESPONSE EXAMPLE 

```json
{
  "partnerCode": "MOMO",
  "requestId": "MM1540456472575",
  "orderId": "MM1540456472575",
  "amount": 150000,
  "responseTime": 145256987,
  "message": "Thành công",
  "resultCode": 0,
  "payUrl": "https://test-payment.momo.vn/v2/gateway/pay?t=TU9NT1NKSTEyMDE5MDgyM3wxNjEzNTMyMDk3OTIyOjAxMjM0NTY3Nzg=",
  "deeplink": "momo://?action=payWithAppToken&amount=150000&fee=0&requestType=payment&orderLabel=M%C3%A3+%C4%91%C6%A1n+h%C3%A0ng&orderId=MM1540456472575&requestId=MM1540456472575&merchantnamelabel=Nh%C3%A0+cung+c%E1%BA%A5p&description=SDK+team.&partnerCode=MOMO&merchantcode=MOMO&language=vi&merchantname=MoMo+Payment&packageId=&extras=&extraData=email=abc@gmail.com&deeplinkCallback=https%3A%2F%2Ftest-payment.momo.vn%2Fgw_payment%2Fm2%3Fid%3DM7EWVy&callbackUrl=https%3A%2F%2Ftest-payment.momo.vn%2Fgw_payment%2Fm2%3Fid%3DM7EWVy&urlSubmitToken=https%3A%2F%2Ftest-payment.momo.vn%2Fgw_payment%2Fpayment_with_app%3FpartnerCode%3DMOMO%26accessKey%3DF8BBA842ECF85%26requestId%3DMM1540456472575%26orderId%3DMM1540456472575%26orderInfo%3DSDK%2Bteam.%26amount%3D150000%26signature%3Ddf2a347519abb91e9c1bd1bee80e675f4108cb6dbcac531979e805857293d486%26requestType%3DcaptureWallet%26payType%3Dapp-in-app&appScheme=",
  "qrCodeUrl": "https://test-payment.momo.vn/gw_payment/s/zoVKZd"
}
```

# READ MORE 

[https://developers.momo.vn]

# USING POSTMAN API FOR TEST IN API FOLDER
