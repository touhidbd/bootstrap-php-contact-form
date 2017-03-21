# [Bootstrap - PHP Contact Form](http://tcoderbd.com#contact)

#Overview
This document provides instructions on how to add extra spam protection to your register and login forms using the free Google reCAPTCHA extension.

#Installing & activating
To add the Google reCAPTCHA extension to your site please do the following:

* Download the fils zip folder from [here](https://github.com/touhidbd/bootstrap-php-contact-form/archive/master.zip).
* Upload all reqiure files in you website.

#Site & secret keys
For the Google reCAPTCHA extension to work on your site you need to generate site and secret keys. If you already have the keys you can skip the next section. If you do not have your reCAPTCHA details already then click the “Generate your site and secret key” button where you will be taken to the official Google reCAPTCHA website.

#Generating your site & secret key
To generate your site and secret keys please visit the [Google reCAPTCHA](https://www.google.com/recaptcha/intro/index.html) site and click the blue “Get reCAPTCHA” button to login to the website using your Google account. Once logged in you will see the following page:

To create your site and secret key please do the following:
* Enter a label for your site e.g Ultimate Member.
* Enter your site’s domain name in the text area (do not include http:// or www and make sure you do not have a forward slash / at end of url).
* Click the register button.

Once you click register your site will be registered with Google reCAPTCHA and you will be redirected to the site overview page which contains the keys. The only two pieces of information you need from this page are the site key and secret key.


#Setup

* Edit the index.html and update your website Google reCAPTCHA Public Key

```html
<div class="g-recaptcha pull-left" data-sitekey="---Your Website Public Key---"></div>
```

* Edit the sendemail.php and update your website Google reCAPTCHA Secret Key and Receiving  Email Address.

```php
	$key = "Your Google Recaptcha Secret Key Here"; // Google Recaptcha Secret Key
	
	$email_to = 'your_email@domain.com';  // Your email address
```


[Demo](http://tcoderbd.com#contact)