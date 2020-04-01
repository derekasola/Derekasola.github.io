---
layout: essay
type: essay
title: "Being Social While Quarantined"
# All dates must be YYYY-MM-DD format!
date: 2020-03-31
labels:
  - JavaScript
  - ES6
  - Meteor
  - React
  - Semantic UI
  - GitHub
---

Because of the covid-19 virus, there has been a stay at home order put in place for all non essential workers. This quarantine, for some, is hard because of the lack of interaction with their friends and family. My idea for this is to make a social media platform for people to interact with each other. The key features i will try to implement will be, sign in/sign up, friends list, media build-board, and even customizable UI.

Sign in / Sign out:
---
This feature is already included with the meteor-react-template we have been using for our WOD's. ill include a link here:  [Meteor-react-template](https://github.com/ics-software-engineering/meteor-application-template-react)


Friends List:
---
The friends list feature, I was thinking of bringing it back to Myspace days with the top friends section of the friends list, and then have the rest of the friends in a drop down menu. To find friend there can be a find friends page that lists all the users in semantic-ui feature "Card" form. i will most likely use Card to display the top 5 friends with their descriptions as well.


Media Build-Board:
---
I want this feature to allow people to "Post" pictures, messages, and videos, most likely in Cards, on a horizontal list like Facebook. I hope to add a comment section as well for friends on your list.


Customizable UI:
---
As far as im going to try to go with this is changing background color, change user picture, and maybe background image. Like most of the features mentioned, it will take the url of the image and store it in a database like the list stuff section of the template i linked above.

Example Of Data Storage:
---
`
"defaultData": [
    { "name": "Basket", "quantity": 3, "owner": "john@foo.com", "condition": "excellent" },
    { "name": "Bicycle", "quantity": 2, "owner": "john@foo.com", "condition": "poor" },
    { "name": "Banana", "quantity": 2, "owner": "admin@foo.com", "condition": "good" },
    { "name": "Boogie Board", "quantity": 2, "owner": "admin@foo.com", "condition": "excellent" }
  ]
`

Conclusion:
---
I'm not sure that all these are possible, and i tend to get a little over my head, but i have a lot of time on my hands because of the situation and im willing to at least stick with the main idea of social media website. I look forward to working on this project and writing up another essay after ive completed it.