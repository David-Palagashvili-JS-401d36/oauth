# OAuth Comparative Analysis
Collaborating with Garhett Morgan for this assignment.
## OAuth Provider Name 

We used GitHub OAuth for this assignment.

### Research Conducted By: Garhett Morgan & David Palagashvili

### Overall Score and Comments

#### Score (Out of 10): 9

#### General Comments
This is suitable for full stack as we have a server that talks to bare bones front end.

We have not looked into database.

As far as efficiency, I would say the methods operate at an O(2) for the most part. 

We were pleased with how readable the documentation was. It was a struggle to get the last two pieces of the authentication:

TOKEN_SERVER=https://github.com/login/oauth/access_token
REMOTE_API=https://api.github.com/user

But with the help of Paul Depew, a fellow classmate, we were able to break down the starter code and follow the data. At the end of the day, we followed the steps in the documentation and they were simpler than Amazon's OAuth.

#### Pros
* Excellent documentation and learnability.
* It is easier to implement and provides strong authentication.

#### Cons
* If you are adding more extension at the ends in the specification, it will produce a wide range of non-interoperable implementations, which means you have to write separate pieces of code.
* If your favorite sites are connected to the central hub and the central account is hacked, then it will lead to serious effects across several sites instead of just one.

### Ratings and Reviews

#### Documentation
It took us quite a while to get through the documentation. It wasn't nearly as long and convoluted as yahoo's OAuth docs but we wanted to understand the process so we took our time. It was well laid out and only required a few adjustments to the starter code.

Starting with the index.html, follow the code backwards through the app and you'll come across the 7 steps of Oauth2.0 similarly to what we were shown in class.

#### Systems Requirements
Dependencies used in our OAuth scenario:
    "base-64": "^0.1.0",
    "bcrypt": "^5.0.0",
    "cors": "^2.8.5",
    "debug": "^4.1.1",
    "dotenv": "^8.2.0",
    "express": "^4.17.1",
    "jsonwebtoken": "^8.5.1",
    "morgan": "^1.9.1",
    "superagent": "^5.1.3"  

The heroku CLI has built-in plugins for github's oauth. We have not looked into AWS yet.

Does it require a certain database? No.

#### Ramp-Up Projections
How long would/should it take a team of mid-junior developers to become productive?


#### Community Support and Adoption levels

Quite a popular authentication tool. 7240 companies reportedly use GitHub in their tech stacks, including Airbnb, Netflix, and Shopify.

Not all of them use GitHub's OAuth but it's a still a beast in the tech world.

### Links and Resources
* [framework](TBD)
* [docs](https://developer.github.com/apps/building-oauth-apps/authorizing-oauth-apps/)
* [examples/tutorials](https://developer.github.com/apps/building-oauth-apps/creating-an-oauth-app/)

### Code Demos
* [live/running application](http://xyz.com)
* [code repository](https://github.com/David-Palagashvili-JS-401d36/oauth.git)

### Operating Instructions
If someone were to download your repo (above), what steps do they need to take to run the application
* `npm start`
* Endpoint: `/foo/bar/`
  * Returns a JSON object with abc in it.
* Endpoint: `/bing/zing/`
  * Returns a JSON object with xyz in it.
