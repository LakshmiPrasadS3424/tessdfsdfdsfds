---
layout: articles
title:  "Recurring newsletters"
categories: campaigns
---

# Recurring newsletters

A recurring newsletter is a newsletter that is sent to a certain segment of customers on a specific schedule.

## Creating a recurring newsletter

To create a recurring newsletter, simply create a new Newsletter, just as you would typically. The difference happens when you click **Launch**.

## Launching a recurring newsletter

To launch your newsletter on a recurring schedule, select the 
**Launch** option from the options menu for the draft newsletter you want to convert into a recurring newsletter:

![{{site.data.screenshots.vero.launch-newsletter['title']}}]({{site.data.screenshots.vero.launch-newsletter.image}})

The launch modal will popup.You can select the option to schedule your newsletter on a recurring schedule, presenting you with the following options:

![{{site.data.screenshots.vero.recurring-options['title']}}]({{site.data.screenshots.vero.recurring-options.image}})

You can elect to trigger your recurring newsletter on a daily, weekly or monthly schedule. At this time we do not support more or less frequent newsletters.

### Without timezone support

When scheduling a standard recurring newsletter you elect the time (in your timezone) that you wish the newsletter to be sent.

For example, you might schedule your newsletter to be sent each week on Monday at 9:00am UTC-7 (PT). This would mean that each Monday, at that time, a copy of your newsletter would be sent to the customers currently matching your segment conditions.

### Timezone support

You can also elect to send the newsletter at a certain time **in each individual customers' timezone**.

For example you might send a newsletter each day at 10:00am. This newsletter will be sent each day at this time **in the customers's timezone** wherever they are in the world. For customers with a blank `timezone` property, Vero will use your Project's default timezone to schedule the newsletter at 10:00am.

**Note** that when launching a campaign with timezone support, the first email will be sent when the time specified is first reached in the **International Dateline West timezone (GMT+13)**.

For example, if you elect to schedule an email daily at 2pm with timezone support, the first email will be sent at the next closest 2pm UTC+13. This ensures all customers are treated equally with the initial send.

## Editing a recurring newsletter

To edit a recurring newsletter, simply select its name on the *Campaigns page*. You will then be taken to the Recurring Newsletter Overview page.

On this page you can edit the actual recurring newsletter and also see the statistics for each of the instances of this newsletter, along with the exact time that they were sent.

## Re-scheduling, cancelling and pausing a recurring newsletter

On the recurring newsletter snapshot page, you can change the schedule. Simply select the new schedule you would like to use, hit save and click **Save changes** on the confirmation dialog. Note that any previously scheduled instances will not send. The newsletter will begin emailing on the new schedule immediately.

You can also elect to cancel a recurring newsletter. This will not delete the newsletter but it will ensure that it is no longer sent to your customers. You can elect to uncancel a recurring newsletter at any time, resuming it's last saved schedule.

Finally, you can choose to skip the next instance of a recurring newsletter. This means that the immediate next send will not be sent, yet the following instance will be. For example, if the next instance was to go out on a Tuesday, you could skip this instance, meaning the next instance will be sent on Wednesday.