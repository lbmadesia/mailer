# Route access module

It is module for send mail with dynamic template controll, it's make you avoid to reated line code for notification.



### Install Dependencies

Step 1.
```
npm install mailer
```
### Required 
these moddule should be installed if not then copy below and install 
Step 2.
```
npm install nodemailer
```
```
npm install dotenv
```
```
npm install path
```
```
npm install fs
```

Step 3. ### add below point in .env
```
APP_NAME=LBSETTECH
DOMAIN_ADD=http://localhost:8080/

MAIL_SERVICE=gmail
MAIL_ID=xyz@gmail.com
MAIL_PASSWORD=xyzz
MAIL_FROM=xyz@gmail.com
```
Step 4. ### link module and use any where in the project 

```
const mailer = require('mailer');

await mailer.greeting("Hello");
  await mailer.subject("it's mail from mailer");
  await mailer.line("your text is through line method, use  line method as much you want new.");
  mailer.link("https://github.com/lbmadesia/documents/mailer","click here"); //second parameter is optional
  await mailer.line(" to Know about mailer");
  await mailer.button("Contact to me","mailto:lbmadesia@email.com");  //second parameter is optional
  await mailer.footer("here is all deatils footer");
  await mailer.attachments([{name:"filename.png",path:"/storages/a.png"},{name:"ptest.png",path:"http://localhost:8080/storages/lb.png"}]);
  let data = await mailer.notify('lalbabu@aresourcepool.com');
```


## Issues

If you come across any issues please report them [here](https://github.com/lbmadesia/mailer/issues).

## Contributing
Feel free to create any pull requests for the project. For proposing any new changes or features you want to add to the project, you can send us an email at following addresses.

    (1) Lb Madesia - lbmadesia@gmail.com

# License
This mailer is open-sourced Module licensed under the MIT license

