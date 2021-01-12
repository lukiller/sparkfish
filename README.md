# Sparkfish

## Interview Questions

- What are examples of the types of projects you have deployed to Azure?
  A web application I finished a year ago for an Oil&Gas company is hosted on Azure. It shows online and historical values of gas measurements acquired all across the country. The project I am finishing right now is mobile app that shows the same information. To get all the required data I developed web APIs that are also hosted on Azure.

- How do you classify your senior-ness as a developer? What are your development strengths?
  If have around 15 years of experience in software development. I classify myself as an expert in certain matters/technologies. My strenghts are mainly within the .Net stack, c#, MVC, Javascript, SQL Server, WPF, MVVM.

- Have you ever had a chance to use TDD? Have you found it to be helpful? If so, when does it work best for you?
  I had the chance to implement it but not for the 100% percent of the project. The project was already started when I came in, and my manager wanted to try test driven design. I followed this technique for new features. I didn't find it to be the panacea of software development. It is useful in the sense that prevents you from forgetting the creation of test cases or entire unit tests when you don't have a separate dedicated test-team.

- Have you been given the opportunity to use tools like ReSharper? What did you like about it?
  Yes, I used it for around 4 years on a project that used Resharper for unit-testing. I guess we could have done the same without it, but I remember it simplified the creation of mockup data for unit-testing. For that company we worked on remote desktops with the development environment already setup for us, and I remember Resharper made the IDE to run slower. It added useful stuff like code snippets, but I didn't like the way it changed the intellisense for Visual Studio. Most of the times I deactivated it until I had to run the unit tests were it was mandatory.

- What about Red Gate's SQL Toolbelt or similar? If you’ve been given the opportunity to use it, did you find it valuable?
  No. I use Microsoft SQL Server Management Studio.

- Can you explain what DevOps and/or continuous integration is, and some of the benefits?
  I worked using automatic CI for around 4 years on a huge project involving a team of several developers all commiting code many times a day. It was actually very useful for detecting code changes that break other modules that do not seem to be related. We had it configured in TeamCity. Each build and it's tests were directly related to developer's tasks and commits, so everytime there was a failure, the responsible developer was advised of that and had to fix the problem before going on with other tasks.

- Are you technology agnostic? Or are you pretty strict when it comes to things like Mac vs Windows, or AWS vs Azure?
  I am pretty much agnostic on that matters. I have both Mac and Windows computers, I work on both of them every day and I like them both equally. On my previous job I worked with AWS, in my current job I am working with Azure. As a personal preference I like more Azure UI, but they both actually provide the same level of service.

- What sort of administration tasks have you performed on SQL Server? What versions were you managing?
  I guess everything. On most of my jobs I almost never had a separate SQL or Database Team to do all administration tasks for me. I always had to do everything, from installing the server, configuring the databases, indexes, backup plans, jobs, to solving deadlocks and tuning queries. I started from version 6.5 till the latest ones.

- What are some of the differences you have found between Azure SQL and a traditional installation of SQL Server?
  From a developer point of view they are both the same. As an administrator, on Azure you do several administration tasks from a web UI, I guess that is the most noticeable difference.

- After you’ve added the obvious indexes to a table, what tools do you think of using to try to sort out why a query is not running as fast as you think it should?
  The execution plan is very useful to find bottlenecks. I also like to run the tunning advisor and compare the results with the current execution plan.

- [ADVANCED] If you’ve had a chance to be exposed to CTEs, how would you describe situations where they can be handy?
  I use them for very specific cases such as when having a parent-child relationship on rows within the same table, so on one query you solve a tree-like result.

- [ADVANCED] So, SQL “window functions” are pretty much on the advanced side of SQL writing, so don’t freak out if you’ve never heard or used them before. Can you attempt to explain a scenario when window functions can be used to solve a problem?
  I use window functions rarely. The one I remember having used the most is the ROW_NUMBER() function when I need to number results. Another functions I remember having used are the common aggregate functions over partitioned data to have running totals. This helps creating reports in just one query when you don't use reporting tools that already do this for you.

- How much duress would be needed to pressure you to write a PowerShell script? (I ask because I personally refuse to write in PS, but sometimes it apparently is needed when managing a SQL Server.)
  I write PS scripts. I never used them for SQL managment tasks, but I use them for automating repetitive tasks. As an example, right now I am using PS scripts for deploying builds to the testing server, since the company I am working on now don't have CI/CD software. I automated the creation of zip packages, copying files, making backups, stopping/starting the web server, setting folders permissions. I usually write a script once a year, but I use them almost every week.

- What’s the big idea with NoSQL? When is it a good idea to use that versus a traditional RDBMS?
  I had the chance to work on a small project using Google Firebase which is a NoSQL database. It actually gives you some flexibility mostly at the beggining of a project that is not fully designed in advance, so while you make progess on the development you can change the structure of the data you store and everything keeps working. I guess for me that have been working more than 15 years with traditional relational databases, it looks unstructured, untidy and I see no benefits at all. Actually, all that is being stated as NoSQL benefits are actually not that hard to achieve with traditional databases as it is said.

- You may have heard of ACID (or perhaps just “transactions”). But can you explain what BASE sorta kinda means? It’s a nerdy topic with its own theorem, so feel free to look this up and explain it in your own words.
  I have used ACID principles several times, mostly on applications that required concurrent writes of related data in different tables by the use of transactions. I am not very familiar with BASE principles, I know it is a consistency model that I guess it applies more for NoSQL databases where data does not require to be as consistent as a traditional relational database require.

- Have you ever had a chance to use SQLite? What are some of the advantages over SQL Server? Or, maybe when is this a bad idea?
  Yes, I used it several times, mostly for personal small projects. I don't recommend it for Enterprise level projects. It has known limitations.

- Python has gained a lot of ground due to the surge in data science. But, we are also finding it useful for easier-to-manage admin scripts and ETL processes compared to the horrid affair that is SSIS. Are you now or will you ever have interest in becoming a pythonista?
  I have a basic knowledge of Python. Actually I had to learn it when I was taking a Machine Learning specialization, since all the code examples where given in Python. This language is being widely used for Machine Learning since it alreay has a lot of very optimized math libraries. I use SSIS, I know it sometimes gives you headaches but once you solve them, your ETLs run forever without issues. I didn't know Python is being used for managing databases or for creating ETLs. I would certainly like to know how it works.

- What problems does MongoDB solve as compared to SQL Server? If you are building out an API back-end, which of these 2 approaches offers a simpler coding path to interact with the DB?
  I used MongoDB just for learning purposes. I can definitely say MongoDB make things easier, specially when retrieving data from the database directly into your entities. This approach obviously provides a simpler coding path. Anyway, I don't actually find this as a problem with SQL Server.

- Pick from one of these NP-hard questions and give your best-guess response: (A) How do you tell a customer they are wrong without offending them? Or (B) You just went 100 hours over budget ... How do you recover the relationship with your customer (and your boss)?
  B: Getting over budget is not that uncommon and it is most of the times predictable so you can warn your customer before it happens. Anyway, if it happens, you should gather all the evidence that made you spent more hours than expected, making it clear that this overtime was for the sake of delivering a better product. You can also show what could have happened if you didn't spend this overtime in these changes/enhancements.

- Do you have any interest in being exposed to data science projects? Statistically speaking, 95% of respondents say yes to this question, so if you are going to say yes, maybe tell me what interests you in this topic.
  I am definitely interested, since I took two machine learning courses in the last year and I still didn't have the chance to put that knowledge into practice on a real project. Even though ML is not mandatory for data science, it is one of the fields used for analysing large amounts of data.

- How comfortable are you in working on a project that involves touching some CSS and HTML?
  HTML and CSS are both parts of my daily job. Of all the projects I worked in my whole career, only 2 times I had the luck of working with graphics designers. Most of the times I had to develop UIs myself.

- Can you explain GPG, SSL or public/private key encryption?
  GPG: I only know it is a tool that encrypts information in order to transmit it in a secure way.
  SSL: Is a protocol for providing secure communications. We use it all the time on HTTPS sites using SSL certificates. It is currently being replaced by TLS.
  Public/private key encryption: It is a way of encrypting a communication using a pair of keys, where the private one is only known by the receiver of the message.

- Have you had the occasion to undergo any training on "secure coding" practices?
  Yes, 2 times. The first one was a long time ago, I took a course on preventing exploits. I guess this knowledge is now deprecated, since it was intended for C++ native development. The other one was a couple of years ago. It was given by the Microsoft Users Group, which is a crew of specialists spreading Microsoft technologies in my country. It was about secure coding guidelines for web applications. They taught us common flaws, how they are exploited and how to prevent them.

- How enthusiastic would you be if we asked to pay you to take some training courses on Udemy?
  I would like that. There are always new things to learn.

- Which of these platforms / languages / concepts / frameworks do you have experience with (so far)?
  React
  SQL
  Excel
  Python
  Linux
  Mac
  Windows
  .NET
  C#
  NUnit
  PostgreSQL
  MySQL
  SQL Server
  SQLite
  bash
  PowerShell
  MongoDB
  Azure
  AWS
  Google Cloud Platform
  SQLCLR
  SQL Cursors
  CTEs
  SQL Window Functions
  Table Valued Parameters
  SSIS
  SSRS
  ETL
  Encryption
