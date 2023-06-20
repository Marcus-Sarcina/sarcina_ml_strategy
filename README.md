<!-- vscode-markdown-toc -->
* 1. [Project Overview](#ProjectOverview)
* 2. [Problems:](#Problems:)
	* 2.1. [**Problem 1: *Property Rights in Human Capital***](#Problem1:PropertyRightsinHumanCapital)
	* 2.2. [**Problem 2: *Trusted Signals and Search Costs***](#Problem2:TrustedSignalsandSearchCosts)
	* 2.3. [**Problem 3: *Hiring Risk***](#Problem3:HiringRisk)
	* 2.4. [**Problem 4: *Administrative Bloat***](#Problem4:AdministrativeBloat)
* 3. [Addressable Market:](#AddressableMarket:)
	* 3.1. [*"Sarcina is a Gig or Freelancing Platform"*](#SarcinaisaGigorFreelancingPlatform)
	* 3.2. [*"Sarcina is a New Standard for Employment"*](#SarcinaisaNewStandardforEmployment)
	* 3.3. [*"Sarcina is a Property Registrar for Human Capital"*](#SarcinaisaPropertyRegistrarforHumanCapital)
* 4. [Products, Customers, and Business Models:](#ProductsCustomersandBusinessModels:)
	* 4.1. [**The Sarcina App**](#TheSarcinaApp)
	* 4.2. [**The Sarcina Registry**](#TheSarcinaRegistry)
	* 4.3. [**Competitive Advantage**](#CompetitiveAdvantage)
* 5. [Architecture, Security, and Privacy](#ArchitectureSecurityandPrivacy)
* 6. [Data Analysis and Machine Learning Practices and Use Cases for the Sarcina Analytic Environment](#DataAnalysisandMachineLearningPracticesandUseCasesfortheSarcinaAnalyticEnvironment)
	* 6.1. [Datasets available within the Analytic Environment](#DatasetsavailablewithintheAnalyticEnvironment)
	* 6.2. [General approach](#Generalapproach)
	* 6.3. [Use Case: Fraud Detection](#UseCase:FraudDetection)
	* 6.4. [Use Case: Skills Model Improvement](#UseCase:SkillsModelImprovement)
	* 6.5. [Use Case: Identification and Comparison of Expertise](#UseCase:IdentificationandComparisonofExpertise)
	* 6.6. [Use Case: Factoring Price Outcomes](#UseCase:FactoringPriceOutcomes)
	* 6.7. [Anti-Use Case: Recommender System](#Anti-UseCase:RecommenderSystem)
* 7. [State of Development](#StateofDevelopment)

<!-- vscode-markdown-toc-config
	numbering=true
	autoSave=true
	/vscode-markdown-toc-config -->
<!-- /vscode-markdown-toc -->
# Sarcina and it's Analytic Environment
An introduction to the Sarcina Project, it's mission, product and technical design, and a discussion of Data Privacy, Data Analytics, and Machine Learning in Sarcina's Analytic Backend and the Sarcina Registry.


##  1. <a name='ProjectOverview'></a>Project Overview

* **Organization** Sarcina is a privately held corporation founded in 2017 by Marcus Zuech and undisclosed collaborators/partners.

* **Mission** Sarcina's mission is to enhance economic justice and freedom by creating tools which facilitate self-employment and agile distributed business organizations.

* **Origins** The germ of the idea for Sarcina came in 2008, when Marcus observed the burden and duplicative effort imposed on job seekers by conventional corporate recruitment. During that same period, Marcus' brother was struggling to re-establish himself after a series of minor legal troubles, highlighting the degree to which administrative and logistical burdens hamper the lives of low-skilled and economically precarious workers.

* **Initial Product Concept** Mr. Zuech's original vision for what later became the Sarcina Registry imagined a service of impeccable trustworthiness workers might use to cache verified records of their work, education, hobby and volunteer activities as well as the results of often duplicated employment screenings such as drug tests and criminal background checks. Mr. Zuech believed that with enough such data, it would be possible to derive a set of statistically valid and reliable attributes and skills to describe human capital, making the problem of matching workers to jobs simpler and saving both workers and employers substantial friction and cost.

* **Evolution** The design of the Sarcina Protocol and Sarcina Registry have evolved significantly over the years. The concept of the Registry predates the release of Bitcoin, the build-out of cloud computing, and the current generation of big data and machine learning technologies. While conception, research, design, and development towards Sarcina has been ongoing since 2008, Sarcina's current architecture which finally allows for a full realization of the projects vision has only become possible very recently. 

* **Alignment Security** Sarcina's mission has always entailed subverting and disrupting the current system of employment relations and labor discipline. While the proposed systems are in every respect legal and compliant under US law, Sarcina assumes it will face political and commercial pushback for attempting to invalidate deep assumptions of the current economic system. It is critically important to the core project team that the platform not become a tool for surveillance and control as has happened with competing labor platforms, social networks, and cryptocurrency exchanges. As such, Sarcina intends to remain forever a closely held corporation under a mission-driven leader who is at liberty to sacrifice personal and pecuniary interests in order to safeguard the project's vision.

* **Funding** In order to maintain the aforementioned independence, Sarcina does not seek venture capital which would rely on an eventual IPO or acquisition and so Sarcina is funded by the founding team directly until such a time as it becomes self-sustaining through operational revenues.

##  2. <a name='Problems:'></a>Problems:

Sarcina seeks to address several systemic problems in the labor market and in business administration:

###  2.1. <a name='Problem1:PropertyRightsinHumanCapital'></a>**Problem 1: *Property Rights in Human Capital***
####  2.1.1. <a name='Problem:'></a>**Problem:**
> Modern ethics, public opinion, and the 13th Amendment agree that it is not permissable for one person to own the labor potential of another.

> Yet there is no reliable mechanism which establishes an individual's effective control of *their own* human capital. Records pertaining to a person's reputation, skill, trustworthiness, and suitability for a given role may be the moral property of the individual, but are typically held by widely distributed custodians such as schools, former employers, and personal references.
####  2.1.2. <a name='Solution:'></a>**Solution:**
> Create a trustworthy, persistent repository of human capital related data where the worker can submit records for validation and forever retain control of those records' visibility while the content of those records may not be altered by either the worker or the platform operator once the record's veracity is validated to some known standard.

###  2.2. <a name='Problem2:TrustedSignalsandSearchCosts'></a>**Problem 2: *Trusted Signals and Search Costs***
####  2.2.1. <a name='Problem:-1'></a>**Problem:**
> In the current system of labor recruiting, a combination of credentials and experience are used as a proxy for a worker's ability to perform a given job. One year of work or an entire degree program are crude, poorly defined units of measure which are non-fungible and difficult to compare across employers, industries, and educational institutions.

> Workers are incentivized to inflate qualifications while employers are incentivized to define jobs defensively, assuming the minimum level of competence for the experience and credentials they demand. The overall result is that workers invest time and effort into often wasteful signalling activities while employers paint themselves into a corner where the pool of "qualified" applicants is highly restricted compared to the population of workers who might in fact perform a given job well
####  2.2.2. <a name='Solution:-1'></a>**Solution:**
> Given sufficiently granular and structured data about high-frequency labor transactions, it should be possible to impute a model of abstracted skills and labor quality measures which are comparable across different schools, employers, and industries. 

> With this model in place, a worker's experience and education can be used to infer a "character sheet" of granular skills and work habits. Employers will then be able to search the whole space of available workers and adjust the terms and weightings of that search in response to trade-offs between the availability and cost of different factors. Such a model will also give workers feedback on the present market value of their already-proven skills and guidance as to the expected value of additional training or targeted work experience while allowing workers, employers, and education providers to observe trends in the supply and demand of various skills.

###  2.3. <a name='Problem3:HiringRisk'></a>**Problem 3: *Hiring Risk***
####  2.3.1. <a name='Problem:-1'></a>**Problem:**
> For workers to properly "own" their human capital, their value as a contributor should be losslessly portable between employer-customers. Lacking this facility, the labor market has fallen into a pattern where workers attach to a single employer for long periods of time. This puts workers in a condition of low-grade peonage where they are far more dependant on their employer then the employer is on them.

> The two solutions to this condition which have previously been found are unionization and regulation. Both solutions serve to increase the administrative burden and business risk an employer faces when hiring a worker, creating a feedback loop where the labor market slows and employers engage in ever more elaborate practices to protect themselves from liability and maintain discipline over their workforce.

> A slow and defensive labor market presuming long-term, full-time, and exclusive employment means the wages a worker can realize for an hour or day of their time is tied to the amortized value of their contribution across entire months or years. Many workers fill critical roles in their organization which are only periodically performed. If an employer needs a certain skill-set for only an hour a day or one day in a week, the pay they can offer a full-time worker to perform that task will be only a tiny fraction of value created by that worker during the minutes or hours they are actually needed.

> The economy as a whole and workers themselves suffer from the resulting under-utilization of their talents as the highest best use of their labor is idled most of the time.
##### **Second-Order Problems:**
> Incremental employment of independent contractors can itself go a long way towards reducing employer risk and the efficiency of labor allocation. However, this "gig economy" has heretofore earned a poor reputation for two reasons:
> 1. "Gig Apps" are typically created as standalone platforms which target a single type of job. The gig app will usually need to structure and formalize this work to a point where individual gig workers are fungible. As a consequence, gig apps typically target unskilled or low-skill work and are most associated with desperate or precarious workers.
> 2. Because gig apps and freelancing platforms are isolated centralized systems where work history and performance data is seen as an asset of the platform operator rather than the worker, the worker's career advancement from engaging in gig work or freelancing is captive to the platform and confined to whatever rating system or gamification features the platform operator chooses to provide.
####  2.3.2. <a name='Solution:-1'></a>**Solution:**
> The Sarcina Protocol is a crytocurrency-based labor transaction protocol which cryptographically enforces workers and employers control over the use of their respective transaction histories and the portability of these records across both temporary and long-term employment.

> The Sarcina reference app can, with sufficient configuration, be used to intermediate any form of employment relationship. More importantly, Sarcina's client-side engine which implements the Sarcina Protocol and enforces the user(worker or employer)'s rights during the transaction exposes a local API on top of which any number of domain-specific apps can be built.

> This means barriers to entry for a gig app developer are drastically reduced, since building on top of Sarcina provides payment integration, session management, transactional data persistence, user identity management, fraud detection, peer-to-peer networking, and infrastructure hosting at no cost or effort to the developer. All that remains for a developer to do is to analyze some particular job or business function and create the interface and default business rules which will effectively "gigify" it.

> Workers, meanwhile, may use any Sarcina-based app with a single sign on and persistent identity, secure in the knowledge that they are accumulating experience and reputational credit which will enhance all of their employment prospects in the future.

###  2.4. <a name='Problem4:AdministrativeBloat'></a>**Problem 4: *Administrative Bloat***
####  2.4.1. <a name='Problem:-1'></a>**Problem:**
> In the first place, the long-running arms race between employers, employees, regulators, and unions to address the fundamental power imbalance of the employment relationship has imposed upon employers a requirement to maintain a parallel workforce of administrators and lawyers merely to protect themselves from the risk of having employees at all. Work roles are often excessively specialized due to the periodic need to formally adjudicate work performance.

> In the second place, narrow job roles and the systematic under-utilization of full-time workers described above mean that in order to conduct a certain business at a certain scale, an employer has to take on and manage a larger body of full-time workers than they can beneficially employ at any given moment. The "Span of Control" problem means that the layers of management necessary to coordinate an organization grows as a consequence of headcount, whether or not those employees are actively contributing to the value-generating processes of the business.

> Companies in our economy are larger, more bloated, and less efficient than they ought to be in large part because the culture of full-time permanent employment imposes additional administrative and managerial overhead which is not inherent in those companies' domains or business models.
####  2.4.2. <a name='Solution:-1'></a>**Solution:**
> With a standardized, low-friction employment protocol like Sarcina, it will be possible to streamline companies according to their core business activities, with managers allocated funds to hire workers as needed on a minute-by-minute or task-by-task basis. While this will not increase a manager's attentional resources or span of control, it will be possible to maximize the useful output generated within that span. Furthermore, Sarcina automates many of the human resource management, payroll, and accounting functions for which companies currently maintain separate support departments or pay for expensive ERP or SAAS solutions. Use of the Sarcina Registry to find and hire workers can reduce the latency from identifying a labor need to getting a qualified worker on-task from months to minutes.

> Furthermore, the Sarcina protocol, while optimized for labor transactions, can also intermediate B2B or B2C service transactions, software licensing, API access, subscription services, and commission/royalty schemes. This feature can aid in the decentralization of large enterprises into more independent cost and revenue centers without a loss in efficiency or coordination.

##  3. <a name='AddressableMarket:'></a>Addressable Market:
There are at least three distinct ways to conceptualize the addressable market of Sarcina. From smallest to largest:

###  3.1. <a name='SarcinaisaGigorFreelancingPlatform'></a>*"Sarcina is a Gig or Freelancing Platform"*
####  3.1.1. <a name='AddressableMarket:455Billion'></a>Addressable Market: **~$455 Billion**
* If you conceive of Sarcina as a Gig/Freelancing platform, as a marketplace for such platforms, or as infrastructure for such platforms, then the addressable market is the current transacted value on all such platforms.
* According to [Statista](https://www.statista.com/statistics/1034564/gig-economy-projected-gross-volume/), the projected gross volume in the freelance business in 2023 will be $455.2B.
* This perspective is the most useful to understand the market Sarcina is seeking to enter in the near term following it's initial public release.

###  3.2. <a name='SarcinaisaNewStandardforEmployment'></a>*"Sarcina is a New Standard for Employment"*
####  3.2.1. <a name='AddressableMarket:10Trillion'></a>Addressable Market: **~$10 Trillion**
* If you conceive of Sarcina as a general model for employment relations to compete with conventional employment, then the addressable market for Sarcina is the total wages of all workers.
* In the US in 2021, total wages were $9,709,991,000,000 according to [The St. Lois Fed](https://fred.stlouisfed.org/series/BA06RC1A027NBEA)
* This perspective is useful to understand the upper bounds of potential transacted value Sarcina might facilitate in the long term

###  3.3. <a name='SarcinaisaPropertyRegistrarforHumanCapital'></a>*"Sarcina is a Property Registrar for Human Capital"*
####  3.3.1. <a name='AddressableMarket:263TrillionAssetsUnderCustody'></a>Addressable Market: **~$263 Trillion Assets Under Custody**
* Because of the systemic issues described in the "problems" section above, we aren't accustomed to thinking about "Human Capital" as an actual asset class with a formal valuation. But if you conceive of the Sarcina Registry as a sort of banking system or stock exchange where human capital is registered to it's owners and labor values are determined by market exchange, then you can calculate the present value of all existing human capital based on it's expected future cash flows.
> * A typical career lasts approximately 40 years from the end of formal education until the age of retirement, so the pool of all workers can be roughly estimated to have an average of 20 years of remaining working life.
> * From [the same Fed data](https://fred.stlouisfed.org/series/BA06RC1A027NBEA) as before, we can see that our present cash flow to labor is ~$10T/year and that this has grown at an average annual rate of 9% from 1985 to 2021. From the [FRB website](https://www.frbdiscountwindow.org/en/PAges/Discount-Rates/Current-Discount-Rates.aspx) we can see a current discount rate of 5.25% (June, 2023).
> * From these figures, a linear projection suggests that Total Wages in 2041 (average retirement date of current workers / 20 years from our benchmark year of 2021) will be $49.9T with a discounted present value of $17.3T.
* Based on the above assumptions, we can calculate the present value of existing human capital in the US to be $262,864,836,109,208.
* **This measure is not intended to give a realistic estimate of Sarcina's potential growth**, but the fact that the value of human capital thus derived vastly exceeds all other asset classes in the US economy combined goes to underline the points made above about the severe economic miscalculations which are possible under the current regime of ambiguity around property rights in human capital.

##  4. <a name='ProductsCustomersandBusinessModels:'></a>Products, Customers, and Business Models:
###  4.1. <a name='TheSarcinaApp'></a>**The Sarcina App**
Sarcina's initial product, to be marketed to the public as "Sarcina" is best described as a peer-to-peer teleconferencing and chat app with a time-incremented payment layer. The organizing analogy of Sarcina calls is that of the old 900-number system; the offer of services exists outside of the call and a customer is automatically charged a pre-disclosed rate per minute for time spent connected.

The invitation to join a Sarcina call is an embeddable configuration file called a "**line**". The line file describes, in condensed, machine-readable form, the following information:
* The public key of the issuer of the line, which serves as a user's anonymous identifier to the Sarcina ecosystem.
* (optional) A link to the issuer's Sarcina Registry profile, once the Registry is in operation.
* Details required to establish an encrypted peer-to-peer streaming connection to the issuer through Sarcina's anonymous, surveillance-hardened "phone book" infrastructure.
* (optional) A description of the purpose and services provided when connecting to the line.
* A set of business rules governing connections to the line such as the price per minute or per message, restrictions on who can connect, hours of operation, and the data streams included in the offer (audio, video, text, geo-location, file transfer, remote desktop, SSL, etc).
* (optional) Any third-party certificates which endorse the service provider issuing the line.

Line files are small, suitable for being attached to email, embedded in a website, or hosted in an etherpad or public git repository for distribution as a hyperlink. Any user with a copy of the Sarcina client can parse the line file to review the terms of the line before connecting. As such, a Sarcina line serves as an adhesion contract, requiring no further negotiation of terms once the users connect.

Each user's Sarcina client is connected to the third-party cryptocurrency wallet of their choice, and a peer-to-peer micropayment channel in the background settles payment automatically as the call proceeds. Each user's client also enforces the terms of the call as described in the line file, ensuring that as long as the connection proceeds and neither user chooses to disconnect, that the services described in the line file are being provided to the satisfaction of the parties.

All steps in the connection and call process are as anonymous and surveillance-resistant as possible with current technology. Centralized infrastructure is only involved for necessarily centralized functions such as translating user IDs to network addresses and providing a common network-wide exchange rate for supported cryptocurrencies. As such, Sarcina is highly resistant to surveillance or suppression and the Sarcina platform is incapable of restricting the use of the service by anyone with a computer and a copy of the client software.
####  4.1.1. <a name='SarcinaAppLaunchStrategy'></a>Sarcina App Launch Strategy
The Sarcina app will be marketed to three groups initially: Content creators and recognized experts, freelancers, and app developers.

***Influencers/Content Creators***

Marketing expenditure will focus on the first group, people whose time and attention are already in demand and who may be looking for a way to monetize their fame which is free of platform risk and lock-in. These are the most valuable possible users since they will be motivated to recruit followers and fans to Sarcina as part of their own monetization efforts, yielding a disproportional payoff in network growth.

Because Sarcina supports recurring subscriptions as well as hands-off downloads or streaming, it works out-of-the-box as a replacement for existing monetization options like Patreon, OnlyFans, YouTube SuperChats, e-Book or other content sales, or subscription blogs.

While dealing with cryptocurrency instead of cash imposes some friction and inconvenience and restricts the potential pool of customers, Sarcina offers a level of suppression resistance which cannot be matched by any platform connected to the conventional banking system no matter how ethical the platform operator may be. As such, it is expected Sarcina will be used as a secondary, premium, or "fallback" monetization option by early adopting influencers who are concerned about de-platforming risk.

***Freelancers***

Sarcina's landing page and documentation focuses on the non-famous freelancer earning their living through remote work using their software. In the long term, Sarcina sees freelancers along with white-label app developers as the core of its business.

Because freelancers are a much larger and more dispersed population than influencers and because they are not usually in a position to dictate platform adoption to their customers, Sarcina markets passively to them through its website, blog, and general online brand rather than through ad buys or other cost-incurring campaigns. The hope is that with time, as the installed base of Sarcina clients grows from people consuming content or connecting to their favorite influencers, use of Sarcina to hire freelancers will become less frictional as the software is more familiar to the public.

***Whitelabel App Developers***

As mentioned above, the Sarcina App is composed of two parts:
1. The conventional UI layer
1. The compiled Sarcina Engine

All network, security, payment, file access, call management, and media handling functions are implemented within the engine, which exposes a local API over which any number of alternative UI layers may be wrapped.

Third party developers can construct any number of "gig apps" as re-skins of the internal API with customized business rules and defaults, mixing in external services or resources to a user workflow tailored to a particular application. In this model, the whitelabel developer can use the certificate function of the Sarcina Protocol to embed an additional transaction fee for themselves when users connect using their version of the Sarcina client.

Third-party developers can also build or import various kinds of business software as extensions to a modified Sarcina UI. To monetize this approach, a developer might use Sarcina's automated subscription functionality to obtain payment for the use to their enhancements.

As is the case with end-users, the app is designed to make it structurally impossible for the Sarcina organization to suppress or gatekeep access by third-party developers.

Marketing efforts targeted at third party developers will be slower and more deliberate and hands-on. A developer guide will be released as part of the initial whitepaper, and anyone and everyone is encouraged to hack on the non-engine portion of the client software. However, members of the core Sarcina development team will only be making themselves available to skilled and serious teams who they believe will produce ethical and high-quality products.
###  4.2. <a name='TheSarcinaRegistry'></a>**The Sarcina Registry**
Sarcina's second product will be the Sarcina Registry, an information service where users can opt-in to have their aggregate past performance, imputed skills, and trustworthiness displayed.

The Sarcina Registry will be like LinkedIn, if the information on LinkedIn were true.

Users of Sarcina do not have to register with the Sarcina Registry (in fact, they do not have to register with Sarcina at all), but if they opt to do so, they will be able to decrypt and retrieve their own validated transaction history on the network and have their imputed "character sheet" displayed publicly. This will allow potential employers to find them through a granular search function and hire them through whichever public lines they choose to publish on their registry profile. It will also serve as an indelible online resume with a high degree of trustworthiness and verification behind it.

Whether users choose to join the Registry or not, the transaction records from which registry profiles are imputed are stripped of all identifying information at the point of receipt and so the Sarcina organization will not be capable of unmasking, excluding, or modifying transaction records of anonymous users (If a user chooses to put e.g. legal name or physical location on their public Registry profile, that is on them).
####  4.2.1. <a name='RegistryLaunch'></a>*Registry Launch*
Because the goal of the Registry is to provide valid and trustworthy assessments of worker's skills and trustworthiness, the models which support this will not be functional until there is a sufficiently large dataset of Sarcina transaction records. As a consequence, the Sarcina Registry will not be released until the Sarcina App has achieved sufficient market penetration and transaction volume to provide this data.
####  4.2.2. <a name='RegistryBusinessModel'></a>*Registry Business Model*
Revenues from the Sarcina registry will come from increased transaction volume on the app and also from paid encoding services. An encoding service is one where a user submits off-platform data such as diplomas or work history or pays for third-party screenings such as standardized test scores, drug screenings, or criminal background checks to be reported to the encoding service provider. 

Encoding services will be provided by third-party bonded validation partners trusted by the Sarcina organization, since Sarcina itself does not wish to ever collect PII or real-world metadata that might be used to unmask pseudonymous users. Once validated, these records will be dis-aggregated into the same skills/attributes model Sarcina uses to represent on-platform performance.
###  4.3. <a name='CompetitiveAdvantage'></a>**Competitive Advantage**
At launch, Sarcina has several characteristics which differentiate it from what a conventional "tech company" or "startup" is likely to offer. All of these follow from the Sarcina organization being a small team of mission-driven activists:

The first is extremely low transaction fees. Sarcina as a platform takes only a 1% transaction fee which, when using a low-cost cryptocurrency option such as BTC via Lightning Network, means a cost to the service provider of less than 1.2% of the transacted value. This is less than the credit card processing fees payed by any credit card based product and far less than the fees a company would have to charge to support a paid development team, much less a "growing startup with a great company culture".

The Sarcina Project is committed to privacy, pseudonymity, and permissionless access in the labor market to a degree which would be seen as too risky and potentially inflammatory by most investors or public companies.

The architecture of Sarcina optimizes for the autonomy of the user and the user's control of their data to a degree which sacrifices much of the value and revenue potential platform operators have grown to expect. Any commercial competitor who attempts to replicate Sarcina's functionality should be assumed to be engaging in some level of surveillance, suppression, or data brokerage unless proven otherwise.

The Sarcina organization intends to remain small and to maintain the core infrastructure and client engine as a basic economic utility on close to a break-even basis. Non-central functions such as developer/integrator training, user support, and encoding services will be allocated to separate trusted organizations.

Most revenues in excess of operations costs and developer or marketing salaries will be reinvested into marketing campaigns, grants to whitelabel Sarcina startups, or reduced fees. Sarcina measures it's success as a project not by profits or equity valuation but by the fraction of the labor market where norms of worker sovereignty, permissionless access, and pseudonymity reign. 

##  5. <a name='ArchitectureSecurityandPrivacy'></a>Architecture, Security, and Privacy

A brief walkthrough of the Sarcina architecture to highlight it's security and privacy features and explain the character of the data which will be available to the Sarcina Analytic Environment: 

**The Sarcina App Front End**

The UI layer with which the user interacts is not itself trusted and it is this layer where modding and re-skinning are encouraged. The lower "engine" layer contains a limited amount of UI code so that it can "burst through" for security critical interactions such as authorizing payments.

**The Sarcina Engine**

The Sarcina Engine is a set of local services which implement the network, transaction management, key management, and rules enforcement functions which allow connections via the Sarcina Protocol. It is written in Rust and compiled to WASM and is expected to be distributed directly from a source certified the the Sarcina organization, either by itself or packaged with the reference UI. It is important that the user trusts their local installation of the Sarcina Engine since it is at this layer that their funds and identity are secured and persisted and it is the engine which enforces the user's rights according to the terms of any line they connect to.

In the reference client, only the engine connects to the internet. The engine makes all necessary connections to Sarcina's support services and holds the various peer-to-peer streams which constitute a Sarcina call. The engine also manages and persists user keys and trusted data such as copies of issued lines. The engine holds a WalletConnect connection to whichever local cryptocurrency wallet the user designates during setup.

**Core Support Services**

Certain centralized services are required in order for Sarcina users to connect and complete calls. Among these is a lookup facility to find current IP addresses of users given their public keys and a common oracle to quote exchange rates of various supported cryptocurrencies to USD so that both parties to a call will calculate the same expected payments given the terms of the line file.

Since this is an obvious weak point in the decentralization and hardening of the network, significant engineering effort has been invested in making these services as trustworthy as possible:
1. Core services are hosted on [Dfinity's IC platform](https://support.dfinity.org/hc/en-us/articles/360057403152-What-is-DFINITY-), which provides a number of benefits:
    - The Sarcina organization is not in control of the hosting environment and the host is not capable of invisibly modifying the content of or traffic to Sarcina's deployed canisters due to the blockchain based governance of the IC network.
    - Deployed canisters are set to an immutable status such that they may not be later altered. Later releases of the core services will happen infrequently and prior versions of the services will remain available as long as users are regularly connecting to keep them funded (see below). A consequence of this feature, along with the thick client design of the Sarcina App is that **even if the the Sarcina Organization is in some way compromised, it will never be able to forcibly upgrade users to a less private or less secure version of the platform**.
    - While not "open source" in the sense of being free to use, the code implementing Sarcina's core services will be made available for examination, allowing interested parties to re-compile the deployed binaries in a deterministic environment and compare checksums with those visible in the deployment transaction to the ICP blockchain. This will create a level of confidence unprecedented in online services in that **users will be able to know with certainty what code is actually running on the services they connect to**.
2. Transaction records are first validated and then provably anonymized at the time of receipt before they are ever exposed to Sarcina's internal systems or accessible by Sarcina staff.
    - Call reports are held in the reporting canister and thus outside of Sarcina organization's control until the payment details are verified against whichever public blockchain the call was settled on. After that, all identifying information is either dropped or anonymized behind a proxy key which can only be generated by the reporting user before the record is shipped to Sarcina's analytic environment.
    - Since the code implementing Sarcina's reporting service is inspectable and verifiable as described above, users can be confident that **Sarcina holds no records which can be tied to their persistent user ID, cryptocurrency addresses, geographical location, or any other potentially identifying information** until such a time as the user chooses to retrieve their performance history by joining the Registry and providing the proxy key.
3. Core services are, to the extent possible, self-funding, with the goal that core services and therefor **the Sarcina App as a whole should be able to continue working even is the Sarcina organization is disrupted for some reason**.
    - An initial endowment of ICP token is deposited by the Sarcina organization at the time of deployment which should be sufficient to cover the IC gas fees for tens of millions of completed calls.
    - Each new user who starts reporting their IP (which only occurs when their client has an active line offer on file) is granted an initial credit sufficient to fund roughly a thousand lookups. 
    - Once this credit is depleted, the user (who is by now assumed to have earned thousands of tens of thousands of dollars through Sarcina) will be prompted to authorize a payment (estimated at $5) to replenish their credit and continue receiving calls. The canister handling funding transactions and performing the conversion to ICP is also immutable, inspectable, and non-logging.
    - In this way, the core services can self-fund indefinitely without financial intervention from the Sarcina organization.

**The Sarcina Analytic Environment**

Once verified and anonymized, transaction records are shipped to Sarcina's analytic environment where they are archived for eventual recovery to the Registry and analyzed to identify fraud, to dis-aggregate experience into granular skills, and to develop and improve models and tools for those purposes. Since this is a research setting, the specific architecture and processes running in the analytic environment will change continuously.

Activities in the analytic environment are discussed in greater detail below.

**The Sarcina Registry**.
The Sarcina Registry will be a separate, non-immutable IC-based application where web and API access to registered users' designated public profiles will be provided.
> **Note on the principle of privacy in the Sarcina ecosystem**
> The design of the Sarcina network has been optimized to the extent currently possible to inhibit bulk collection or retroactive surveillance of user data and to give confidence to Sarcina users that the platform itself is neutral, incorruptible, and respectful  user's data sovereignty and privacy.

> Some exposure of user data is implicit in the service, such as the exposure of a user's current IP address to their counterparty in a call or the exposure of a user's timezone to those who attempt to connect to them according to their hours of operation. Users who feel they need a greater degree of obscurity than Sarcina can provide are encouraged to take additional precautions to obscure whatever data they are concerned about.

> The Sarcina organization is not responsible for and does not encourage illicit or scandalous activity on their platform, and is not building that platform with the desires of such users in mind.

##  6. <a name='DataAnalysisandMachineLearningPracticesandUseCasesfortheSarcinaAnalyticEnvironment'></a>Data Analysis and Machine Learning Practices and Use Cases for the Sarcina Analytic Environment

###  6.1. <a name='DatasetsavailablewithintheAnalyticEnvironment'></a>Datasets available within the Analytic Environment
1. Call records
	1. Proxy user IDs for all parties to the call
	1. Unmasked user IDs for certificate issuers involved in the call
	1. Business rules governing the call, including certificate terms
	1. Reduced precision start and stop times of the call
	1. Transacted value in USD broken out by individual payer and payee
	1. Structured service category and sub-category indicated in the line description
	1. Unstructured description text from the line description
	1. Structured post-call performance assessment responses
	1. Unstructured post-call performance assessment responses
	1. Engine and Infrastructure version of each participant
1. Data imported from the Registry (registered users only)
	1. Low-precision physical location (metro area or postal code)
	1. Unstructured description text
	1. Active and inactive public line offers
	1. Unconfirmed details of education, certification, or work experience
	1. Confirmed details of education, certification, or work experience

###  6.2. <a name='Generalapproach'></a>General approach
Analysis of Sarcina's records will lean heavily on both conventional and machine learning approached to graph analysis of the relations between users. The aim will be to bootstrap meaningful attributes and taxonomies of activity from commonalities in patterns of communications, building off the seed of user provided data such as reported occupations and reported quality of service.

Both supervised and unsupervised learning approaches will have a role to play in extracting the true variables and their relationships from this combination of attested but unreliable human-labeled structured data and unlabeled graph topology.

The aim of any ML model used on Sarcina data will be to bring forth some deterministically describable feature or relationship in the data. Sarcina will, as a matter of policy, not use any large, uninterpretable "black box" models to make judgments about user data.

Instead, narrow models will be trained to predict outcomes or identify common factors and will then be interrogated, either by direct examination, combinatorial challenge batteries, or adversarial models in order to extract a compact description of the patterns the model has recognized. Only once such patterns can be described deterministically can it be determined whether the patterns triggering accurate model output represent legitimate insights about the domain under examination.

###  6.3. <a name='UseCase:FraudDetection'></a>Use Case: Fraud Detection
Sarcina will work continuously to identify fraudulent users and low-quality service providers and to develop tools to algorithmically identify patterns indicating fraudulent behavior of users.

Though Sarcina is not able to take direct action against fraudulent or incompetent users, it is important to identify such users and transactions in order to (1) exclude fraudulent transactions from the data sets used for other functions and (2) adjust the imputed trustworthiness of users engaging in suspicious behavior if those users also create Registry accounts (3) take steps to harden Sarcina's analysis chain against exploits.

###  6.4. <a name='UseCase:SkillsModelImprovement'></a>Use Case: Skills Model Improvement
Because data from the Sarcina App can not be tied to conventional credentials or legal identities, the model used to describe worker attributes will need to be bootstrapped from the call report data Sarcina receives. This will provide a unique opportunity to recapitulate the categorization of human expertise free from the incumbent institutional models.

Seeding it's interface options with terms and categories drawn from existing models such as [O*Net](https://www.onetonline.org/), Sarcina will be able to observe directly which keywords, job titles, and other descriptors correlate to success and earnings in the market, which do not, which descriptors conflate functionally distinct factors, and which make distinctions which do no in fact exist.

###  6.5. <a name='UseCase:IdentificationandComparisonofExpertise'></a>Use Case: Identification and Comparison of Expertise
An additional strategy will be to use graph analysis of users and their transactions to identify benchmark individuals claiming to practice a given occupation who are strongly connected to a network of individuals who claim the same or related occupations. Even without knowing the personal details or formal qualifications of such individuals, Sarcina will be able to develop confidence that such a person is a genuine and successful practitioner and thus use the pattern of their activity to assess the activities of others claiming to practice the same occupation.

It is hoped that sufficiently mature pattern-recognizing models based on this dataset will be able to perceive resonances between different fields and thus aid workers in identifying value-positive career changes which might suit their temperaments and abilities or suggest non-intuitive search terms to potential employers using the Registry. 

> **Note about the Registry Skills model:** In order to make a clear distinction between reported and imputed data, the Sarcina Registry uses a two-dimensional descriptor for user skills and attributes. The first dimension is magnitude - the level of experience reported to Sarcina by various channels. The second attribute is veracity - the level of confidence that the Registry has in the reported magnitude of the attribute. 

###  6.6. <a name='UseCase:FactoringPriceOutcomes'></a>Use Case: Factoring Price Outcomes
Having burnished it's empirical model of human capital factors, Sarcina will be in a position to identify the impact of attributes at various levels of magnitude on the volume and financial value of work obtained, both in isolation as as part of common patterns of qualification and network participation.

###  6.7. <a name='Anti-UseCase:RecommenderSystem'></a>Anti-Use Case: Recommender System
Sarcina does not intend to build a matching or recommender system to "assign" workers to jobs or to draw conclusions about who is or is not qualified for a particular task. Instead, the aim is to generate an easily manipulable palette of data visualization tools with which workers and employers can explore the space of productive work and human capital so that users can project their own intuitions and insights about their particular needs, abilities, and interests. Sarcina's belief is that by taking the element of authority out of the question of who ought to perform which work, greater insight will emerge from the organic feedback of rapid, low-friction hiring and dismissal.

##  7. <a name='StateofDevelopment'></a>State of Development
Sarcina is currently in the process of developing it's initial public Sarcina App. The core service layer is complete, as is the primary structure and system integration of the Client Engine. 

Sarcina is currently aiming for a Fall-Winter 2023 soft launch of a headless Engine and Core Service stack for use by whitelabel developers, with the full user-facing app to follow in 2024. 