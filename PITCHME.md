@snap[midpoint]
# Demystifying CI/CD 
@snapend

Note:
- Who here is familiar with CI/CD?
- Who knows the difference between CD and CD?
- Who doesn't care and was looking to pass the time checking email during this session?
I've been part of development teams where code would take weeks or months before it was pushed to testing, and often months before it would be deployed to production. And that was just one team, working on one feature, while other teams worked on other features doing the same thing. It was also not uncommon to be working on a project for a year - only to have it dumped because the business and/or customer had already moved past the need. Who here would prefer slow code delivery cycles? Every technology delivery team wants to increase their code delivery velocity and the quality of the code they push to market.

---
## TickTock

![time is ticking](assets/img/time-is-ticking.gif)

Note:
Time is a dev's most important and valuable asset. If we don't manage our time properly, then we're not able to accomplish our goals, finish our projects per their deadlines, etc. In addition we also run the risk of failing our team in regards to delivering tasks and software. Often times devs get wrapped up in our own heads sometimes when we're doing pretty intensive work on trying to fix bugs manually, and we tend to encounter these moments that we'll call time sucks. I'm not talking about Snapchat, TikTok, or Twitter. It's where we're just spinning our wheels looking for bugs, for problems within the code base. And a lot of times we can leverage some other tooling to help us with these these time sucks that we get ourselves into.

---
@snap[west span-45 text-center]
![jeremy](assets/img/london-bridge-over-thames-jeremy-800px.png)
@snapend

@snap[east span-55 text-8 text-center]
Head of DevRel<br />
![width=300](assets/img/logo.png)
@snapend

Note: 
Hi, I'm Jeremy Meiss and I am the Head of Developer Relations and Community at CircleCI. Today I'm going to be diving into what CI/CD is and hopefully make it easy to get a handle on, and as kind of a jumping off point to either implementing into your company, org, or project, or making improvements to your already existing process. So with that, I figure it's good to jump into defining some terms that I will be using over the next 25 minutes or so.

---
# "DevOps"

![What is devops](assets/img/devops_is_coming.jpeg)

Note:
DevOps is a set of practices that combines software development (the "Dev") and information-technology operations (the "Ops") which aims to shorten the systems development life cycle and provide continuous delivery with high software quality.

---
@snap[west span-45 text-center]
### DevOps Lifecycle
@snapend

@snap[east span-55 text-8 text-center]
@ul[list-spaced-bullets list-fade-fragments](true)
- Plan @note [Initially plan yourself regarding the type of application you need to develop. Make the rough picture regarding the development process]  
- Code @note [Code the application as per the client requirement.  with the plan, you have made in the initial step.]  
- Build @note [Build the application by performing the integration of various codes you have done in the previous step.]  
- Test @note [This is the heart of the application. Test the application that you have built so far. And the rebuilt the application if necessary.]  
- Releases @note [If you succeed in the Test phase, then its time to release the application into Live.]  
- Deploy @note [Deploy the code into a cloud environment for further usage. It is performed in such a manner any changes made should not affect the functioning of high traffic website.]  
- Operate @note [Perform the operation on the code if any have.]  
- Monitor @note [Monitor the performance of the application as per the client requirement. Keep a note on the performance of the application. Make modifications if any to satisfy the clients. And if does not reach up to the mark make changes in that particular area to satisfy the client.]  
@ulend
@snapend

Note:



---
@snap[midpoint]
## Continuous {Integration|Delivery}
@snapend

Note:
CI/CD are Principles & Practices that enable teams to release quality code
Fail Fast is the most important here. The ability to know when stuff is broken is invaluable. It leads to faster fixes and delivery of quality code. Quickly fix issues, resubmit fixes. Deliver stable code consistently.

---
@snap[west span-45 text-center]
## "CI"
@snapend

@snap[east span-55 text-8 text-center]
@ul[list-spaced-bullets list-fade-fragments](true)
- Merge code changes often
- Run automated tests to validate builds
- Only integrate tested code into code base
- Changes frequently merged into release branches
@ulend
@snapend

Note: 
Continuous integration is the practice where developers are merging code often to a shared code base. Meaning, if you have a repo on GitHub and you have, let’s say ten developers, all ten developers will branch from that shared code base and they’ll have an individual silo based on their development environments. And, as they’re writing code they are continuously pushing code up into this shared code base. The reason for that is sometimes when we write code it can take us a week, two weeks, whatever the time frame is and what that means is if you are developing in isolation the rest of your team doesn’t really know what’s happening until push those changes upstream, right, to that upstream repo. So that, they can pull them down and see what’s going on. By doing so the team is more informed about what each other’s code base looks like and the potential future conflicts that could arise. So as developers are merging codebase changes often, we want to run automated tests, right, automated tests to validate these builds. So, as you’re pushing your code base up stream we’re definitely inclined to start running these automated tests to insure the code that you’re pushing is actually of quality. Again, only tested code is integrated into the code base and then the merge of these changes are frequently released to our production branch or our release branch. Continuous integration gets us a speed in a sense that, you know, once you write some code, you push it up stream and automation takes over, and it them validates those builds to insure that you’re only pushing quality code into the production branches. 


---
@snap[west span-45 text-center]
## "CD"
@snapend

@snap[east span-55 text-8 text-center]
@ul[list-spaced-bullets list-fade-fragments](true)
- Faster release cycles
- Low-risk releases
- Higher quality
- Lower costs
@ulend
@snapend


Note:
Now, continuous delivery is basically automation, or the overall chain of processes generally called a "pipeline", that helps us with releasing our software faster by automatically getting source code changes and running them through building, testing, packaging, and other related operations to produce a release. The goals of CD in producing software releases are generally automation, efficiency, reliability, reproducibility, and verification of quality (through continuous testing). In most cases it also means you are delivering smarter and lowering risks to your release processes. The code and the software being released should be at a higher quality, and by using these continuous delivery mechanisms you're actually lowering your costs for time for your developers, your costs for actual billable items such as time spent delivering software to multiple infrastructures like staging, QA, and production.

---
@snap[midpoint]
## So now can I CI/CD?
@snapend

Note:
Much has changed in the way that developers build and ship code. In implementing CI/CD, you're implementing practices and principles which aren't really about tooling. It's important that you and your teams sit down and decide how you will implememnt CI/CD practices and principles. CI/CD aims to break down the walls between Dev and Ops and get everyone on the same page working together. You don't have to implement CI/CD all at once. Instead, thing about it as iterative in and of itself. The systems and tech currently in place in your organization, combined with the culture (which in itself might need to be reformed) dramatically incluence the customization needed to implement.

---
@snap[midpoint]
## CI or CD?
@snapend

Note:
Continuous integration automates the building and testing of your software. Continuous deployment is an extension of this automation and allows for your software to be deployed after every code commit that passes your test suite. The most successful development teams deploy their software often.

The software development process consists of three main centers of work:

---
@snap[midpoint]
### Code creation
@snapend

Note: 
Creation of the code: This is where the software development team is the most creative. They are turning user stories into elegant code. The most important tool here would be the VCS like GitHub, BitBucket, etc.

---
@snap[midpoint]
### Code orchestration
@snapend

Note: 
Orchestration of new code as software: This is where the heart of continuous integration lives. Once the developer commits code, the continuous integration build server automates the build, test, and deploy process. It does the heavy lifting of turning the code into working software. Users configure how the code is processed via a config file, usually YAML, and this file often allows for almost infinite configurations, allowing teams to build and test their way.

---
@snap[midpoint]
### Code logistics
@snapend

Note: 
Logistics: This is the final step of shipping the new software to production. The logistics part of the software development process includes getting the tested and approved code into production. This includes the setup, configuration, and management of the production servers. To gain the full benefit of continuous integration, continuous deployment is necessary.

---
@snap[midpoint]
## Benefits of CI
@snapend

Note:
The fundamental tenet of continuous integration is quite simple: commit and integrate your code often—daily at a minimum. Such a small change in your software development process can yield big results.
Using this development strategy, you can:
- Improve team productivity and efficiency
- Accelerate speed to market
- Identify product/market fit
- Release higher quality, more stable products
- Increase customer satisfaction
- Keep developers happy and shipping code

---
@snap[midpoint]
### Say _WHAT_ about benefits?
@snapend

Note:
You may be thinking: "How do these benefits accrue from such a simple change in your workflow?"
When you commit more often, you can identify and resolve merge conflicts earlier, or avoid them altogether. So, instead of writing a thousand lines of code and finding an error, you’ve only written a hundred. Finding the bugs in your code becomes an errand of a few minutes instead of a few hours. This leads to improved team productivity and helps developers ship working code more quickly.

---
@snap[midpoint]
### I feel the need.... the need for SPEED!
@snapend

Note:
Shipping new features quickly means increasing your speed to market. This gives your team a competitive edge in two key ways:

1. Your customers are getting access to new features faster, leading to higher customer satisfaction
2. Your company is getting a faster return on investment from new features. Rather than waiting for the next milestone to release code, you can deliver value as soon as a new feature is ready for the market.

---
@snap[midpoint]
## So now CI?
@snapend

Note:
With that bit of info out of the way, it is important to get a continuous integration (CI) pipeline set up as early as possible in the development of your application. Once tests are added to your CI pipeline, you can continue to innovate and build with confidence knowing that you cannot merge code to master that doesn’t pass your tests. Additionally, developing a continuous deployment workflow into your CI pipeline provides the automation of deployment. Automating your software’s build, test, and deployment is important to getting back to work building the features that your users care about the most.


---
@snap[midpoint]
### Make sure everyone is on the same page
@snapend

Note:
Make sure everyone is on the same page with respect to what you’re trying to achieve by introducing a new CI/CD tool. There's nothing worse than reading from different playbooks on how to do a task. This requires everyone in the org to know what the processes are and how to go about their day.

---
@snap[midpoint]
### Always start small
@snapend

Note: 
Continuous integration is not just about implementing a new tool. It is about changing how the development team works. It’s a new mindset. And, making culture changes in an organization is not easy. The best way to get started with continuous integration is to start small. Don’t try to make your entire organization into a model DevOps team overnight. Give it a day or two :D. Instead, make process changes on one team to see if they work within your organization. If you see improvements, keep moving incrementally.

---
@snap[midpoint]
### Do what works for you
@snapend

Note:
Do what works for you. Know that DevOps might not be the right solution for your organization. Some companies have been successful for a long time without DevOps, and it might not be right for them, given their culture or their product needs. For example, if confidentiality is a big part of your company’s product strategy, then shipping incrementally to get feedback would not work for you, as you’d need to keep all product details under lock and key until a big launch. In that environment, it would be very difficult to build a DevOps culture.

---
@snap[midpoint]
### Always measure
@snapend

Note:
Always measure. Before you start any improvement plan, get accurate metrics for where you’re currently at (i.e. our dev cycle takes X amount of time). Do this before you’ve invited a site reliability engineer onto the development team. Then after a small amount of time, you’ll be able to see whether it’s been effective. As an example: When a lot of Agile transformation was happening, many companies adopted standups, without really understanding why, or measuring whether it had a positive effect on their team. This likely wasted more time than it saved. We'll touch on a few universal metrics to pay attention to in a few minutes.

---
@snap[midpoint]
### Do not try to automate everything
@snapend

Note:
Do not try to automate everything. At least not all at once. One misconception about DevOps is that all the infrastructure provisioning and the configuration management must be done automatically. This is referred to as “infrastructure as code.” But some things work better when they are manual; automation is not the solution for everything. Sometimes, you have to start the manual way to figure out what the best solution for automation actually is.

---
@snap[west span-45 text-center]
### Proof of concept
@snapend

@snap[east span-55 text-8 text-center]
@ul[list-spaced-bullets list-fade-fragments](true)
- A rigorous testing practice
- Consistent software environments
- Training on continuous integration practices.
- Reports to measure key metrics.
@ulend
@snapend

Note: 
A great way to get started seeing how this could work for you is to use your next small project as a proof of concept and get the following fundamentals into place:

- A rigorous testing practice, ideally using automated tests.
- Consistent software environments, from testing to production.
- Training on continuous integration practices.
- Reports to measure key metrics.

Once your team starts committing regularly and in small increments, they’ll see how much easier it is to be responsive to bugs. And, as they resolve bugs faster, they will deliver features even faster. This will give your team the momentum to scale continuous integration across the organization.

---
@snap[west span-45 text-center]
## CI/CD Better Practices
@snapend

@snap[east span-55 text-8 text-center]
@ul[list-spaced-bullets list-fade-fragments](true)
- Make testing an integral part of the development process. @note [Fostering a rigorous testing culture is the most important element that a company needs for successful continuous integration. In order to confidently integrate new code into the mainline, the team needs the confidence that the code is sound. Engineers should write tests as each feature is being developed. At CircleCI, we run tests on any new code that is committed and our system alerts the developer if they have a successful “green” build, or if they need to fix issues because the build was “red.” Without tests, of course, green builds are meaningless. Ideally, the team is using automated testing, though that is not a requirement. QA services, such as Rainforest QA, can be integrated into the continuous integration process.]
- Ensure that the testing environment mirrors production. @note [To support your rigorous testing culture, it’s important that the testing environment mirrors the production environment. Otherwise, you have no guarantee that what you’re testing will work in production. This means the testing environment should use the same version of the database, web server configuration, artifacts, etc.]
- Use coding better practices, such as pair programming. @note [Another better practice for software development is pairing during coding. For more complex pieces of functionality, pairs discuss the architecture approach before a single line of code is written. Before any code is merged into production, another developer always reviews the code. This helps ensure that coding best practices have been used, the code does not conflict with existing code or code that another developer is working on, and the new functionality is scalable.]
- Automate the deploy workflow. @note [Finally, to ensure that the entire software development pipeline is fast and efficient, the deploy workflow should also be automated. By automating the deploy workflow, the team gets their finished code to production more quickly. Because, after all, what’s the point of developing software quickly if it’s not getting to the customer?]
@ulend
@snapend

Note:
Developers who practice continuous integration commit early and often. This allows them to detect conflicts before deploying code to production. And, having a smaller commit makes it easier to troubleshoot the code if there are any issues. Committing software daily, or even more often, is necessary for continuous integration, but not sufficient.

---
@snap[west span-45 text-center]
## Key CI/CD Metrics
@snapend

@snap[east span-55 text-8 text-center]
@ul[list-spaced-bullets list-fade-fragments]
- Lead time @note[Lead time is the length of time that it takes for your workflow to run from first trigger to completion. It is a measure of how quickly you can get a signal. A short lead time requires a maximally automated software development pipeline. That is why teams use continuous integration to automate building and testing. Automation of the pipeline via CI shrinks deployment timelines of weeks to months down to hours, if not minutes.]
- Deployment frequency @note[Deployment frequency: How often your team kicks off a workflow is an indication of how many discrete units of work are moving through the development pipeline. With a fully automated software development pipeline, even complicated updates to your codebase can be deployed automatically. Hotfixes are available immediately — and they go through the same rigorous testing as any other update.]
- Mean time to recovery (MTTR) @note[Mean time to recovery (MTTR): Mean time to recovery is contingent on getting actionable information, fast. Getting a failed status returned quickly will enable you to get from red to green in the shortest amount of time. Adopting CI/CD practices enables rapid feedback loops, and is the best way to ensure fast signal for your developers. A robust CI/CD practice includes realtime artifacts such as logs and coverage reports from your test suite and gives devs the ability to troubleshoot in an environment equivalent to the production environment.]
- Change fail percentage @note[Change fail percentage: The highest performing teams rarely push bad code to their default branch. But this doesn’t mean that these teams never write faulty code. Testing and security checks are performed on a separate branch and only when everything passes is a merge allowed to take place. A team should know that their code works well before it is merged into the default branch.]
@ulend
@snapend

Note:
So earlier I mentioned that there were some key metrics to track regardless....


---
@snap[midpoint]
### Regular cadence
@snapend

Note:
It’s helpful to have a regular cadence of reporting. Automated daily reports help ensure that if there is an error, the team catches it fast. And, analyzing the weekly reports allows teams to dive much deeper into the CI processes and find improvement areas.








