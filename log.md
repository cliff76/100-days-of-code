# 100 Days Of Code - Log

### Day 11: January 21th, 2017
##### I've been REALLY slacking!

**Today's Progress**:
I worked through an example using Couchbase mobile on Android. I also started this project by implementing a vanilla dependency injection technique and a "simplest thing that works" mentality.

**Thoughts:** 
I'm itching to understand more about modeling with modern NoSQL DBMS systems. I'm also trying to refamiliarize with this particular technology after spending a good amount of time building hybrid app technology. I'm most proud of my methodology around dependency injection. I reminded myself that I don't need fancy Dagger/RoboGuice frameworks and resisted the urge to brew any glorified home-grown annotation processors. I inject using a dependency injector factory which returns an interface. Here I was tempted to read the root object and look for @Inject annotations via reflection, instead I implement the interface with a SimpleDependencyInjector that knows all about the app and simply casts the root object to the concrete type. That makes it unusable in any other app but because this is just an example to get my feet wet with Couchbase I don't need anything that fancy. Moreover, because my app depends on just the factory and interface I can easily swap in RoboGuice, Dagger, or anything without losing sleep.

### Day 10: January 15th, 2017
##### I've been slacking!

**Today's Progress**:
I finally forced myself to sit and refactor my build a bit so I could get hot-reloading going. I also broke out an explicit build and clean task and tried to optimize building only modified files with gulp-newer.

**Thoughts:** 
 I'm not familiar with some of these tools and I have suspicions on how well they will work together but we'll see. I need to get some TDD going next so I can begin some real rapid dev work.

### Day 9: January 12th, 2017
##### Taking it easy!

**Today's Progress**: Keep it moving!

**Thoughts:** 
I needed something simple to do tonight because it was an extremely busy day. I went back to Javascript30 and did day 2, the CSS clock. I really need to up my style game for what's to come so this is right on time.

### Day 8: January 10th, 2017
##### Over-react to my server

**Today's Progress**: Client-server woes

**Thoughts:** 
I addded server side data logic to my react todo example and stretched my wings a bit. I couldn't get the server to accurately report all additions and deletes but it's coming along regardless. It sorta works but it's very sloppy.

**Link to work:** [Project repo](https://github.com/cliff76/100dayscraig)

### Day 7: January 8th, 2017
##### I wanna do open source!

**Today's Progress**: Leading by example

**Thoughts:** 
After seeing Scooter's latest push I decided it was time to pull the trigger. I blogged my idea and attempted to submit the PR only to be hit with a merge conflict due to her latest changes. I redid the pull request along with my blog entry then pinged her over DM to get her thoghts. I honestly felt like she was gonna cuss me for poking around in her repo without asking and doing her homework for her! (Just kidding!) She warmly welcomed my contribution because that's what this whole game is about anyway!

**Link to work:** [The story](https://codeforfun.wordpress.com/2017/01/09/getting-into-open-source/)

### Day 6: January 7th, 2017
##### Can I do open source?

**Today's Progress**: I created a pull request example for our Twitter group

**Thoughts:** 
I had a long discussion in our Twitter group after listening to folks dream about eventually getting involved in open source. I tried to tell everyone how much the are already involved then the discussion inspired me to give a concrete example. Using [@Scooter Phoenix](https://twitter.com/ScooterPhoenix) as the poster child of open source, I secretly enhanced her work. I saw her blog was slightly ahead of her repository so I decided to hold back a day before submitting my secret pull request surprise.

**Link to work:** [Project repo](https://github.com/techmom215/tipcalc/commit/50f09426b2e53740d2b34d6980baec11295019c7)

### Day 5: January 5th, 2017
##### Todo or not Todo? That WAS the question!

**Today's Progress**: I struggled through a React Todo app example. I also investigated how to work custom deployment on Azure. The custom deploy scripts are local and have not yet been pushed. I'll tackle Azure this weekend.

**Thoughts:** 
Faking the funk! I've been missing days and not making much progress. My log is looking abysmal as I've taken on two significant challenges for the year. The 1st and more important challenge is my Bible study which is also at risk of slipping. Add my day job and kids to the mix and its a wonder I can find time to set reminders for Alexa by asking Google to tell Siri about it! I spent most of my time re-learning REact/Redux as well as webpack, gulp, while tinkering with Yarn. I spend more time learning than coding but it's all in the same spirit. I'm hoping that pattern changes soon as I pick up speed.

**Link to work:** [Project repo](https://github.com/cliff76/100dayscraig)
[Azure Deployment](http://100dayscraig.azurewebsites.net) (It's broken until I learn Azure deployments!)


### Day 4: January 3rd, 2017
##### Tic Attack Toe?

**Today's Progress**: I struggled through a React Tic tac Toe example.

**Thoughts:** 
Barely got this working before 12am

**Link to work:** [Project repo](https://github.com/cliff76/100dayscraig)
[Azure Deployment](http://100dayscraig.azurewebsites.net) (It's broken until I learn Azure deployments!)


### Day 3: December 31st, 2016
##### If you build it, will they come?

**Today's Progress**: Mostly project structure changes and refactoring. I managed to integrate gulp for managing the build of both client and server pieces. I plan to continue refining the build until I get things in a way that make me feel productive.

**Thoughts:** 
webpack, vs, npm, vs gulp... So many ways to build a JS project. I only started with webpack because I want to learn how to use ES6 for client side stuff as I start re-learning ReactJS. I'm mostly familiar with gulp and npm. I've started delegating npm build script targets to my gulpfile and I want to get the whole hot file reloading for development. I need to be careful because each push triggers a redeploy of my Azure server. Also I have many dev dependencies listed as general dependencies. I need to keep this for now until I learn more about continuously deploying nodeJS on Azure.

**Link to work:** [Project repo](https://github.com/cliff76/100dayscraig)
[Azure Deployment](http://100dayscraig.azurewebsites.net) It renders still! (I think!)

### Day 2: December 30th, 2016
##### It continues

**Today's Progress**: Guilty! I didn't commit yesterday but I did make progress from the day prior! I learned about [some open public APIs](https://github.com/toddmotto/public-apis) which I may consider using. I finally managed to get webpack and Babel working for client side ES6.

**Thoughts:** 

**Link to work:** [Project repo](https://github.com/cliff76/100dayscraig)
[Azure Deployment](http://100dayscraig.azurewebsites.net) It renders!

### Day 1: December 28th, 2016
##### It continues

**Today's Progress**: I created an Azure WebApp for this project. I then started a NodeJS project in IntelliJ. Pushed it to Github (from the cmd line b/c our in-office proxy was giving me all sorts of problems) then Added ExpressJS to the mix. I then linked my Azure site to my newly created GitHub project using the new portal and GUI options. I deployed the Express app to the site but it didn't render initially. It was because I wasn't using the production port assigned by Azure. Googling "start azure nodejs deployment" pointed me [here](https://docs.microsoft.com/en-us/azure/app-service-web/app-service-web-nodejs-get-started) where I found my fix!

**Thoughts:** Azure seems to dramatically update each year while prompting you to try their "new portal" and abandon the old one. Didn't I just do this 1-2 year(s) ago? I think I'll really enjoy re-familiarizing with NodeJS, Express, and tinkering with the new Azure deployment and continuous delivery stuff.

**Link to work:** [Project repo](https://github.com/cliff76/100dayscraig)
[Azure Deployment](http://100dayscraig.azurewebsites.net) Doesn't currently render! (Please don't spam the site!)

### Day 0: December 28th, 2016
##### It begins

**Today's Progress**: I begin the challenge by forking this repo,  and setting up the log. 

**Thoughts:** I plan to study OAuth 2.0 and try to do some hack integrations with 3rd party service providers like Flickr or Twitter. I've never done much with OAuth2.0 so this should be fun!

**Link to work:** [This repo](https://github.com/cliff76/100-days-of-code)
