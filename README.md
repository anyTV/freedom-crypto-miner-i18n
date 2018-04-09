Please refer below steps to add a new language for Crypto Miner. E.g: now we will add Japanese 

### 1. Clone freedom-crypto-miner-i18n and create new branch 

`git clone https://github.com/anyTV/freedom-crypto-miner-i18n.git`

then...

`cd freedom-crypto-miner-i18n`

We we can see list of supported languages in this folder 
![](https://content.screencast.com/users/VoTuanPhong/folders/Jing/media/5df16f2b-e2c4-4192-bce8-59e59b08bb59/2018-04-09_1357.png)

then create new branch. E.g: Support_Japanese

`git checkout -b Support_Japanese`


### 2. Translating new language

#### 2.1 Copy en folder and rename it to new language ('ja')

![](https://content.screencast.com/users/VoTuanPhong/folders/Jing/media/ae891a9e-aa7f-4ab3-bd8b-c584b7648e33/2018-04-09_1409.png)

Please refer [iso-2-letter-language-codes](https://www.sitepoint.com/iso-2-letter-language-codes/) to find the language code

     E.g: Japanese   -> ja
          Italian    -> it
          ...

#### 2.2 Start translating new language

 Now you can start translating new language in new folder. E.g: ja\index.json

` cd ja`

 Use any text editor to open file index.json and start translating...
 This is json utf unicode format file, we will translate the value field of this file. E.g:

 ![](https://content.screencast.com/users/VoTuanPhong/folders/Jing/media/4f72af9d-7d63-44c6-a60c-203ecf9db456/2018-04-09_1440.png)


_Note: we have to make sure that index.json is stored in utf8 unicode_

### 4. Commit and Push 
Add your translation file

`git add ja\index.json`

_Note: you have to replace 'ja' by your support language_

Commit your work

`git commit -a -m "Support Japanese"`

Push your change

`git push`

_Note: please input your github authentication info if you are requested_

### 5. Create pull request 

Go to github repo [https://github.com/anyTV/freedom-crypto-miner-i18n](https://github.com/anyTV/freedom-crypto-miner-i18n)
If you push your work successfully, we can see the button 'Compare & pull request', click it to create pull request
![](https://content.screencast.com/users/VoTuanPhong/folders/Jing/media/6a5ead20-d637-4aba-8763-0b5d3a66878a/2018-04-09_1505.png) 

Click on 'Create pull request'

![](https://content.screencast.com/users/VoTuanPhong/folders/Jing/media/97c32142-8779-43ce-b8ad-cc3ebc1830e6/2018-04-09_1509.png)

Everything is done. We would receive notification of the pull request, and we'll
   1. review and test the code
   2. request for changes
   3. once all that's done, we'll merge and update our code
