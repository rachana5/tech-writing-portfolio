# How to use DeepL API

Postman is a software .... xxxx to be continued.
DeepL is .... xxxx to be continued.

Scenario: You want to test the DeepL API for text translation. You are using Postman for this.
This guide shows you how to call DeepL API endpoints to translate text using Postman.

## Prerequisites

1. A Postman account - you can create an account for free if you don't have one. See https://www.postman.com/ 
2. A DeepL account - you can create an account with the free plan. You need to provide your credit card details but you are not charged unless you manually upgrade to the pro plan. See https://www.deepl.com/translator

## Steps to translate
We are using the API endpoint **POST** `{domain}/v2/translate`. We are translating the phrase "Hello, world!" from English to Estonian. 

1. When you first log in to Postman, you can see the home page.

![Screenshot of the Postman home screen](images/welcome-screen.png)

2. Click **Create request** from the left-hand menu to create our first API request. An **Untitled Request** opens which is set to the **GET** method by default.

![Screenshot of the new untitled request](images/new-request.png)

3. Select the method **POST** from the drop-down menu. In the text bar next to the method, enter the URL `https://api-free.deepl.com/v2/translate`.
4. In the **Params** table, enter the following:

  | Key  | Value |
  | ------------- | ------------- |
  | auth_key | Go to your DeepL account details and copy the authentication key here. |
  | target_lang | et |
  | text | Hello, world! |
  
  The request should something like this: 
  
  ![Screenshot of the API request and parameters](images/post-request-params.png)
