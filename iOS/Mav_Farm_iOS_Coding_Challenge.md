<p align="center">
  <img src="https://s3.us-east-2.amazonaws.com/mavfarm-assets/static/images/mavfarm_logo.png"/>
</p>

## Mav Farm iOS Coding Challenge

# Mav Farm meets SpaceX

We believe that the best way to gauge a developer’s skills is to inspect their work on a specific project. This gives the person a chance to show their understanding of the platform they specialized on, regardless of their social or personal skills that could interfere during an in-person interview.

This exercise is a way for you to show us your skills. Here are the basics of how we will evaluate the delivered project:

- Proper use of the version control system
- Understanding of object oriented programming and iOS patterns 
- Good grasp of best practices in Swift
- Solid understanding of UIKit, its core classes and functionality
- Ability to work with RESTful APIs, networking integration on iOS

Beyond these topics, you can feel free to experiment with additional features and functionality, or with cosmetic improvements to the app. Animations, custom transitions and UI elements would be good additions to show your skills. We care about how you would compose an elegant UI that presents good user experience

It’s fine to simplify things which should have been implemented in a real world project, to save some of your time, as long as you explain what you have skipped. If there is something unclear, ask your questions via email;
emel@mav.farm

### What you’re going to build?

You’ll build an app to display upcoming SpaceX missions.

SpaceX has a public API on ​[https://github.com/r-spacex/SpaceX-API](https://github.com/r-spacex/SpaceX-API)
 
Documentation is [https://docs.spacexdata.com/?version=latest](https://docs.spacexdata.com/?version=latest)

1) You’re going to get the list of upcoming launches and display the data in a table view. Displaying `mission_name`, `launch_date_*`, `mission_id`, `rocket_name` and showing if that rocket has any reused pieces is enough. Reused data is available inside different stages of rocket model.
(The model has launch date in different formats, feel free to pick one and format it properly)

`curl --request GET \ --url https://api.spacexdata.com/v3/launches/upcoming`

2) At the top of the table view there’ll be a countdown timer, showing how much time left for the next mission. You can use the following method for getting the next mission.

`curl --request GET \ --url https://api.spacexdata.com/v3/launches/next`

Notes:

- You’re free to design the UI in a way you like. We'd be happy to see an elegant UI that presents good UX.
- For the ease of implementation you do no need to build full data models for
networking. Just including the data to be displayed is enough.
- Details of the networking implementation are left up to you, but we do recommend using a networking library such as Alamofire.
- You’re free to use any dependency manager you want.
- Do not implement views in xib files or storyboards, please use an autolayout framework
such as SnapKit or use NSLayoutConstraints.
- Instead of using here_is_the_app.zip approach, we want you to upload the app to github/bitbucket etc. address, showing us every step of creation.
The main purpose of this assignment is to understand how fluent you are in writing well structured and understandable code in a mobile app. So implement your assignment accordingly.
