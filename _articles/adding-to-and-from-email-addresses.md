---
layout: articles
title:  "Adding TO and FROM email addresses"
categories: "email design"
---
  
##Adding "To" and "From" email addresses?
    
In your Vero [Account](https://app.getvero.com/account) settings you can manage the [email addresses](https://app.getvero.com/account/email_addresses) that your emails are sent TO or FROM.

 
##Adding an email address
   When adding an email address there are three fields:
 
- Email: The email address. 
e.g. chris@getvero.com
	
- From name: The name you want the email to come from. 
e.g. Chris from Vero
	
- Reply-to (optional): The email address you want the replies to go to. 
e.g. support@getvero.com

##Complex / dynamic addresses:
You may want to email your customers based on other actions (events). To do this you could store a 'related_customer_email' property with an event or on a customer profile. 
This would use the Liquid syntax language such as {{user.related_user_email}} or {{event.related_user_email}}.
 
You can create an email address using this data. You might set the **Email** field to be {{user.related_user_email}} and the 
**From name** to be {{user.related_user_name}}. When the email goes out, Vero will pick up these values and use them.

##Using an email address
Once saved you can use an email address when creating a new campaign.

Here's an example of a dynamic email address as setup in your `Settings`:

![](https://s3.amazonaws.com/helpjuice_production/uploads/upload/image/742/3318/Screen_Shot_2014-01-28_at_12.42.21_pm.png)
You can then select the email as a 'To' or 'From' address when creating an 
**automated**
 campaign:
![](https://s3.amazonaws.com/helpjuice_production/uploads/upload/image/742/3319/Screen_Shot_2014-01-28_at_12.45.56_pm.png)
Ensure you track the required payload data with the base event:
![](https://s3.amazonaws.com/helpjuice_production/uploads/upload/image/742/3320/Screen_Shot_2014-01-28_at_12.45.04_pm.png)
 

                
                
