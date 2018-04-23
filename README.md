# FirebaseNotification

#What are push notifications?
A push notification is a message that pops up on a mobile device. App publishers can send them at any time; users don't have to be in the app or using their devices to receive them. They can do a lot of things; for example, they can show the latest sports scores, get a user to take an action, such as downloading a coupon, or let a user know about an event, such as a flash sale.
Push notifications looks like SMS messages and mobile alerts, but they only reach users who have installed your app. Each mobile platform has support for push notifications — iOS, Android, Windows and BlackBerry all have their own services.
Why are they used?
Push notifications provide convenience and value to app users. For example, users can receive:
-	Sports scores and news right on their lock screen
-	Utility messages like traffic, weather and ski snow reports
-	Flight check in, change, and connection information
For app publishers, push notifications are a way to speak directly to a user. They don't get caught in spam filters, or forgotten in an inbox — click-through rates can be twice as high as email. They can also remind users to use an app, whether the app is open or not. They can also be used to drive actions, such as:
-	Promoting products or offers to increase sales.
-	Sending transactional receipts.

#How do push notifications appear to users?
Mainly, users see a notification as a banner or pop-up alert as they are using their phone. This alert is shown no matter what the user is doing.
Most mobile operating systems also show push notifications together in a single view. On iOS, Apple has a Notification Center. The Notification Center is organized in chronological order, and users get to the Notification Center by swiping down from the top of the screen. Android devices show unread messages on the lock screen.
iOS lets users customize push notifications at an individual app level. Users can turn sounds on or off, and pick the style that iOS uses to show a notification. Users can also control the red "badge" showing the number of unread notifications on an app's homescreen icon. Android uses a standard banner approach that users cannot change at an OS level.

Users can choose to mute notifications from specific apps, and with the Android 8.0.0(Oreo) notifications has to be “streamed” through channels, this is to enable the user to manage his/her incoming notifications. 
Offers, sales or any promoting of the app won’t be shown to the user, therefore most apps, doesn’t settle with just notifications, beneath is explained the alternative options to Push notifications.   
Your Push-Less Strategy
Admittedly, push notifications are unique. They flash on the device’s screen the moment they’re received, so they’re perfect for announcing anything that requires immediate action, as mentioned above. Some alternatives to push notifications: 
-	Email, like push, is delivered outside of your app or website. It can grab attention from users who wouldn’t have opened your app in the next short span of time, but not many check their email as often as the phone. Some mails do end up in the Spam filter as well.
-	Like push, in-app and in-browser messages vanish quickly, but the content can be long and visually complex like an email.
-	News feed cards within your app or site’s message center, so they’re great for richer and more valuable content. Plus, unlike any of the other channels, you control how long they remain viewable.

#Use Emails With Urgent Subject Lines
If a customer is on your email list, craft an urgent subject line (“Our special offer ends soon. Hurry!”). When the email lands in the user’s inbox, depending on their settings, their smartphone may buzz or generate a notification, achieving the same immediacy as push. At the very least, you’ll get the user’s eye the next time they scan their inbox. Don’t forget, though, that emails are great for delivering rich content. Do use the subject line to grab attention with short and direct copy about your timely message, and then make sure the rest of the email offers value that brings the user to your website or app.
Once the user has opened your app, you can deep link directly to the content (news, sales, or other promotion) you want them to see. You can also send them to an in-app message or News Feed Card that expands on your message or provides more valuable information.
Take A Multichannel Approach
What if the customer isn’t on your company’s email list? Fortunately, targeted News Feed Cards offer another great way to send an alert-like message. News Feed Cards trigger an inbox-like number within the app, alerting app users that a new message awaits. Of course, only customers who open your app will see this message, so when you can’t pair it with push or email, for users who aren’t on either list, other methods such as retargeting and social media can be used to bring users back to the app.

Push is one of the strongest way to encourage users to use your app, the alternatives is there, but if combined a lot better. If you use email along with push notifications, you target a broader segment and encourage your users to enable notifications.
 
#One demo app to rule them all
Creating push notifications is getting easier for every day, Google acquired Firebase and quickly enabled Firebase Messaging with Android Studio, I intend to use Firebase Cloud Message to send my push notification to my users.

Android Studio with firebase is godlike – both managed by Google, meaning that Android Studio has an easy setup – walkthrough guide where the most is done by the IDE itself.

#What it does for you is:
In the manifest, id adds A service that extends FirebaseMessagingService:
<action android:name="com.google.firebase.MESSAGING_EVENT"/>
This is needed to To receive notifications in foregrounded apps, to receive data payload, to send upstream messages, and so on, you must extend this service.
It also adds the dependency:  
compile 'com.google.firebase:firebase-messaging:15.0.0'

I created an java class: FirebaseMessagingService, within the class I the following functions:
onMessageReceived()
onDeletedMessages(), not used though.
sendNotifications(), this was added because I wanted to do more than just send notifications from firebase console, so I added some extra features such as allowing users to login, authenticate and send notifications to each other, I didn’t get to implement the later. 

But to enable push notifications is rather easy with Android Studio!
 

#How it’s done
Visit: https://www.firebase.google.com
Sign in to the console: https://console.firebase.google.com
Choose the project you set up to work with your android app.
Choose “Cloud Messaging” from the left menu bar.
Press “New Message” and enter an message text.
When done, choose the app (usually it’s the package name of the app)
And enjoy your OP push notification


#Conclusion / Reflection
Push notifications are a must with all apps, some more than others, but to enable communication without having the user to have the app open, is a strong communication tool for app developers.
Use it to some extent, too much will lead the user to uninstall the app or mute the app. 


