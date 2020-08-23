---
title: User Guide
toc: true
hero: tome 1 - 0316 - Gérard Grandville.jpg
summary: A complete userguide on how to use Platy+.
visible: True
---

# Administration Interface

## Main page

The main page gives an overview of the last registered users, diverse payment and registration data displayed in charts.

## Attendees

### Attendees List

To display a list of all the created account, choose in the menu Attendees > Add an attendee.


About the different columns:

* __Registration date__ is the date on which the account has been created.

* __#__ is the user's regnumber.

* __Name__ the name of the attendee.

* __Nick__ its nickname. The nickname is not mandatory.

* __Email__. Email adress.

* __Bal__. is the payment balance: a positive balance means that the attendee owes us money. A negative one that we owe money to the attendee.

* __Reg__. if the attendee has been through the registration process, the value of that column will be Y.

### Manually add an attendee

To manually add an Attendee, choose in the menu Attendees > Add an attendee.



Fill in the different fields. Be careful to not attribute the wrong User Level (the default one is Attendee, which has no access to the Administration).



About the:

* __Registered field__. This field indicates if the user has been through the registration steps and prevents him from going through it again.

* __Custom forms__. This forms might be visible or not from the user's profile. The forms are created from Attendees > Forms .



## Download a CSV with the attendees information

To manually download a CSV with the attendees information, choose in the menu Attendees > Download CSV.

You can select if you want to download only the basic attendees information saved in the system and, if you want:

* Add to it the values entered in the custom forms.

* Or the tickets (by type or category).

## Registration configuration

You can set up the opening and closing of the registration page, add a description, activate/deactivate payment methods from the Configuration page. To access to it go to Attendees > Configuration.

### Convention

All the convention information:

* _Website_: the main website (not necessarily the registration website).

* _Convention name_

* _Registration email address_: this email will appear in all the confirmation emails sent.

* _Registration team name_: this name will appear in the emails.

* _Country_: the default country.

### Dates

Different dates can be set up:

* _Pre-registration opening_ which allows people to create accounts and go through the pre-registration steps.

* _Staff opening_ which is when the staff is allowed to go through the registration process with the Staff Code.

* _Public opening_ which is when the registration opens for everyone.

* _Force Closing_ forces the closing of the registration for people who don't have an account yet.

* _Close also for users with an account_.

* _Convention first day_ indicates when the convention starts, it allows the system to calculate if attendees will have at least 18 years at the event.

* _Staff code_ is the secret code used for the Staff Opening.

### Profile Page

You can choose which forms are displayed, if the attendee is allowed to assign his tickets, his room or to upload pictures.


### Registration Page

You can modify the text displayed on the Login Page and set the Cart Timeout (in seconds).


### Payment Methods


Screenshot of the payment methods. Note that the system will display if that method is in production or testing mode. Depending on how it has been configured.

### Invoices

All the information that are displayed on the invoices:

* _Header_: on the top left of the invoice. This usually contains the name, address and VAT number of the company.

* _Footer_: on the bottom of the invoice, address, bank account information are usually put in there.

* _Instructions_: extra payment instructions (typically if bank transfers are allowed, how much time the attendee has to pay the invoice).

## Registration

Platy+ allow a non-linear way to register. The registration process is composed of different steps that can be rearranged in different ways.

### Registration Steps

Registration steps are the element of the path that an attendee will have to follow during registration.

<!-- ### Add a registration step

WIP: add the different types of steps. -->


### Registration Process

The registration process allows to create the different paths that can be followed by the attendee during his registration. From here you organise the steps. One step can be used more than once.

It all starts from the root, a step that the attendee will not see. You can only add a new step from that point. Then…

Delete: delete that point in the path. All the next points are still preserved and just get closer to the root.

Add step: add a step just after the current step.

Branch: add a step to the right (on the same level).

(Un)mark as step: this step will appear in the breadcrumb.

The ↓ and ↕ buttons indicates if the attendee is, respectively, not allowed to go back or is allowed to go back and forth of the next step. Clicking on it will reverse the rights.

## Groups rights

Users can be assigned to different groups with specific rights on the registration system.

The rights can be found on Attendees > Groups.

<!-- ### Edit a group

WIP. -->

### Rights

Here is a summary of the different rights that can be assigned to groups.


The Super Admin has all the right.

| Name                 | System name             | Description                                                            |
|----------------------|-------------------------|------------------------------------------------------------------------|
| Admin panel access   | admin_access            | Show the admin link and give access to the admin panel.                |
| Attendees management | admin_attendees         | Allow management of the attendees.                                     |
| Rooms management     | admin_rooms             | Allow management of the rooms.                                         |
| User groups          | admin_attendees_groups  | Allow the management of the different user groups.                     |
| Check in             | admin_checkin           | Allow to use the checkin/checkout.                                     |
| Registration process | admin_registration      | Allow to edit the registration process.                                |
| Events management    | admin_events            | Allow to use the events manager.                                       |
| News                 | admin_news              | Allow possibility to edit/write/delete news                            |
| Products             | admin_products          | Allow the possibility to create/edit/delete products and their prices. |
{: .table }

## Forms

It is possible to create forms and have them displayed on the user's profile, during the registration process and also to use them internally (for example keeping track of volunteers). Groups with Registration rights have read and write access to all the forms, but it is possible to give specific rights to specific groups that don't have the Registration rights.

To access to the forms go to Attendees > Forms.

Forms can be made Visible, Hidden or Read Only for the users.

### Edit a form

Users with Registration rights can create new forms and edit/remove fields. To create a new form go to Attendees > New Form.


#### Form

This tab contains all the basic information (name and status) of the form and the different fields (called elements).

#### Rules

The rules are going to trigger actions like: display or hide another field/form.

#### Preview

The preview tab displays how the form will look like.

#### Data Access

From this tab, it is possible to assign read/write access to the form data.

### Results

Results of specific forms can be seen, edited or download as a CSV file when clicking on the "Results" button.


The results page display each entry per attendee. Clicking on "View" will result in the display of the values obtained from the form. Users with write rights can edit that values.


## Badges

Badges are automatically generated by the system, new badges are generated every 24 hours. Badges re-generation can be forced.

You can download all the badges at once, or edit a user's profile to see the badge.

### Badge editor

To access to the badge editor edit an existing badge from Attendees > Badges model or  create a new one from Attendees > New badge.

The creation of badges is scripted, there are two ways to create/edit badges templates:

* Manually writing the configuration file and uploading it to the server (requires an admin access).

* Using the badge editor.

#### Characteristics

The characteristics of the badge:

* Name.

* Background image.

* Width and height of the badge canvas.

* Background color.

#### Conditions

To know which badges must be generated for which user, the system uses "Conditions". The conditions is a set of instructions that when true will trigger the generation of a badge.

Profile, custom forms, and tickets can be used as conditions.


You can also apply conditions to the fields.

#### Fields

Fields are the elements that are going to be placed on the badge. Here is a table with the different available fields.

All the fields use x,y coordinates. The top left corner of the picture being 0.


| Name               | Values                                    | Description                              |
|--------------------|-------------------------------------------|------------------------------------------|
| Avatar             | Width/Height                              | Display the user's avatar                |
| Text               | Width/Height/Field/Font/Font size/Color   | Display a text from form/profile values  |
| Text (auto-resize) | Width/Height/Field/Font/Font size/Color   | Display a text from form/profile values. If the text box is too small, the text automatically fits in |
| Picture (form)     | Width/Height/Field                        | Display a picture uploaded via the form  |
| Picture (uploaded) | Width/Height/Field/Uploaded               | Display a custom picture.                |
{: .table }

#### Download badges

To download the generated badges go to Attendees > Download Badges.


Before choosing the model to download, you can force the generation of all the badges of a specific model by pressing Force (re)generation. The forced (re)generation might take a while, do not close your browser in the meantime.


The badges are download in a zip archive.

## Documents models

Documents models are documents generated on the fly, for example a pre-filled waiver. To access to the models go to Attendees > Document model. To create a new one go to Attendees > New model

The generated documents are visible when you edit the user's profile (in the Documents tab) or during checkin.


Documents can use conditions to be generated in specific cases only.


You can use markdown, html and special tags for the text.


#### Preview

You can preview the document by clicking on the Preview button when you are in the Documents list. It uses then your personal data to fill in the tags.

# Booking

## Booking and Tickets

This page displays all the different categories of tickets created on the system. To display it, go to Booking > Bookings and Tickets.

For the Rooms and the Seats, you can click on them and see the placement of the different spots.



The meaning of the different columns are:

* _Name_. The name of the ticket.

* _Places_. The size of the room.

* _Total_. The total number of tickets of that kind (for bedrooms, divide the Total by Place to get the number of rooms).

* _Unassigned_. Spots taken from the pool of available spots, who have no attendee (regnumber) assigned to it.

* _Open (used/available)_. Spots with an assigned attendee, booked in the available pool of spots.

* _Canceled (used/total canceled)_. Canceled spots. Cannot be seen by the attendee from his profile

* _Hidden (used/total hidden)_. Hidden spots. Cannot be seen by the attendee from his profile



### Unassigned spots

From that page you can also see the spots who have not been assigned to an attendee.

### Download a CSV with the bookings

This allows you to download a complete list of the bookings. It contains all the different spots taken, and also contains information like: who took it rm_regnumber - rm stands for regmaster - and who is assigned to it.

Here is the list of information you will get from it:

* _Room_: room number if applicable (Room or Seat ticket).

* _Regnumber_: registration number of the attendee to which that spot has been assigned to.

* _Rm_regnumber_: the registration number of the attendee that owns the spot (in most cases the one who bought the spot).

* _Rbid_: internal unique id for that spot.

* _Pack_: the spots with the same pack number are grouped. This allows to quickly set the same regnumber for all the spots with the same pack number and rbid.

* _Type_: category of ticket (Room, Seat, Ticket or Goodie)

* _Name_: name of the ticket

* _Accepted_: indicates if the attendee that the master has assigned accepted (Y: yes; N: No).

* _Oid_: Order ID, the unique identifier for the invoice/quote to which that spot is linked to.

* _Checkin_: the check in state for that spot (I: checked in, N: not checked in yet or O: checked out).

* _Attributed to_: The attendee assigned to that spot.

* _Email_: his email address.

* _Owner_: The master/owner of that most.

* _Owner email_: his email address.



<!---## Rooms

### Manage Rooms

This page allows you to see all the rooms saved in the system, and to add, edit or delete rooms.

WIP

### Add a Room

WIP


## Goodies and Tickets

### Manage goodies and Tickets

WIP

### Add Goodies and Tickets

WIP-->



# Orders

The orders are all the quotes and invoices stored on the system, an order is created automatically when the attendee lands on the checkout page or manually from the Attendee edition interface or directly from Orders > New order.

For legal reasons, orders can not be deleted.

## Orders

<!-- ### New order

WIP -->

### Download CSV

Download a CSV file containing all the main information about all the created orders:

* Oid: an unique identifier for the quote.

* Paid: the amount paid for that quote.

* Total: the total without vat for the quote.

* Total_vat: the total with the VAT included.

* Name: the name of the debtor.

* Date: date of creation of the quote or invoice

* State: the state of the order:

  * quote.

  * quote_auto: an automatically generated quote

  * invoice.

  * deleted_quote: a quote that has been deleted.

* Invoice: the unique invoice number (if the order is an invoice)

* Generated: Y if a pdf has been generated.

* x% exc: the sum on which the x% VAT rate will apply.

* x% inc: the sum on which the x% VAT rate has been applied.

## Transactions

Transactions represent announcements of payments, payments and refunds.

### Download CSV

Download all the transactions in a CSV file.

# Events

There is an in-build event manager. Events can be displayed on the website, the dedicated page in Platy+, on the app, the kiosk screens…

The attendee can also create his own personalized schedule by picking up the events he is going to attend. This allows some rough estimation of the attendance/interest for the event.


<!-- ###  Schedule an event

WIP

### Add an event

WIP

### Edit an event

WIP

### Add a localisation

WIP

### Edit a localisation

WIP -->

## News

Platy+ includes an internationalised news system. It is also useful to transmit important but not critical information to the app.


News have:

* _A title_.

* _Text_.

* _Creation date_ (common between the different translations).

* _State_:

  * _Draft_: the news exists in the system but is not ready to be displayed on the website

  * _Waiting for Preview_: the news is not displayed on the website, and is waiting to be proofread.

  * _Published_: the news is displayed on the website.

* _Languages_:

  * The language in which to publish the post.

### Add a piece of news

To create a new post, just go in News > Add a post.

The default language is already selected, but you can change it for whichever other languages you want to write the news in. Only the posts written for the selected languages will be displayed.


<!-- ### Edit a piece of news

WIP -->

## Mass Emails

It is possible to schedule emails sendings. The system uses conditions and the groups to limit which users should get the mails


__Warning: do not use it for advertising, unless the users have given their consent (RGPD).__


### Sending an email

To schedule a mail for mass sending, you will have to go to News > Mass Emailing.

From there a wizard will guide you step by step to schedule the mail.


If no group is selected, then everyone will receive the mail.

It is the same for the conditions, if none is chosen, there will be no filter from there.


As for the documents, you can use html, tags and markdown.


Note: the schedule date is in the following format YYYY-MM-DD (with YYYY being the year, MM the month and DD the days all in numerical form).

### Email sending conditions


Conditions configuration can be created and saved to be used and reused for each time mails have to be sent. It can be accessed from News > Conditions, and can be created from News > New conditions

The conditions can use the profile data, tickets and forms in order to decide whether or not to send an email to a specific user.


### Email models

Email Models are templates for the emails, they can be used as a way to emphasize the content or just make it look nicer.


Existing models are available through News > Models, and can be created from News > New model.


As for the documents, you can use html, tags and markdown.

### Scheduled mails

It is possible to see the scheduled mails, and to cancel them or reset them. Go to News > Scheduled mails.


The page provide an overview of the sending date, the conditions used, the groups to which to mail it, the model used and the state.

The different possible states are:

* Idle: the mail sending has been scheduled, and will be sent on the requested day when * the mail sending job will be running (normally around 3:00 in the morning).

* Cancelled: the mail sending has been cancelled.

* Done: the mails have successfully been sent.

* Error: an error happened while sending the mails.


Deleting will end up in definitely removing the mail from the schedule.


Clicking on the mail name will give you more information about that scheduled mail: a preview, sending date, conditions… and the users to which the emails have been sent.



This will help you to diagnose if the conditions were working correctly.

## System

### Updates

Platy+ can be updated from System > Update. For the moment the files have to be updated manually.

### Maintenance modes

The system can display a maintenance page separately for the website part, the registration part or for both. This can be accessed from System > Maintenance.

In the screenshot, all the maintenance modes are deactivated.

### Version

The page provides miscellaneous information about the registration system (version, changelog, licenses…).

### Translations

It is possible to provide translations for dynamic fields. Normally, the translations it is already accessible from the edition interfaces of the events, products, etc. But it is possible to find all the translations through System > Localize.

# Attendee's interface

The administrators and registration staff should get used to the attendee's interface in order to provide them quick assistance.

Here are the different functionalities the user has access to:

* Custom forms from the profile.

* Convention schedule and custom schedule.

* Stats.

* Attendees list.

## Profile

### Changing password

The attendee can reset his password from the login page.

Or he can change it from his profile

### Double authentication

The attendee can activate double authentication from his profile. He will need for that an app like Google Authenticator.

# How to

This part contains quick tutorials on more or less advanced uses of certain functionalities.

<!-- WIP -->

## Attendees

### Cancel an invoice

For legal reasons you can't delete an already generated invoice, you will have then to create a negative invoice.

* If you know the Order number or the Invoice number:

  * Directly go to Orders > Orders and from there click on the invoice you want to cancel.

* If you don't know the number, but you know the user's regnumber. You can access to it from the user's edition page.

  * Go to Attendees > Attendees list.

  * Find the user and edit it.

  * Go on the Orders tab

Once you are on the order you want to cancel, you can just hit the "remove" button for each line of the invoice (if you want to partially cancel an invoice, you hust have to hit the "remove" button for the specific lines you want to cancel).

It will look like you are creating a new quote.

Once you are done removing the products, hit the "Save and create a new quote" button on the top left of the page.

From here you have quote cancelling the invoice. As it is a quote, you can still edit it (add/remove products).

Once you have obtained what you wanted, you can hit the "Generate Invoice" button.

Don't forget to remove manually the bookings and tickets that you cancelled.

Go back to the user's edition page (you can click on his regnumber).

Then go to the Ticket & Bookings tab.

For the payments and reimbursements, check with your head of registration on how to proceed.

### Create a user

For on site registration, guests or for users having trouble you can directly create a new user.

Go to Attendees > Add a User.

### Generate a quote

For products that are not accessible through the registration steps or for users who have troubles you can manually generate a quote.

The user will see the quote from his Profile panel. Once he initiates payment, it is turned into an invoice.

Check on the user's profile in the "Bookings and tickets" tab if everything has been set correctly.

### Manually create an invoice

See first "Generate a quote".

Once a quote is created, you can generate an invoice.

### Delete a user

While it is very straightforward, some points should be carefully be taken into account.

* Has the user an unpaid invoice?

  * Maybe cancel the invoices, and check that the user payment balance is what it is expected to be.

* Has the user still bookings/goodies/etc?

  * You should remove any items that the user is never going to claim before deleting the user.

  * Also if a badge has been sent for printing don't forget to remove it from the batch.



The steps are:

* Go to Attendees > Attendees list.

* Look for the user for which you want to delete the account. And edit that user

* After all the verifications have been done go to the Delete Tab. Check "Delete the user" and hit "Delete".

What data is there left?

* The user's invoices and quotes are kept for legal reasons.

<!-- ## Products

### Add a new product

WIP. -->

# During the event

This chapter provides clues and information on how to set up the registration desk during the convention/event. And also how to prepare it properly to circumvent usual issues (fallbacks), and how to answer to more rare cases

## Tech set up

### Setup the local WiFi/Ethernet network

* Setup our network with our own routers. A local webserver should be running a copy of the website and ready to run in case of Internet connection failure (throught the hotel network or our 3G/4G backups).

### Setup the registration desks

* Laptops/Desktop computers connected to the hotel network and capable to reach our internal network.

* Check connection to the shared printer.

* Check connection with the badge printer.

* If applicable, test the QR/barcode code reader.

  * If it is not function try to install the drivers/restart the computer.

  * If QR/barcode code reader is out of use, do not worry the registration staff can manually enter the ticket code or find the attendee.

* Let members of the registration team (and ConOps if they will server as backup) have a hand first on the check in. Check if everything goes well.

## Troubleshooting

Note: in some case, it might be wise to make an inventory at the end of the day of the keys/goodies/tickets that have been handled to the attendees.

### There is no Internet Access

* Communicate to the staff the lack of Internet Access and the team is working on it.

* For the registration switch to the local web server until the end of the day.

  * The Registration Team has a special procedure to follow.

* Try to troubleshoot the connections issues.

* If everything is fixed, and after the online web server has been updated:

  * __Make a copy of the local web server database.__

  * Replace the database with the online web server copy.

  * Communicate to the other teams the problems are fixed.

### The local web server dies/the WiFi/Ethernet connection fails

* Ask the registration team to continue to register on the individual desktops through local files.

  * The Registration Team has a special procedure to follow in that case.

* Make a copy of each file on each desktop.

* Help the registration team  to pool the data.

### All the registration computers fail

* Communicate with the registration team, tell them to switch back to paper and pens.

* The Registration Team has a special procedure to follow in that case.

## On site registration desk

### Tips

One-two month before the convention:

* Commission the badge designs (don't forget to commission different design according to the tier of the attendee: Super-sponsor, sponsor, regular).

* Order the sponsor gifts, lanyards, and bags

Two weeks before the convention:

* Send the list of attendees to the hotel, with the booked rooms and the allergies.

### Before the convention.

* Print the badges.

* Cut the holes in the badges.

* Order the badges by regnumber, separate each 10 badges with an index.

* Prepare different set of bags.

  -  Normal:

    * A lanyard.

    * An erratum in case some of the information in the conbook incorrect..

    * The conbook.

  - Sponsor

    * Same as normal plus sponsor gift.

  - Do not put the shirts in the bags, keep them separated by size.

Save a CSV/ODS copy, print a paper copy of the Attendees. The copy should contain:

* The regnumber.

* The first and last name.

* The nickname.

* Ticket types. (which days, and which bedroom).

### During the convention

Estimated time: 1h.

Set up the Pre-registered desk.

There should be 1 pre-registered desk per 80/120 attendees.

Version 1.a:

* The bags must be behind the desks.

* A sufficient number of liability waivers for the point a.

* A computer with an Internet connection (and an electronic copy and paper copy of the attendees list in case of internet failure) at the point b.

  - One person who checks the liablity waivers were correctly filled in.

  - One person doing the check in on the computer/printed documents.

  - One giving the badge. An extra person can handle the badges for one to three desks.

  - One person who handles the gifts and stuffed badges.



Version 1..b:

* The bags, gifts and shirts must be behind the desks.

* A printer (one/per three desks) that prints the liability waivers when someone registers.

* A computer with Internet connection (and an electronic copy and paper copy of the attendees list in case of Internet failure) at the point a.

  - One person who checks in and starts the printing of the waivers.

  - One person who gets the papers and the bags.

  - One person who handles the gifts and stuffed bags.

NB: be able to switch to version 1.a in case of issues with the printed liability waivers (have a buffer of 10% of waivers printed, have material to print the new ones).


Set up the Non-registered desk

There should be a desk put apart for people who didn't bought the badge or in case of issues with the registration:

* A computer with internet connection.

* A badge printer.

* A regular printer.

* An electronic payment point/cash box.


Registered attendees:

* Attendees should move into a unique flow:

  * Liability waiver: the attendee should sign it first.

  * ID check and badge distribution: check the ID card (name and birthday).

  * Convention package.

  * T-shirt

  * Room key (if relevant).



Non registered attendees

* They can go directly to the non-registered desk.

* Buy a ticket there, sign the liability waiver and get a badge.

* Once registered, they can get back into the registered attendees line.

### Closing of the registration

* Be careful that everything is packed and ordered correctly. Download a local copy of the attendees and/or make an offline backup of the attendees list.

* Check there are enough liability waivers.

* If the room can be closed by a key, leave the computers and the stuff in the room. Close correctly the room.

* Count the money, write and date the last count. Bring the money to the accountant.

### Reopening

1 hour before:

* Check if there are new badges to print.

* Print the badges, prepare the packages.

* Do as during the opening.

## Troubleshooting

While Platy+ is getting used by more and more events, some bugs can happen and quick and proper answers should be brought to that situations to avoid data loss and attendees from waiting for too long.

But the greatest risks are external issues (no Internet connection, server not reachable, etc). You will also find here answers to that situation.
