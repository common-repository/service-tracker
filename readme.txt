=== Service Tracker ===
Contributors: bucklit
Donate link: https://bucklit.com.au/products/service-tracker/
Tags: mobile application, manage services, service, jobs, technician, work, status
Requires at least: 4.7
Tested up to: 5.8
Stable tag: 1.0.0
Requires PHP: 7.0
License: GPLv2 or later
License URI: https://www.gnu.org/licenses/gpl-2.0.html

A simple plugin and mobile application designed for business or organisations to add service requests, link the work to a customer, assign a worker or technician , set a booking time and finally update status on job progress. 

== Description ==

Service Tracker is a simple "plugin" and "mobile application" designed for business or organisations to add service requests, link the work to a customer, assign a worker or technician , set a booking time and finally update status on job progress. 


After activation of the plugin, you'll find Services on the WordPress admin screen menu. The services or jobs can be added in the admin. With Service Tracker, you are no longer need to manually manage the jobs assigned to staffs, technicians or workers. This tool allows their employees to add a job or work, link the work to a customer, assign a worker or technician , set a booking time and finally update status on job progress. 

= All features =

WP Admin or Manager will be able to:

* Add Service Requests (it can anything related to job or work)
* Add and select the customer who requested the work and assign a job to a suitable worker.
* Select a date and time the job has to be completed.
* The worker can keep track of the works assigned to them and update the status + add additional notes about the work.
* Under Users> Add new user. Plugin adds a new role 'technician'. So when a user is created select role 'technician' for the worker and 'subscriber' for the customer. 
* That's it. Now you can add a service, select a customer, assign it to the technician, select date and time of the work, update the service or work status.

== Mobile Application == 

= Prerequisites =

Mobile application requires [JWT Authentication](https://wordpress.org/plugins/jwt-authentication-for-wp-rest-api/)
 for WP-API WordPress Plugin to be installed in your website.

= Configuration in wp-config.php =

* The JWT requires a secret key - define('JWT_AUTH_SECRET_KEY', 'SECRET KEY') (the secret key can be generated here at https://api.wordpress.org/secret-key/1.1/salt/)

* Add the above code in wp-config.php


= Configure CORS support in wp-config.php =
define('JWT_AUTH_CORS_ENABLE', true);

= Test if configuration is working = 

Use Postman or any REST CLIENT to test 

* JWT AUTH URL is working <YOUR-WEBSITE-URL>/wp-json/jwt-auth/v1/token (POST)
* SERVICES REST API is working <YOUR-WEBSITE-URL>/wp-json/wp/v2/services/

= Install the Mobile Application =

[Available in the Google Play Store](https://play.google.com/store/apps/details?id=com.bucklit.servicetracker)


The application is ready to use on Android Phone. For iPhone application or any type of customisation, feel free to [email us](info@bucklit.com.au).

= Mobile application usage =

* Install application on your Phone
* Application loads with Spalsh screen and redirects to Login screen
* In order to login and access services type Website URL- <YOUR-WEBSITE-URL>, Customer or Technician login details.
* On successful login, user is redirected to DashBoard screen. Click Services to access the services.
* The Services is a list of services with Service Title, Service Booking Date and Time & Status. 
* When a service is clicked, user is redirected to Service Details Screen, with service, customer and technicain details.
* Technician or Customer can change the service status and post additional comments.
* The comments posted is viewable to administrator or manager only. The history of comments are saved.


For more detailed information, please refer to the page [contact us](https://bucklit.com.au/products/service-tracker/).

= Installation Video =

[youtube https://youtu.be/bSj5gJ6aW9I]

= Configuration and Working Video =

[youtube https://youtu.be/hjSnbAEHg58]


== Installation ==

Below are the steps to install and configure the plugin:
1. Login to Wp Admin
2. Go to Plugins > Add New
3. Upload plugin `service-tracker.zip`, install and Activate.


FTP
1. Upload the entire `service-tracker` folder to the `/wp-content/plugins/` directory.
2. Activate the plugin through the 'Plugins' menu in WordPress.


== Screenshots ==
1. User Listing- Adding a Technician
2. User Page - Adding a Technician or Customer
3. Services Listing - List of Services
4. Service Details Page - Service Title and Description
5. Service Details Page - Service related form fields
6. Mobile Application - Splash Screen
7. Mobile Application - Login Screen
8. Mobile Application - Dashboard Screen
9. Mobile Application - Services Screen
10. Mobile Application - Service Details Screen - Update Status and Comments
11. Mobile Application - Splash Screens

== Frequently Asked Questions ==

= 1.Which role should I select when adding a new user as technician or customer? =
For Technician select 'Technician' and for customer select 'subscriber'.

= 2. Who can change Service Additional notes? =
Currently, the additional notes is meant for administrator/manager or even technician given the website allows technician to login.
We are working on a Mobile Appliacation, this will allow both technician and customer to post comunication/status.
 


== Changelog ==

== Upgrade Notice ==