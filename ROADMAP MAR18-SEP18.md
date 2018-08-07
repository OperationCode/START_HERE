# Operation Code Roadmap - March 2018 to September 2018

**Join. Code. Contribute.**

These three words describe one of Operation Code’s founding principles - that a member should join our organization, start learning to code right away, and immediately begin contributing to our open source projects.  Our emphasis is on learning through doing - our open source projects are more than products, they are essential teaching tools, getting our veterans real world experience with the most in demand technologies of today’s industry.  When a member has contributions to our (or other) Open Source projects, they have a portfolio of real world work that they can show to employers, it is a major help in landing that elusive first tech job.

While we have a wonderful and deeply appreciated group of contributors, the time between when someone joins Operation Code to when they submit their first commit has stretched to months.  Part of this is due to the tech stack that was chosen.  This is not to say it is the wrong stack - for us or any organization.  It was chosen with the intention of providing our members experience with the technologies potential employers look for most - and there is a lot of value in that.  At the same time, we need to recognize that having an advanced tech stack makes contributing as a beginner much harder.  While I don’t think we should rethink our tech stack at this time (starting over on even one component would set us back significantly, which we cannot afford at this point), there are things we can do to make the path to that first commit much easier.

In considering a road map for the next six months I’d like to make one vision front and center.  That is “One week to join, code, and contribute a first open source commit.”  I would like this principle to be the priority for the next six months.  This is not to say there are not other things we need to get done - but when considering priorities or new features, we must think about them in terms of whether they make that first time contribution experience easier.

Here are my current thoughts on a roadmap for our overall engineering organazation, as well as each individual component.

## Overall

* Open Source Basic Training - this will be a guide to getting started with Open Source.  This needs to include lessons (links to particularly good blog post tutorials, etc. are welcome) on Git and Github.  Git is often a major hurdle to getting started - we need strong and very visible learning materials on the essentials of git.  We also need a repo that users can immediately contribute to to put their git and Github skills in action - perhaps a repo of text files that a user can add their name or something else to?  The goal of this basic training is to familiarize someone with the workflow of git and Github - which is critical to contributing to any or our projects.  This should also include a brief guide to each of the major Operation Code Open Soure Projects - what technology they use, links to 101 guides to those technologies, etc.  Members should receive a link to this training immediately when they join the org.
 * _05AUG - still a big priority -conrad_
 * _05AUG - we have the pieces in place but need to get them all together -ashley_
 * _05AUG - maybe slackbot pings people about it and directs them to a page -nell_

* Deprioritized ~~Better broadcasting across platforms - our town halls are great, especially now that they can be broadcast over Youtube live.  We should look into broadcasting these across other platforms as well - i.e. going live on Facebook or Twitter at the same time as we go live on Youtube, perhaps even including Twitch.  We need to look into software that would let us broadcast over multiple platforms - or at the very least push announcements that we are live to multiple platforms.  Eventually I would like to see this show on the main home page of the site, but that is not within this six month roadmap. 

## Front End

* ~~Policy Page (this is needed for an upcoming event, Jameel Matin will be providing the copy)~~ *COMPLETE*

* Templates for static pages. *COMPLETE*
 * _05AUG - Kyle has made this easier as part of the new frontend, and we're looking at some form of CMS integration for next roadmap._

* ~~Host docsify page on docs.operationcode.org - we need to have our docs in one easy to find and easy to navigate place, this is essential to making sure people can find the information they need quickly.~~ _05AUG - deprioritized, github will suffice for now -nell_

* *P1* Landing Page Redesign
 * _05AUG - we need to communicate who we are and how you become a part of us, how to join. How do they know if we're legitimate? -davidm_
 * _05AUG - need a designer for this_
 * Re-think and redo hero banner implementation

* Introduce a drop-down item for the navbar.

* Make sure that all UI components have Jest snapshot tests and Storybook instances
* Document how to add a Jest test and a Storybook instance of a component
 * _05AUG - both in progress with kyle_

* Discuss moving shared components into UI Lib via NPM
 * _05AUG - deprioritized -nell_

## Backend

* ~~Deploy interface for execs to query the database (possibly Active Admin or Forest)~~ _done!_
 * As operations, I want the member list in the backend to contain both signup *and* Slack information, so that I can have a single view of our membership base.
  * _06AUG - This is a current WIP for both pybot and BE. -william
  * 06AUG - BE issues: 312, 319, 320, 322 are all related to this. The idea is use pybot as a way to register email and user information updates from slack api, and transmit this to the BE. -william
  * 06AUG - Here's his high level view before it was broke out into individual issues: OperationCode/operationcode_backend#314 -william
  * 06AUG - Issues 1 and 5 are done. 2, 3, 4 are waiting. -william
  * 06AUG - If this is P1 for @JennWeideman maybe get @dmarchante to review the status and make an epic or something to track this progress? -william_

* ~~Add ability to run Cron Jobs (need help of infrastructure)~~
 * _05AUG - deprioritized until we have a backend lead -nell_
 * _05AUG - PR needs review from new backend lead OperationCode/operationcode_backend#257 -jhampton_

* ~~Set up new Code Climate account - this will help give us insight into the health of our codebase, and ensure we are using best practices and keeping it beginner friendly!~~
 * _05AUG - this is already done -conrad_

* ~~Implement roles/permissions for end users~~ _done!_

* Implement an authentication strategy/option to secure and expose the API (for non-signed in user consumers, i.e. Slack, apps, etc.)
 * _06AUG - harry came up with a good idea for how to integrate pybot into BE. For now we can use that for this one case and treat pybot as a main focal point so I don't have to re-architect in ruby. -william_

## Infrastructure

* *P1* Staging Environment for operationcode.org - this is the number one priority, currently we can only run operationcode.org components locally or in production, we need a staging environment we can deploy to and test components in a production-like environment before deploying to production.  This is essential and gives us a strong safety net for testing the effects of new commits before they go to production.
 * _05AUG - done on new frontend -kyle_
 * _05AUG - Ashley and Walt to discuss backend staging env implementation, @kylemh to alias preview builds with backend staging env_

* Log Collection Solution - currently logs can only be viewed through the Kubernetes cli - and it is very difficult to see logs across our Kubernetes pods.  We need a centralized logging solution to help quickly troubleshoot errors and watch for patterns.
 * _05AUG - still a priority -nell_
 * _05AUG - needed for debugging -ashley_

* Secrets Management Solution
 *  _05AUG - deprioritized since there is a way to do this through Kubernetes right now -nell_
