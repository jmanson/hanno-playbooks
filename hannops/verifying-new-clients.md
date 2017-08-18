# Verifying New Clients

How to complete the simple checks, verifications and billing for new clients

To send invoices to clients, we have to make sure they've been added into our system correctly. This is part of our [Invoices](hannops/invoices.md) workflow.

## Get their details

We automatically add new clients into the system as soon as they complete our business details form. Once they complete this form, they'll be added to Xero by Zapier, and will show up on our [Contacts Page](https://go.xero.com/Contacts/Search.aspx).

For any new client, you should check in Google Drive.
```
Hanno Team > Pitching > New Client Details
```

If they're not inside our contacts already (it's always worth checking this):

1. __If they've filled out the New Client Details form already__, go to the __Responses__ spreadsheet and get the details from here. You shouldn't actually need to do this--if their details are in the spreadsheet, they should also be in Xero. But maybe the Zapier integration failed when they filled out the form.
2. __If they're not, send them the New Client Details form__. When you're inside that form, there's a button in the navigation to __View live form__. That's the one you need to share. This URL is also in Asana.
Okay, so the client should now be in Xero.


## Check and correct their Contact Information and Financial Details

Once we have these details in Xero, there are usually a few tweaks that we need to make, so that invoicing is set up correctly.

#### Load up the new client

Head to [Contacts > All Contacts](https://go.xero.com/Contacts/Search.aspx). You'll see the list of all of our clients and suppliers. Do a quick search to find the client that has been added:

![validation1](https://www.datocms-assets.com/1058/1495450917-validation1.png?w=1000&fit=max)

Click on their name, to open them up. Then click on the Edit button:

![validation2](https://www.datocms-assets.com/1058/1495450919-validation2.png?w=1000&fit=max)

#### Set their Contact Information

You'll need to inspect the contact details. This is usually quite simple, and they tend to be correct. Just watch out for obvious mistakes.

![validation3](https://www.datocms-assets.com/1058/1495451004-validation3.png?w=1000&fit=max)


### Consider adding an extra contact person

One thing which is worth doing is adding additional contacts to the client. The client will have entered a billing email, which is what will be added here, but if this is a bigger company, that might not be the same email address as our product owner. For example, a __billing@clientcompany.com__ address. It's pretty simple to add extra contacts, though:

![validation4](https://www.datocms-assets.com/1058/1495451023-validation4.png?w=1000&fit=max)

### Set their Financial Details: Default Account Settings

Scroll down a little, until you reach the __Financial Details__ section. We need to set up a few standard settings:

* __For Sales__: __Default tax__ should always be set to Amounts are tax exclusive
* __For Sales__: __Default account__ should always be 200 - Sales
* __For Purchases__ can be left unchanged (it doesn't apply to people we're selling to)

![validation5](https://www.datocms-assets.com/1058/1495451049-validation5.png?w=1000&fit=max)

### Set their Financial Details: VAT

This is trickier and needs to be done correctly. If you have even a tiny bit of uncertainty, please ask for help!

####  UK clients

All UK clients are treated in the same way. It doesn't matter if they're VAT registered, or not:

- EU Country should be United Kingdom
- VAT Number can be filled in if you have it, but it's completely fine to leave it blank
- Sales VAT must be 20% (VAT on Income)
- Purchases VAT can be blank

![validation6](https://www.datocms-assets.com/1058/1495451084-validation6.png?w=1000&fit=max)

#### EU clients

The way we invoice EU clients depends on whether they have a valid VAT registration or not.

__If they don't have a valid EU VAT number__
Then just use the same details as we did for UK clients, a second ago. Obviously, set the EU Country field to match their location.

__If they've given us a VAT number__
If they're in the EU and give us a valid VAT number, then they'll be invoiced at 0% VAT. But we have to ensure that the VAT number they give us in the company details form is correct, and matches the company name they give us, otherwise, we might be liable to pay the VAT ourselves.

To verify the VAT number:

1. Visit the [VIES validator](http://ec.europa.eu/taxation_customs/vies/)
2. Enter the details they've given us into the __Member State__ fields.
3. Enter our details into the __Requester Member State__ section. Our VAT number is __GB140908328__ and the requester state is of course, __GB-United Kingdom__.

If the details match, and VIES approves things--perfect! We can remove the VAT from their invoices. So for this client:

- __EU Country__ should be their country (the same one you entered into VIES)
- __VAT Number__ must be filled in, including the country code. So it'll be something like FR12345678
- __Sales VAT__ must be Zero Rated EC Services
- __Purchases VAT__ can be blank.

![validation7](https://www.datocms-assets.com/1058/1495451147-validation7.png?w=1000&fit=max)


#### Clients from outside the EU

This is simple--we don't charge them VAT.

- EU Country should be blank.
- VAT Number should be blank.
- Sales VAT must be No VAT
- Purchases VAT can be blank.

![validation8](https://www.datocms-assets.com/1058/1495451197-validation8.png?w=1000&fit=max)

### Set their Financial Details: Invoice Settings

#### Invoice Settings: Default branding theme

There are 3 routes here. The one we pick, determined what invoice template we use:

1. If they're in the UK, we will always get paid with a direct bank transfer.
2. If they're outside of the UK, particularly in the US, we get them to pay using Stripe (even though we get charged fees on this).
3. If they have issues using Stripe (some clients had problems with their cards being declined due to maxing out limits), or we're doing a major amount of work with them and come to a specific agreement, we might decide to get them to pay via bank transfer.

So there are 2 _Default Branding Themes_ (invoice templates) in the system:

1. __Default Branding Theme: Bank transfer only__: this is what we use for UK clients, and anyone paying by bank transfer. It just has our bank account details shown on it, and they make a regular transaction.
2. __Default Branding Theme: Online payment enabled__: these invoices will come with Stripe links on them, and the notification email will also have Stripe details on it.

When setting up the client, we pick the most appropriate option for them.

#### Sales Invoices Default Due Date

This is pretty simple. All clients are invoiced at __net-14__, which means that the due date of the invoice is 14 days after we send it.

- Set Sales Invoices Default Due Date to be due __14 day(s) after the invoice date__

#### Invoice Settings examples

So a UK client will usually look like this:

![validation9](https://www.datocms-assets.com/1058/1495451237-validation9.png?w=1000&fit=max)

And a US/EU client will look like this:
![validation10](https://www.datocms-assets.com/1058/1495451257-validation10.png?w=1000&fit=max)
