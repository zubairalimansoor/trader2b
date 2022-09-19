# how to use <a href="https://trader2b.com/pricing/">trader2B</a> C# API for trading

1- In your solution add reference to C# api dll provided by the support
2- Create instance of HaywoodAPI
3- call function connect with following parameters 
  - Server IP or URL something like xyz.trader2b.com (please get it from trader2B support)
  - your username
4- Call function Login with username and password
5- if login is successfull call following based on need to load trading accounnt details
   - GetUserDetails
6- Subscribe to receive order/position updates by registering for delegtes 
  - onTradeMsg
  - onSymbolPositionUpdate
  - onAccPositionUpdate
  
7- Use folloiwng functions for sending order and also to cancel order
    - PlaceOrder
    - CancelOrder
    - ReplaceOrder
