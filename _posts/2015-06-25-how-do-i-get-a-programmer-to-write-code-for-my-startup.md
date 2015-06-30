---
layout: post
title:  "How do I get a programmer to write the code for my startup?"
date: 2015-06-25 15:50:00
categories: startups coding
author_name : Chris Sharkey
author_url : /author/chris
author_avatar: chrissharkey
show_avatar : true
read_time : 34
feature_image: feature-laptop
show_related_posts: true
square_related: recommend-laptop
comments: true
---

The traditional path for finding a technical co-founder is to find a young whipper-snapper with programming skills who you can get to work for free in exchange for equity. This was what happened when my business partner and I created Stayz: we agreed on a 50/50 split - I did all the programming and SEO and he brought the business knowledge, connections and ideas. I worked for 2 years without pay, and we ended up selling the company for $12.7 million 2 years after that. I'm sure it is the path that many successful startups take.

While it works, the approach is no longer realistic. The public knowledge around creating a startup now is such that a programmer of any skill level knows that the execution is at least as important as the idea, and would either prefer to do something on their own, or wants to be paid for their work.

Either way, the below approach is going to help you whether you have a young programmer working for equity, or you are paying someone to develop the software for you. The short version is that you need to know every single detail of what you want, and do as much of the work as you can without knowing how to program a computer. And that is a lot. You want the programmer only working on the things which you cannot.

A lot of what is seen as part of the web or phone app software development process, is stuff which could have been done in advance of involving a programmer. Things you find by trial and error through actually programming a product are a good way to learn, but it is expensive in money if you're paying for it, and time consuming either way.

Time your developer spends fleshing out your ideas is time that they should be spending coding your app. You should already know what the features of version one of your system will be in explicit detail. If you don't, you need to figure it out before you engage a developer. It will save you time and money and you will end up with a better first version of your product. A programmer with no domain-specific knowledge should not be making feature decisions about your product.

By all means be agile and iterate later, respond to customer feedback and tweak and improve, but first get your base product done with a simple set of features that you know inside and out. The developer who makes your first system should be like someone baking a cake that you wrote the recipe for: they follow the recipe as it is written, and the only reason you didn't bake it yourself was because you didn't know how to work the oven.

As a non-technical founder, you are capable of creating at least the following before you need a programmer:

- A succint list of fully-described features.
- Full working mockups of screens.
- V2 features (things that you are actively choosing to save until later).
- A full database structure and test data.
- A server/hosting budget and account and any technology preferences.
- Domain name, logo, images, content and accounts for exernal integrations.

That's a lot of stuff! A lot of stuff that if you don't provide to a programmer, they are going to have to extract from you gradually over time, or figure out for themselves.

Allow me to describe each of these in detail so you know exactly what you need to deliver to the programmer of your minimum viable product.

**A succinct list of fully described features**

Succint means stuff that makes your app unique. If you're making Facebook it is: profile page, photos, comments. If it is Reddit it is: post links, upvote/downvote, comments. The less features to start with, the better.

A good way to describe your features is to write the help documentation for them as if they already exist. Nothing hones your thinking like having to describe to a beginner how something works. As soon as you have to be specific, you corner yourself into making key system decisions.

Let's say we wanted to have a feature in our app which allows the user to set their profile picture. To write the documentation, we need to ask ourselves:

- How does the user get to this part of the app?
- How do they upload their photo?
- Can they resize or alter their photo?
- How does the photo get saved and where?
- Are there any permissions on the photo, can everyone else in the app ecosystem see it or just some?

This process helps us identify how much work there is for a seemingly simple feature. From a technical perspective you've got:

- System navigation to get to the feature: menu, icons, code for navigation.
- Accessing the user's camera, web cam or file system to get the photo.
- Potential image resizing tools which are complex and add design and mathematical challenges.
- Requirement for a server-side feature: data storage and retrieval for photo storage.
- Permissions system and security to protect the photos.

Don't worry if you can't think of these technical challenges on your own, exposing them by writing the help steps is enough, your developer will identify them quickly when shown the documentation.

At this point you should also ask: how badly does the first version of my product need profile images? If it's a dating app it is probably a must. If it is a system for finding cleaning services, maybe give it a miss in version 1, even if the app is less aesthetically pleasing.

Once you have gone through this process and decided that you need the feature, try writing the steps for the end user of how they would use it:

> Uploading your photo allows other users in the system to see who they are going to date. To upload yours:
> 
> 1. Click on the default profile image.
> 2. Click "Upload photo".
> 3. Select a photo from your hard drive (JPG or PNG).
> 4. Use the cropping tool by dragging the slider to get your photo how you like it.
> 5. Save the photo or cancel.
>
> You can now see your profile on the top left of the screen whenever you are using the app, other users can see your photo in the marketplace view when they are looking at the tyres you have available to sell.

Through writing this basic help article we have identified almost everything that the developer is going to need to implement this feature. 

You need to be the one thinking out each branch and course of activity that can happen in your system, not your programmer. They should spend their time implementing the solution, not describing it. 

If you can't or won't go through this process, I'd have you consider how serious you are about working on a startup. The work will only increase from here and doing this is easy compared to the work ahead.

**Full working mockups of screens**

There are several excellent tools which allow you to visually design web and mobile applications in detail. [Moqups](https://moqups.com/) and [Invision](http://www.invisionapp.com/) are two that I would recommend. Both will allow you to create wireframe designs for your app to give to a developer, and both allow you to wire up buttons and things so it can actually somewhat work like he app will when finished.

Any time you spend mocking up the UI in these tools is time that your programmer doesn't have to spend experimenting and making mistakes on the real thing. It will save a *lot* of time.

If you hand your programmer access to fully complete mockups of your application at the start of development, along with the help guides you wrote in the previous step, the time to implement your application will be drastically reduced and will reduce the time and cost to get your minimum viable product online.

**V2 features**

As you plan out each of the features of your project, you will come up with more ideas for features. Part of the excitement of working on a startup is that you've found something which will bring value to people in your target audience. That excitement is increased when you think of how much more value the additional features will bring.

The crucial thing here that you have to keep in mind is: there's no point having all these features if no one uses your app long enough to need them.

- If your app takes longer to get our there because of the additional features: no one will use the new features.
- If your app fails on its basic use case because you didn't get the core features right: no one will use the new featues.
- If users are confused about what your app is for because of all the additional features: no one will use the new features.

Create a V2 list and put your additional ideas there. Then follow Warren Buffet's advice and avoid working on these features at all costs. These are the main things which will distract you and your programmer from getting the project completed and any time spent thinking about them, planning them or working on them is by definition going to detract from the main project.

If your startup works, there's going to be plenty of time to work on those V2 features and add that extra value later.

**A full database structure and test data**

Even if you are non-technical you understand that your application is going to need to contain and store data. 

Firstly, your app might need data in order to operate. Perhaps you are making a stock trading app and need access to price information. Perhaps you are working on a turn-based directions app and need map data. 

You should gather such data in advance and have it ready for your programmer before they start. If you don't know how to gather the data, you should at least know where it can be found, or buy it.

Secondly, you need to know what data your app needs to store and the types of that data. Writing out something simple like the following to represent the data you will need to store will be simple once you have written out your features in detail as described above. 

As shown below, you should also show how the different types of data are connected, e.g. "Joined with Clients.id"

    Clients:

        id        number
        FirstName text
        LastName  text
        Email     text
        Age       number
        OptedIn   boolean

    Pets:

        id        number
        client_id number (Joined with Clients.id)

Additionally, you should provide your developer with test data. Providing some test data is important because it will flesh out any issues your application has with "real world" data. Developers use all sorts of ridiculous things to test with, but usually it looks something like:

    wfisuhfsjhfeg
    sdfihdf
    sfhdgfjshgf
    fkfh

The problem with using this kind of data to test with is that it doesn't match what happens in the real world and doesn't help to identify application problems with: data types, character sets (e.g. can your application handle umlauts or emojis?) and scalability. If you always test with 1 or 2 entries and your clients are going to use 1000s, you're going to run into those issues when you go live rather than when you're still testing. 

Providing your developer with a few hundred or thousand realistic-looking users and types of data you expect to store, will help immensely and reduce the amount of debugging and tweaking time your spend in your launch phase.

**All and Sundry**

Finally, there are lots of little things you need to provide to your developer: a name for the project, a domain name and the login information to set it up, a server to host it on or at least a budget to spend to get hosting, a logo for your company, images to use on the website or in the app, content to use on the website, frequently asked questions, terms and conditions, privacy policy.

On top of that you need to think about accounts you'll need with other services: [Google Analytics](http://www.google.com/analytics), in-app event tracking like [Segment](https://segment.com), other external integrations you might need. Are you expecting to receive files via [Dropbox](https://www.dropbox.com)? Set up an account and provide the developer with the API key.

I'm sure you're getting the idea.

**Marketing automation and other external infrastructure**

One other thing to consider is: how much of my app could just be done by another service? The core of your app might be unique, but things like:

- Capturing leads through forms
- Tracking significant application events through segment and starting customer journeys
- Sending email/SMS/Slack notifications to clients 
- Customer segmentation
- Transactional emails
- Net promoter score surveys
- Newsletters

All of these can be handled by a marketing automation solution like [Autopilot](https://autopilothq.com). Using a marketing automation solution means that these aspect of the system can not only be set up quickly, but they can be done by you while the programmer is working on aspects of the system that only they can do. There is no need to re-invent these tried and true systems which can be done much better by a dedicated organisation.

**How this well help you get a programmer to write code for your startup**

This post has basically said that to get a programmer to write code for your startup that you need to just do everything for them. It all sounds like a lot of work! But that's the point. When an experienced developer is asked to be a technical co-founder on a project or to "just handle the technical side", they will consider some or all of the above in their thinking about whether they would like to take on the project.

If you have considered these things and are very prepared, a programmer is far more likely to want to partner with you because they will know that you're willing and able to do your share of the workload. If you're paying a programmer to do the work, they'll be able to charge you less knowing that the project is unlikely to blow majorly out of scope since you have done so much preparation.

Your project will be completely more quickly, cheaply and you'll end up with a more finely honed minimum viable product which you can build into a sustainable and profitable business.

