# E-Shop (An online UK clothes site)

E-shop is a website designed to be sleek, easy UI and UX designed to work for everyone. It is suitable for all ages and has potential to advertise
too.
 
## UX
 
 During this project there were a large amount of user stories gathered asking various questions to people in order to know what they look for 
 in an online store:

#### Viewing and Navigation:

As a shopper, I would like to: 

                                1. View a list of products to be able to select one to purchase.
                                2. View individual products to be able to see all detailed and required information about it.
                                3. Quickly be able to access any deals and special offers to be able to take advantage of them.
                                4. Easily view my total amount in my current basket to be able to avoid spending too much.


With the site, it s designed to automatically render through 'for' loops in order to show the whole list of products, as well as sort them 
into individual catergories, such as clearance/deals as well as their own item categories too. The site has a seperate page that will also 
render each individual item and store its useful information that the customer would be looking for. The basket is also fully responsive,
updating as you shop as well as sending toast messages to the customer updating them on their shopping and actions.

#### Registration and user accounts

As a site user, I would like to:

                                1. Easily register for an account to be able to have my personal data saved and stored and check profile history.
                                2. Easy log in and out functionality to be able to access my account smoothly.
                                3. Be able to recover a lost password fuss free to be able to regain access to my profile.
                                4. Recieve email confirmation for registering to be able to see my account is verified successfully
                                5. Have a personalised account to be able to track my order history and save my payment and shipping details.


The profile app fufills all these user stories, it has email veriafication set up via a external Gmail account, using POST method in the code.
if a user forgets their password, a link will be emailed to them the same way veriafication of their account set up would be. All users shipping 
and personal data is stored and can be edited at anytime. We also have made order history avaliable which track it and will display all information
regarding that specific Object_ID of the order.

#### Sorting and searching

As a shopper, I would like to:

                                1. Sort through the list of products avaliable to be able to identify best rated ect...
                                2. Sort into specific categories to be able to easily find more specificly what I am looking for.
                                3. Sort multiple categories simultaneously to be able to to find best deals across broad categories.
                                4. Search by name or description to be able to find products quickly.
                                5. See what I have searched for to be able to decide if what i want is avaliable.

When products are rendered on the page, they are first registered via categories in the database, it is easy to click and search within these,
each item can be rated and can appear in order of rating value. The search bar is fully intergrated with the database, picking out
key words in both the product title and the description. The search bar also records searches to see what you have previously searched for too.

#### Purchase and checking out

As a shopper, I would like to:

                                1. Select the size and quantity I would like to purchase to be able to make sure I don't purchase the wrong size.
                                2. View items in my bag to be able to see what my sub-total is, check I havent put more than I would like in there.
                                3. Change the quantity of items selected in my bag to be able to edit my order before checkout.
                                4. Easily enter my payment details to be able to checkout fuss free.
                                5. Feel like my payment is secure and authenticated to be able to feel confident paying safely.
                                6. View the order confirmation after it has been placed to be able to see if there are any mistakes.
                                7. Recieve an email confirmation to be able to keep a personal record of my purchase.

The shopping bag app has all the functions listed above, you can search for specific key words to help locate a product, it also
saves your search results for future use. the categories are in palce allowing for broad groups of items to be listed together 
once and item is placed into the bag, a toast message will appear updating you on the item and description added as well as the price.
On the toast is also the option to checkout straight away if the shopper has finished browsing and would like to pay.
Once the payment form is filled in, the user has the option to save their details if they have decided to register an account with E-shop
and will be emailed on the email address given by them, via our customer service email account set up with Gmail.
There is also an order summary after checkout is completted to evaluate.

#### Admin and store management

As and Admin/Store owner, I would like to:

                                1. Add a product so new items can be listed on the store.
                                2. Edit/update existing products so if there are any promotions or any criterea to change it can be.
                                3. Delete a product so when a product is discontinued it can be removed.

When a user is granted super user status they will become an admin, admins on the website have the ability to change products with a built
back office system, in which everything can be editied fully, also if it is a simple deletion, super users can also add and edit a product
on the main website rather than logging into the back office admin.



## Features
 
### Existing Features

- Feature 1 - Login Functionality
    
    - This feature allows users to create/register accounts to the website, this feature allows users to track their order history as well
      as save their shipping and billing info for future purchases. This also applies for store owners/admins, who can create a super user account
      in order to edit things on the site.

- Feature 2 - Search Bar and Category Sorting
    
    - In order to help customers with finding items, there is an intergrated search bar which will help users search for key words in descriptions
      or titles to help find specifically what they desire. The search bar will also remember yor search history for ease of revisiting.

- Feature 3 - Full Operational Shopping Bag and Checkout system
    
    - When a user find what they require and add it to the bag, toast messages have been added in order to notify their current activity,
      and also given the option to checkout straight away when any item is placed in the bag. the checkout page is straight forward and easy to fill,
      though the stripe setup is currently on test as to not let people make legitimate payments. Once the payment has been confirmed, the user is 
      redirected to the order confirmation screen. This screen has the enitre order listed with all information, and an order confirmation email is sent.

- Feature 4 - Add / Edit / Delete 

    - When a user had admin/super user privileges they are able to edit everything either from the front end of the website, or in the admin section.
      forms have been made for the backend to be able to make editing products, adding and removing products seamless.

- Feature 5 - Mobile Compatability

    - The website has been built to be mobile friendly and will work and run effortlessly on a mobile device making the UX easy.

### Features Left to Implement

- Potential Features:
 
    - Comments / Reviews under items so customers can have written reasons for the ratings.
    - Click and collect option, providing the store has shops and isnt soley online.
    - Advertisement spaces

## Technologies Used

In this section, you should mention all of the languages, frameworks, libraries, and any other tools that you have used to construct this project. For each, provide its name, a link to its official site and a short sentence of why it was used.

- Languages used: 
                    - HTML
                    - CSS
                    - JS
                    - python
                    - JSON

- [JQuery](https://jquery.com)
    - The project uses **JQuery** to simplify DOM manipulation and to create some interative functions within the site.

- [BootStrap](https://getbootstrap.com/)
    - The project uses **BootStrap** to help structure the sight easily, small changes in the static CSS has edited this slightly but for the most part, this was used.

- [AWS](https://aws.amazon.com/)
    - **AWS** using the **IAM** and **S3** for storing any media files to use in the **HEROKU** deployment.

- [STRIPE](https://stripe.com/en-gb)
    - Used **Stripe** for a payment system, good and easy template to work with in CSS. 

- [Django](https://www.djangoproject.com/)
    - **Django** was used as the core framework system using python as the primary coding language.

- [FontAwesome](https://fontawesome.com/)
    - Used for some icons.

List of installed packages used: 

- boto3==1.14.41
- asgiref==3.2.10
- botocore==1.17.41
- dj-database-url==0.5.0
- Django==3.0.8
- django-allauth==0.42.0
- django-countries==6.1.2
- django-crispy-forms==1.9.2
- django-storages==1.9.1
- docutils==0.15.2
- gunicorn==20.0.4
- heroku==0.1.4
- jmespath==0.10.0
- oauthlib==3.1.0
- Pillow==7.2.0
- psycopg2-binary==2.8.5
- python-dateutil==2.8.1
- python3-openid==3.2.0
- pytz==2020.1
- requests-oauthlib==1.3.0
- s3transfer==0.3.3
- sqlparse==0.3.1
- stripe==2.50.0

## Testing

#### Search bar Testing

        1. Type into the search bar a key word of an item you are looking for, for example; 'JEANS'
        2. When searched check to see that all items are relevant to the key word, whether that is in
           the title or the description.
        3. Once done, click back to the home page via the logo, click the search bar, it will either show your result,
           if not, type j and it should then appear on the drop down text field.

#### Accounts

        1. Under 'My Account' click on register.
        2. Fill in the required fields, if you would like to check for security, type in an easy password i.e: 'Password123'
           this should come up with an error message saying, password too common. also try to put a password similar to username.
        3. Now once the form has been filled out on a non error test run, a toast should pop up asking for verification via email.
           originally before setting up the real email outgoings, you used to have to use the terminal to fetch the link, but if you
           have used a real or temporary email address the link in the email will work.
        4. Once you have verified via the email link, try to log in with your new account. 
        5. You have now logged in.
        6. If you are trying to make a super user account you will have an extra function on your profile called product management,
           if you do not and try to use a path like '/remove/<item_id>' it will produce a toast error and stop this happening.

#### Checkout

        1. First start by picking what ever items you would like from the selection and add them/it to the basket. 
        2. Either click on the bag to checkout or the checkout link toast that appears when an item is added to continue
           onto the checkout page.
        3. Please fill out the form as normal, remember to put the correct post code for the relevant country selected.
        4. On the card number, as this is still set to a test stripe account, please use card number: 4242 4242 4242 4242 ex: 42/42 cvc: 42424
        5. Click payment, and this should then lead you to an order confirmation screen as well as sending and email to you.


## Deployment

originally during development this site was used by running it on a local server. If you wanted to run the site through Gitpod please enter the following command:

$ Python3 manage.py runserver

It is now deployed via Heroku. To view Click here [E-shop-HEROKU](https://fullstack-project-eshop.herokuapp.com/)

Both developments have had different config variable on the webhooks (STRIPE_WH_SECRET), other than that they share the same STRIPE SECRET_KEYS.
I needed to link the heroku Config vars to the S£ and IAM AWS servers in order to make a connection for the static media files.

## Credits

### Media

The background image on the front page was Designed by Freepik

### Acknowledgements

- I received inspiration for this project from sites such as topshop and H&m.