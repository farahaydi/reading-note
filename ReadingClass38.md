# What are the three criteria an acticity’s intent filter must fulfill in order for a system to send an intent to that activity?
An activity's intent filter must meet three criteria for the system to send an intent to that activity:

Action:

Specify the action to perform, like ACTION_SEND, using <action>.
Data:

Describe the associated data, using <data> with attributes like MIME type or URI.
Category:

Characterize the activity, often with CATEGORY_DEFAULT, using <category>.

# How does an activity retrieve the Intent that it was started by?
An activity retrieves the Intent that started it by calling the getIntent() method. 
This method is part of the Android Activity class and allows the activity to obtain the Intent object that was used to start it.
Typically, this is done during the early callbacks of the activity's lifecycle, such as onCreate() or onStart().

# Explain intents to a non-technical friend.
let's imagine your phone is like a city, and your apps are different buildings with specific purposes. Intents are like messages that these buildings can send to each other.

So, let's say you're in a photo app (like a photo building), and you want to share a picture with a friend through a messaging app (like a messaging building). You don't need to leave the photo app and go to the messaging app; instead, you send a special kind of message called an "intent." 
This message says, "Hey, I have a picture, and I want to share it!"

The messaging app has a special system to understand these messages (this is like the messaging building having a mailroom). 
When it receives your message (intent), it knows how to open and show the picture you sent. This way, you can easily connect different buildings (apps) without having to go back and forth all the time.

# Compare and contrast implicit and explicit intents.
Implicit Intents:

What: General action without specifying a particular app component.
How: System dynamically decides which app or component should handle the intent based on intent filters.
Example: Sharing content with any app that can handle sharing.
Explicit Intents:

What: Specifies the exact app component (activity or service) to be started.
How: App knows the component's name at compile-time; no dynamic resolution.
Example: Starting a specific feature or service within the same app.
Comparison:

Implicit: Flexible but less control; system decides.
Explicit: More control and security; app decides.
Use Case: Implicit for generic actions; explicit for specific tasks within the app.

# What is the primary information contained within an Intent?


The primary information contained within an Intent includes:

Component Name:

Specifies the name of the component (activity or service) to start.
Makes the intent explicit, ensuring it is delivered to a specific app component.
Action:

A string specifying the generic action to perform (e.g., view or send).
Defines the purpose of the intent, guiding the recipient on what action to take.
Data:

Represents the URI (Uniform Resource Identifier) of the data to be acted upon.
Specifies the type of data using a MIME type, helping the system find the best component to handle the intent.
Category:

A string providing additional information about the kind of component that should handle the intent.
Categorizes the intent, influencing how the system resolves and delivers it.
These components collectively define the characteristics of an intent, guiding the Android system on which app component to start and how to perform the specified action. Additionally, an intent may contain:

Extras:

Key-value pairs carrying additional information required to accomplish the requested action.
Used to provide extra data needed by the recipient component.
Flags:

Metadata that instructs the Android system on how to launch and treat the intent after launch.
Guides the behavior of the system when handling the intent.

