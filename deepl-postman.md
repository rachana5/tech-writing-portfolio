# How to translate text with DeepL API using Postman

## Introduction

[Postman](https://www.postman.com/) is a software for developers to create, test, and manage API endpoints. [DeepL](https://www.deepl.com/translator) is a translation tool and with the API users can integrate translation to applications.

This guide describes how to send a request to the DeepL translation endpoint to translate text using Postman. By the end of this guide, you will have a basic understanding of using Postman to create and send API calls.

## Prerequisites

1. A Postman account - you can create an account for free if you don't have one. See https://www.postman.com/ 
2. A DeepL API account - you can create an account with the free plan. You need to provide your credit card details but you are not charged unless you manually upgrade to the pro plan. See https://www.deepl.com/pro#developer

## Steps to translate
We are using the DeepL API endpoint **POST** `{domain}/v2/translate` to translate *Hello, world!* from English to Estonian. You can either download the Postman app to your machine, or you can use it on the web.

1. When you first log in to Postman, you can see the home page.

	![Screenshot of the Postman home screen](images/welcome-screen.png)

2. Click **Create request** from the left-hand menu to create your first API request. An **Untitled Request** opens which is set to the **GET** method by default.

	![Screenshot of the new untitled request](images/new-request.png)

3. Select the method **POST** from the drop-down menu. In the text bar next to the method, enter the URL `https://api-free.deepl.com/v2/translate`.
4. In the **Params** table, enter the following values:

	| Key  | Value |
	| ------------- | ------------- |
	| auth_key | Go to your DeepL account details and copy the authentication key here. |
	| target_lang | et |
	| text | Hello, world! |
  
	The table should look something like this: 
  
	![Screenshot of the API request and parameters](images/post-request-params.png)

	>**Note**
	>For detailed information about the endpoint and the parameters, see [Translate Text](https://www.deepl.com/docs-api/translate-text/translate-text/).

5. Click **Save**. You are prompted to edit the request name and create a collection. A collection is a folder to save your requests.

	Enter the **Request name** as **hello-world** and create a collection called **Translation**. Once you have created the collection, you should see the following screen:
	
	![Screenshot of the page to save the request](images/save-request.png)
	
6. Click **Save**. The collection called **Translation** is created and the POST request **hello-world** is saved in this collection.

7. Now, click **Send**. For a successful request, you can see the translated text in the response body. The following screenshot shows the response with the translated text *Tere, maailm!*:

	![Screenshot of the response with the translated text](images/response.png)
	
Nice work! You have sent your first successful request in Postman.

>**Note:**
>In case of errors, see the DeepL [Error Handling](https://www.deepl.com/docs-api/api-access/error-handling/) section. 
