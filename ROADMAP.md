# Operation Code Roadmap - March 2018 to September 2018

**Join. Code. Contribute.**

These three words describe one of Operation Code’s founding principles - that a member should join our organization, start learning to code right away, and immediately begin contributing to our open source projects.  Our emphasis is on learning through doing - our open source projects are more than products, they are essential teaching tools, getting our veterans real world experience with the most in demand technologies of today’s industry.  When a member has contributions to our (or other) Open Source projects, they have a portfolio of real world work that they can show to employers, it is a major help in landing that elusive first tech job.

While we have a wonderful and deeply appreciated group of contributors, the time between when someone joins Operation Code to when they submit their first commit has stretched to months.  Part of this is due to the tech stack that was chosen.  This is not to say it is the wrong stack - for us or any organization.  It was chosen with the intention of providing our members experience with the technologies potential employers look for most - and there is a lot of value in that.  At the same time, we need to recognize that having an advanced tech stack makes contributing as a beginner much harder.  While I don’t think we should rethink our tech stack at this time (starting over on even one component would set us back significantly, which we cannot afford at this point), there are things we can do to make the path to that first commit much easier.

In considering a road map for the next six months I’d like to make one vision front and center.  That is “One week to join, code, and contribute a first open source commit.”  I would like this principle to be the priority for the next six months.  This is not to say there are not other things we need to get done - but when considering priorities or new features, we must think about them in terms of whether they make that first time contribution experience easier.

Here are my current thoughts on a roadmap for our overall engineering organziation, as well as each individual component.

## Overall

* Open Source Basic Training - this will be a guide to getting started with Open Source.  This needs to include lessons (links to particularly good blog post tutorials, etc. are welcome) on Git and Github.  Git is often a major hurdle to getting started - we need strong and very visible learning materials on the essentials of git.  We also need a repo that users can immediately contribute to to put their git and Github skills in action - perhaps a repo of text files that a user can add their name or something else to?  The goal of this basic training is to familiarize someone with the workflow of git and Github - which is critical to contributing to any or our projects.  This should also include a brief guide to each of the major Operation Code Open Soure Projects - what technology they use, links to 101 guides to those technologies, etc.  Members should receive a link to this training immediately when they join the org.

* Better broadcasting across platforms - our town halls are great, especially now that they can be broadcast over Youtube live.  We should look into broadcasting these across other platforms as well - i.e. going live on Facebook or Twitter at the same time as we go live on Youtube, perhaps even including Twitch.  We need to look into software that would let us broadcast over multiple platforms - or at the very least push announcements that we are live to multiple platforms.  Eventually I would like to see this show on the main home page of the site, but that is not within this six month roadmap. 

## Front End

* Policy Page (this is needed for an upcoming event, Jamel Martin will be providing the copy)

* Templates for static pages.  One of the biggest bottlenecks over the past year has been React - it can be a difficult framework to get started with, especially when someone is brand new to web development.  Rather than attempt to rewrite our front end in a different framework, I’d like to focus on making our particuarly implementation of React more beginner friendly.  Adding in static content is a great way for a beginner to get started with contributing - let’s make a template that can be copy and pasted for any new static page.  Yes, we might violate the DRY rule a bit here, but I think this is a worthy exception and necessary to our mission.  We need the process of using this template very well documented.  Any new copy for the front end should go in a Github issue with a link to this guide, and these issues should be reserved for first time contributions whenever possible.

* Host docsify page on docs.operationcode.org - we need to have our docs in one easy to find and easy to navigate place, this is essential to making sure people can find the information they need quickly.  

* Landing Page ReDesign

* Introduce a drop-down item for the navbar.

* Re-think and redo hero banner implementation

* Make sure that all UI components have Jest snapshot tests and Storybook instances

* Document how to add a Jest test and a Storybook instance of a component

* Discuss moving shared components into UI Lib via NPM

## Backend

* Deploy interface for execs to query the database (possibly Active Admin or Forest)

* Add ability to run Cron Jobs (need help of infrastructure)

* Set up new Code Climate account - this will help give us insight into the health of our codebase, and ensure we are using best practices and keeping it beginner friendly!

* Implement roles/permissions for end users

* Implement an authentication strategy/option to secure and expose the API (for non-signed in user consumers, i.e. Slack, apps, etc.)

## Infrastructure

* Staging Environment for operationcode.org - this is the number one priority, currently we can only run operationcode.org components locally or in production, we need a staging environment we can deploy to and test components in a production-like environment before deploying to production.  This is essential and gives us a strong safety net for testing the effects of new commits before they go to production.

* Log Collection Solution - currently logs can only be viewed through the Kubernetes cli - and it is very difficult to see logs across our Kubernetes pods.  We need a centralized logging solution to help quickly troubleshoot errors and watch for patterns.

* Secrets Management Solution
