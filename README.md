Team RH iOS Technical Test 
==================================

Thank you for taking the time out of your day for the initial interview, and we 
appreciate you putting together this short take home test.

The main goal of this is to demonstrate and showcase your knowledge and skillset 
in Swift, UIKit, and well put together code. You will be creating a simple three 
screen application which displays zoo animals from an API, and a settings screen 
for the user.

The interface of the application is totally down to you. However we expect you to 
choose a sensible user interface design and implement layouts in a way that 
provides good user experience following Apple’s interface guidelines for any 
controls or views.

## Specification 
- The application must be written in Swift 5 or above. Use this to show off any 
particular areas of modern Swift you know.

- All interfaces must use UIKit. How you choose to do this (e.g xibs, 
storyboards, or in-code) is entirely your choice.

- We do not require you to write tests for this application, however if you find 
this makes development easier for you, feel free to do so.

- Please comment throughout your code to explain your reasonings or choices 
made.

- You should choose your most preferable code architect and patterns you like 
to use when developing apps. The Team RH iOS application uses MVVM, 
however if you prefer to use another approach, this is entirely your choice.

- Perform network API calls, this should use URLSession, and handle positive 
and failure paths throughout your code. We do not expect you to focus on 
the network part of your application, but the layers that communicate to your 
network code (e.g not handling status codes other than 200 and 400 is OK). 
Expect this application to be tested when offline, we do not expect you to 
handle offline storage but rather the API failed to call.

- Parse images from a URL to display, you may use a third party library for this 
to save time such as KingFisher.

- Perform conversion for height and weight. The users preference should be 
saved locally to the device and persist across sessions. How you choose to 
save this is your choice.

## The API 
In order to complete the technical test, we would like you to use a free Zoo animals 
API. The API can be found here. [https://zoo-animal-api.herokuapp.com](https://zoo-animal-api.herokuapp.com)

All data from the API is measured in imperial units:

- Animal lengths are in feet (ft.)

- Animal weights are in pounds (lbs.)
