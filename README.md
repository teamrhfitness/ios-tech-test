Team RH iOS Technical Test 
==================================

Thank you for taking the time out of your day for the initial interview, and we appreciate you putting together this short take-home test.

You will be creating a simple three-screen application which displays zoo animals from an API, and a settings screen for the user.

You should choose your most preferable code architecture, patterns and any libraries you like to use when developing apps (if any). The main goal of this is to demonstrate and showcase your knowledge of clean code architecture and iOS-specific design guidelines. The interface of the application is totally down to you. However, we expect you to choose a sensible user interface design and implement layouts in a way that provides a good user experience following Apple’s interface guidelines for any controls or views.

## Specification 

- The application must be written in Swift 5 or above. Use this to show off any particular areas of modern Swift you know.
- All interfaces must use either SwiftUI (preferred) or UIKit.
- Please comment throughout your code to explain your reasonings or choices made.
- If you have experience with the Combine framework we would encourage you to use it, however, this is entirely optional.
- Perform network API calls, this should use URLSession, and handle positive and failure paths throughout your code. 
- Parse images from a URL to display, you may use a third-party library for this to save time.
- Perform conversion for height and weight. The user's preference should be saved locally to the device and persist across sessions. How you choose to save this is your choice.

## The API 

To complete the technical test, we would like you to use a free Zoo animals API. The API can be found here: [https://zoo-animal-api.herokuapp.com](https://zoo-animal-api.herokuapp.com)

All data from the API is measured in imperial units:
* Animal lengths are in feet (ft.)
* Animal weights are in pounds (lbs.)

## Requirements

### List View (Initial screen) 
Upon launching the application a user is asked how many zoo animals to view in a list between 1 and 10. Upon selection, this should populate the list with the selected number of zoo animals from the API.

The list should display;
* An image of the animal as a thumbnail
* The name of the animal
* The habitat of the animal

Additional requirement;
* There should be a refresh icon within the navigation bar of the screen. Tapping this icon should prompt the user to input how many animals they wish to list, and call the API with that specified number.


### Detail View 
Tapping on an entry from the list launches the detail view for the selected animal.

This detail view should display;
* An image of the animal
* The name of the animal with its Latin name within brackets e.g “Naked Mole-rat (Heterocephalus glaber)”
* The diet of the animal
* The minimum and the maximum weight of the animal
* The minimum and the maximum height of the animal
* All weight and height values must be converted to the user's saved preference with the unit displayed alongside it e.g "1.9 lb”. If no user preference has been set yet, default to provided API values.

### Settings View 
The user should be able to select their preferred unit choice for both height and weight. Upon first entering the view, height should default to feet, and weight should default to pounds (lbs).
The user should have a choice of updating both on the same screen, presented with a “Save" button somewhere on the screen. 

Height choices;
* Feet
* Centimetres
* Metres

Weight choices;
* Pounds (lbs)
* Kilograms (kg)
* Stones (st)

Note: All values displayed in the UI when converted can be shown as the value itself, e.g stones converting to a value of 1.42, you do not need to split this up into 1 stone 42 lbs, it is OK to display “1.42” for time-saving sake. 


## Submission
Once we receive your submission we will try our best to review it as soon as possible and get back to you.
When reviewing your solution we will be using several criteria, including but not limited to;

* Readability
* Consistent coding styles
* Usage of platform-provided APIs
* Architectural and design choice considerations
* User interface considerations

Once completed please share your project on Github with RyanLeake (ryan.leake@teamrhfitness.com) and sammygriffiths (samuel.griffiths@teamrhfitness.com) along with a README that contains a brief description of your implementation and what you would like to have added if you had more time.

Please don't hesitate to contact us if you need any clarification on the test. Thanks for your time, we look forward to hearing from you!