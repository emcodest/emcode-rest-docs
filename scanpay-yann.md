

#  ScanPay  Doc on Yann

### 1. @LOGIN TO USER WALLET

###### HTTP/1.1 POST

**EndPoint:** {{base_url}}/api/v2/login  

**Request Body:** {
	
    "phone":"+2348064642044",
    "pin": "1421"
	
}

**Response Body:** {


	"status": "success",
	"message": "Successfully logged in.",
	"results": 1,
	"data": {
		"jwt": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJfaWQiOiI2MGExNTMyNGZhNGQwMWZmMGUwYjkzMTkiLCJlbWFpbCI6ImVlZW1hOUBnbWFpbC5jb20iLCJzZXNzaW9uX3Rva2VuIjoiVEstaTR6Q2tUNWF2N3dlXnBLVF9hQ2UiLCJpYXQiOjE2ODgwNDY1OTIsImV4cCI6MTk0NzI0NjU5Mn0.eG_-yVE7lDotcQq8sDDy4OfQnHWNZ5w7xJbCdbe2Dzg",
		"email": "eeema9@gmail.com",
		"isVerified": true,
		"reference": "SCANPAY-664253",
		"referral_code": "XY5Y66k-1621185316",
		"message": "",
		"success": true,
		"error": false,
		"code": "00",
		"pin": "xxxx",
		"user_id": 53,
		"token_expires": "false",
		"full_name": "Emma Jr",
		"address": null,
		"phone": "+2348064642044",
		"account_no": "7810595478",
		"bank_code": "035",
		"balance": 476,
		"token": "TK-i4zCkT5av7we^pKT_aCe",
		"card_details": [],
		"facially_recognized": false,
		"facial_recognition_pictures": [],
		"_id": "60a15324fa4d01ff0e0b9319"
	}
}
### 2. @REGISTER WALLET

###### HTTP/1.1 POST

**EndPoint:** {{base_url}}/api/v2/register   

**Request Body:** {

     "firstname":"Emcode",
    "lastname":"LLC",
    "email":"emcodellc@gmail.com",
    "phone":"+2348064642044",
    "address": "Port Harcourt, Nigeria",
    "pin": "1421",
    "location": "Latitude: 3.4555587,Longitude: 6.7534736",
    "bvn": ""
	
}

**Response Body:** {

	"status": "success",
	"message": "Successfully Registered",
}

### 3. @GET USER WALLET

**EndPoint:** {{base_url}}/api/v2/user/account  

###### HTTP/1.1 GET

**Header:** {

    "Authorization": "Bearer jwt-token"
}

**Request Body:** {

    "firstname":"Emcode",
    "lastname":"LLC",
    "email":"emcodellc@gmail.com",
    "phone":"+2348064642044",
    "address": "Port Harcourt, Nigeria",
    "pin": "1421",
    "location": "Latitude: 3.4555587,Longitude: 6.7534736",
    "bvn": ""
	
}

**Response Body:** {

	"status": "success",
	"message": "Retrieved successfully",
	"results": 1,
	"data": {
		"message": "successful",
		"success": "true",
		"error": false,
		"code": "00",
		"bank_code": "000",
		"bank_name": "Wallet Account",
		"balance": 0,
		"account_name": "oluwasae oluwaseyi",
		"account_number": "2235206248",
		"reference": "64838a1f1e868b115ea10564",
		"wallet_id": "64838a1f1e868b115ea10562",
		"wallet_token": "************",
		"wallet_pin": "xxxx",
		"phone": "+2347063319339",
		"email": "oluwasaejoseph@gmail.com",
		"created_at": "2023-06-09T20:22:55.000Z",
		"fos": 0
	}
}



