# DatabaseAssignment11

The assignment is made in Pythons Jupyter Notebook, and Mysql 8.0 database is used.
The ORM is programmed in tailored process and is not flexible like a real middle component that can handle the entire class/relational concept. The program follows the json format as the starting data.

{"schemaName": "MicroShop",
  "entities": [
  	{"Customer": {
  		"name": "String",
  		"orders" :"*Order"}},
  	{"Order" :{
  		"date": "String",
  		"total": "Number",
  		"customer": "Customer",
  		"lines": "*OrderLine" }},
  	{"OrderLine" : {
  		"order": "Order",
  		"product": "Product",
  		"count": "Number",
  		"total": "Number" }},
  	{"Product" : {
  		"name": "String",
  		"price" :"Number"}}
  ]
}

To run the program you will need to have python/jupyter notebook and mysql installed. If not you can use colab as an alternative. 
