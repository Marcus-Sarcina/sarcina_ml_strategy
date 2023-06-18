# Sarcina and it's Analytic Environment
An introduction to the Sarcina Project, it's mission, and a discussion of Data Privacy, Data Analytics, and Machine Learning in Sarcina's Analytic Backend and the Sarcina Registry.


## Project Overview

* **Organization** Sarcina is a privately held corporation founded in 2017 by Marcus Zuech and undisclosed collaborators/partners.

* **Mission** Sarcina's mission is to enhance economic justice and freedom by creating tools which facilitate self-employment and agile distributed business organizations.

* **Origins** The germ of the idea for Sarcina came in 2008, when Marcus observed the burden and duplicative effort imposed on job seekers by conventional corporate recruitment. During that same period, Marcus' brother was struggling to re-establish himself after a series of minor legal troubles, highlighting the degree to which administrative and logistical burdens hamper the lives of low-skilled and economically precarious workers.

* **Initial Product Concept** Mr. Zuech's original vision for what later became the Sarcina Registry imagined a service of impeccable trustworthiness workers might use to cache verified records of their work, education, hobby and volunteer activities as well as the results of often duplicated employment screenings such as drug tests and criminal background checks. Mr. Zuech believed that with enough such data, it would be possible to derive a set of statistically valid and reliable attributes and skills to describe human capital, making the problem of matching workers to jobs simpler and saving both workers and employers substantial friction and cost.

* **Evolution** The design of the Sarcina Protocol and Sarcina Registry have evolved significantly over the years. The concept of the Registry predates the release of Bitcoin, the build-out of cloud computing, and the current generation of big data and machine learning technologies. While conception, research, design, and development towards Sarcina has been ongoing since 2008, Sarcina's current architecture which finally allows for a full realization of the projects vision has only become possible very recently. 

* **Alignment Security** Sarcina's mission has always entailed subverting and disrupting the current system of employment relations and labor discipline. While the proposed systems are in every respect legal and compliant under US law, Sarcina assumes it will face political and commercial pushback for attempting to invalidate deep assumptions of the current economic system. It is critically important to the core project team that the platform not become a tool for surveillance and control as has happened with competing labor platforms, social networks, and cryptocurrency exchanges. As such, Sarcina intends to remain forever a closely held corporation under a mission-driven leader who is at liberty to sacrifice personal and pecuniary interests in order to safeguard the project's vision.

* **Funding** In order to maintain the aforementioned independence, Sarcina does not seek venture capital which would rely on an eventual IPO or acquisition and so Sarcina is funded by the founding team directly until such a time as it becomes self-sustaining through operational revenues.

## Problems:

Sarcina seeks to address several systemic problems in the labor market and in business administration:

### **Problem 1: *Property Rights in Human Capital***
#### **Problem:**
> Modern ethics, public opinion, and the 13th Amendment agree that it is not permissable for one person to own the labor potential of another.

> Yet there is no reliable mechanism which establishes an individual's effective control of their *own* human capital. Records pertaining to a person's reputation, skill, trustworthiness, and suitability for a given role may be the moral property of the individual, but are typically held by widely distributed custodians such as schools, former employers, and personal references.
#### **Solution:**
> Create a trustworthy, persistent repository of human capital related data where the worker can submit records for validation and forever retain control of those records' visibility while the content of those records may not be altered by either the worker or the platform operator once the record's veracity is validated to some known standard.

### **Problem 2: *Trusted Signals and Search Costs***
#### **Problem:**
> In the current system of labor recruiting, a combination of credentials and experience are used as a proxy for a worker's ability to perform a given job. One year of work or an entire degree program are crude, poorly defined units of measure which are non-fungible and difficult to compare across employers, industries, and educational institutions.

> Workers are incentivized to inflate qualifications while employers are incentivized to define jobs defensively, assuming the minimum level of competence for the experience and credentials they demand. The overall result is that workers invest time and effort into often wasteful signalling activities while employers paint themselves into a corner where the pool of "qualified" applicants is highly restricted compared to the population of workers who might in fact perform a given job well
#### **Solution:**
> Given sufficiently granular and structured data about high-frequency labor transactions, it should be possible to impute a model of abstracted skills and labor quality measures which are comparable across different schools, employers, and industries. 

> With this model in place, a worker's experience and education can be used to infer a "character sheet" of granular skills and work habits. Employers will then be able to search the whole space of available workers and adjust the terms and weightings of that search in response to trade-offs between the availability and cost of different factors. Such a model will also give workers feedback on the present market value of their already-proven skills and guidance as to the expected value of additional training or targeted work experience while allowing workers, employers, and education providers to observe trends in the supply and demand of various skills.

#### **Problem 3: *Hiring Risk***
#### **Problem:**
> For workers to properly "own" their human capital, their value as a contributor should be losslessly portable between employer-customers. Lacking this facility, the labor market has fallen into a pattern where workers attach to a single employer for long periods of time. This puts workers in a condition of low-grade peonage where they are far more dependant on their employer then the employer is on them.

> The two solutions to this condition which have previously been found are unionization and regulation. Both solutions serve to increase the administrative burden and business risk an employer faces when hiring a worker, creating a feedback loop where the labor market slows and employers engage in ever more elaborate practices to protect themselves from liability and maintain discipline over their workforce.

> A slow and defensive labor market presuming long-term, full-time, and exclusive employment means the wages a worker can realize for an hour or day of their time is tied to the amortized value of their contribution across entire months or years. Many workers fill critical roles in their organization which are only periodically performed. If an employer needs a certain skill-set for only an hour a day or one day in a week, the pay they can offer a full-time worker to perform that task will be only a tiny fraction of value created by that worker during the minutes or hours they are actually needed.

> The economy as a whole and workers themselves suffer from the resulting under-utilization of their talents as the highest best use of their labor is idled most of the time.
##### **Second-Order Problems:**
> Incremental employment of independent contractors can itself go a long way towards reducing employer risk and the efficiency of labor allocation. However, this "gig economy" has heretofore earned a poor reputation for two reasons:
> 1. "Gig Apps" are typically created as standalone platforms which target a single type of job. The gig app will usually need to structure and formalize this work to a point where individual gig workers are fungible. As a consequence, gig apps typically target unskilled or low-skill work and are most associated with desperate or precarious workers.
> 2. Because gig apps and freelancing platforms are isolated centralized systems where work history and performance data is seen as an asset of the platform operator rather than the worker, the worker's career advancement from engaging in gig work or freelancing is captive to the platform and confined to whatever rating system or gamification features the platform operator chooses to provide.
#### **Solution:**
> The Sarcina Protocol is a crytocurrency-based labor transaction protocol which cryptographically enforces workers and employers control over the use of their respective transaction histories and the portability of these records across both temporary and long-term employment.

> The Sarcina reference app can, with sufficient configuration, be used to intermediate any form of employment relationship. More importantly, Sarcina's client-side engine which implements the Sarcina Protocol and enforces the user(worker or employer)'s rights during the transaction exposes a local API on top of which any number of domain-specific apps can be built.

> This means barriers to entry for a gig app developer are drastically reduced, since building on top of Sarcina provides payment integration, session management, transactional data persistence, user identity management, fraud detection, peer-to-peer networking, and infrastructure hosting at no cost or effort to the developer. All that remains for a developer to do is to analyze some particular job or business function and create the interface and default business rules which will effectively "gigify" it.

> Workers, meanwhile, may use any Sarcina-based app with a single sign on and persistent identity, secure in the knowledge that they are accumulating experience and reputational credit which will enhance their employment prospects in the future.

#### **Problem 4: *Administrative Bloat***
#### **Problem:**
> In the first place, the long-running arms race between employers, employees, regulators, and unions to address the fundamental power imbalance of the employment relationship has imposed upon employers a requirement to maintain a parallel workforce of administrators and lawyers merely to protect themselves from the risk of having employees at all. Work roles are often excessively specialized due to the periodic need to formally adjudicate work performance.

> In the second place, narrow job roles and the systematic under-utilization of full-time workers described above mean that in order to conduct a certain business at a certain scale, an employer has to take on and manage a larger body of full-time workers than they can beneficially employ at any given moment. The "Span of Control" problem means that the layers of management necessary to coordinate an organization grows as a consequence of headcount, whether or not those employees are actively contributing to the value-generating processes of the business.

> Companies in our economy are larger, more bloated, and less efficient than they ought to be in large part because the culture of full-time permanent employment imposes additional administrative and managerial overhead which is not inherent in those companies' domains or business models.
#### **Solution:**
> With a standardized, low-friction employment protocol like Sarcina, it will be possible to streamline companies according to their core business activities, with managers allocated funds to hire workers as needed on a minute-by-minute or task-by-task basis. While this will not increase a manager's attentional resources or span of control, it will be possible to maximize the useful output generated within that span. Furthermore, Sarcina automates many of the human resource management, payroll, and accounting functions for which companies currently maintain separate support departments or pay for expensive SAAS solutions. Use of the Sarcina Registry to find and hire workers can reduce the latency from identifying a labor need to getting a qualified worker on-task from months to minutes.

> Furthermore, the Sarcina protocol, while optimized for labor transactions, can also intermediate B2B or B2C service transactions, software licensing, API access, subscription services, and commission/royalty schemes. This feature can aid in the decentralization of large enterprises into more independent cost and revenue centers without a loss in efficiency or coordination.

## Addressable Market:
There are at least three distinct ways to conceptualize the addressable market of Sarcina. From smallest to largest:

### *"Sarcina is a Gig or Freelancing Platform"*
#### Addressable Market: **~$455 Billion**
* If you conceive of Sarcina as a Gig/Freelancing platform, as a marketplace for such platforms, or as infrastructure for such platforms, then the addressable market is the current transacted value on all such platforms.
* According to [Statista](https://www.statista.com/statistics/1034564/gig-economy-projected-gross-volume/), the projected gross volume in the freelance business in 2023 will be $455.2B.
* This perspective is the most useful to understand the market Sarcina is seeking to enter in the near term following it's initial public release.

### *"Sarcina is a New Standard for Employment"*
#### Addressable Market: **~$10 Trillion**
* If you conceive of Sarcina as a general model for employment relations to compete with conventional employment, then the addressable market for Sarcina is the total wages of all workers.
* In the US in 2021, total wages were $9,709,991,000,000 according to [The St. Lois Fed](https://fred.stlouisfed.org/series/BA06RC1A027NBEA)
* This perspective is useful to understand the upper bounds of potential transacted value Sarcina might facilitate in the long term

### *"Sarcina is a Property Registrar for Human Capital"*
#### Addressable Market: **~$263 Trillion Assets Under Custody**
* Because of the systemic issues described in the "problems" section above, we aren't accustomed to thinking about "Human Capital" as an actual asset class with a formal valuation. But if you conceive of the Sarcina Registry as a sort of banking system or stock exchange where human capital is registered to it's owners and labor values are determined by market exchange, then you can calculate the present value of all existing human capital based on it's expected future cash flows.
> * A typical career lasts approximately 40 years from the end of formal education until the age of retirement, so the pool of all workers can be roughly estimated to have an average of 20 years of remaining working life.
> * From [the same Fed data](https://fred.stlouisfed.org/series/BA06RC1A027NBEA) as before, we can see that our present cash flow to labor is ~$10T/year and that this has grown at an average annual rate of 9% from 1985 to 2021. From the [FRB website](https://www.frbdiscountwindow.org/en/PAges/Discount-Rates/Current-Discount-Rates.aspx) we can see a current discount rate of 5.25% (June, 2023).
> * From these figures, a linear projection suggests that Total Wages in 2041 (average retirement date of current workers / 20 years from our benchmark year of 2021) will be $49.9T with a discounted present value of $17.3T.
* Based on the above assumptions, we can calculate the present value of existing human capital in the US to be $262,864,836,109,208.
* **This measure is not intended to give a realistic estimate of Sarcina's potential growth**, but the fact that the value of human capital thus derived vastly exceeds all other asset classes in the US economy combined goes to underline the points made above about the severe economic miscalculations which are possible under the current regime of ambiguity around property rights in human capital.

## Products, Customers, and Business Models:
### **The Sarcina App**
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
### Sarcina App Launch Strategy
The Sarcina app will be marketed to three groups initially: Content creators and recognized experts, freelancers, and app developers.

#### *Influencers/Content Creators*
Marketing expenditure will focus on the first group, people whose time and attention are already in demand and who may be looking for a way to monetize their fame which is free of platform risk and lock-in. These are the most valuable possible users since they will be motivated to attract their followers and fans to Sarcina as part of their own monetization efforts, yielding a disproportional payoff in network growth.

Because Sarcina supports recurring subscriptions as well as hands-off downloads or streaming, it works out-of-the-box as a replacement for existing monetization options like Patreon, OnlyFans, YouTube SuperChats, e-Book or other content sales, or subscription blogs.

While dealing with cryptocurrency instead of cash imposes some friction and inconvenience and restricts the potential pool of customers, Sarcina offers a level of suppression resistance which cannot be matched by any platform connected to the conventional banking system no matter how ethical the platform operator may be. As such, it is expected Sarcina will be used as a secondary, premium, or "fallback" monetization option by early adopting influencers who are concerned about de-platforming risk.
#### *Freelancers*
Sarcina's landing page and documentation focuses on the non-famous freelancer earning their living through remote work using their software. In the long term, Sarcina sees freelancers along with white-label app developers as the core of its business.

Because freelancers are a much larger and more dispersed population than influencers and because they are not usually in a position to dictate platform adoption to their customers, Sarcina markets passively to them through its website, blog, and general online brand rather than through ad buys or other cost-incurring campaigns. The hope is that with time, as the installed base of Sarcina clients grows from people consuming content or connecting to their favorite influencers, use of Sarcina to hire freelancers will become less frictional as the software is more familiar to the public.
#### *Whitelabel App Developers*
As mentioned above, the Sarcina App is composed of two parts:
1. The conventional UI layer
1. The compiled Sarcina Engine

All network, security, payment, file access, call management, and media handling functions are implemented within the engine, which exposes a local API over which any number of alternative UI layers may be wrapped.

Third party developers can construct any number of "gig apps" as re-skins of the internal API with customized business rules and defaults, mixing in external services or resources to a user workflow tailored to their application. In this model, the whitelabel developer can use the certificate function of the Sarcina Protocol to embed an additional transaction fee for themselves when users connect using their version of the Sarcina client.

Third-party developers can also build or import various kinds of business software as extensions to a modified Sarcina UI. To monetize this approach, a developer might use Sarcina's automated subscription functionality to obtain payment for the use to their enhancements.

As is the case with end-users, the app is designed to make it structurally impossible for the Sarcina organization to suppress or gatekeep access by third-party developers.

Marketing efforts targeted at third party developers will be slower and more deliberate and hands-on. A developer guide will be released as part of the initial whitepaper, and anyone and everyone is encouraged to hack on the non-engine portion of the client software. However, members of the core Sarcina development team will only be making themselves available to skilled and serious teams who they believe will produce high-quality products.
### **The Sarcina Registry**
Sarcina's second product will be the Sarcina Registry, an information service where users can opt-in to have their aggregate past performance, imputed skills, and trustworthiness displayed.

The Sarcina Registry will be like LinkedIn, except statistically valid.

Users of Sarcina do not have to register with the Sarcina Registry (in fact, they do not have to register with Sarcina at all), but if they opt to do so, they will be able to decrypt and retrieve their own validated transaction history on the network and have their imputed "character sheet" displayed publicly. This will allow potential employers to find them through a granular search function and contact them through whichever public lines they choose to publish on their registry profile. It will also serve as an indelible online resume with a high degree of trustworthiness and verification behind it.

Whether users choose to join the Registry or not, the transaction records from which registry profiles are imputed are stripped of all identifying information at the point of receipt and so the Sarcina organization will not be capable of unmasking, excluding, or modifying transaction records of anonymous users (If a user chooses to put e.g. legal name or physical location on their public Registry profile, that is on them).
#### *Registry Launch*
Because the goal of the Registry is to provide valid and trustworthy assessments of worker's skills and trustworthiness, the models which support this will not be functional until there is a sufficiently large dataset of Sarcina transaction records. As a consequence, the Sarcina Registry will not be released until the Sarcina App has achieved sufficient market penetration and transaction volume to provide this data.
#### *Registry Business Model*
Revenues from the Sarcina registry will come from increased transaction volume on the app and thus increased fees and also from paid encoding services. An encoding service is one where a user submits off-platform data such as diplomas or work history or pays for third-party screenings such as standardized test scores, drug screenings, or criminal background checks to be reported to the encoding service provider. 

Encoding services will be provided by third-party bonded validation partners trusted by the Sarcina organization, since Sarcina itself does not wish to ever collect PII or real-world metadata that might be used to unmask pseudonymous users. Once validated, these records will be dis-aggregated into the same skills/attributes model Sarcina uses to represent on-platform performance.
### **Competitive Advantage**
At launch, Sarcina has several characteristics which differentiate it from what a conventional "tech company" or "startup" is likely to offer. All of these follow from the Sarcina organization being a small team of mission-driven activists:

The first is extremely low transaction fees. Sarcina as a platform takes only a 1% transaction fee which, when using a low-cost cryptocurrency option such as BTC via Lightning Network, means a cost to the service provider of less than 1.2% of the transacted value. This is less than the credit card processing fees payed by any credit card based product and far less than the fees a company would have to charge to support a paid development team, much less a "growing startup with a great company culture".

The Sarcina Project is committed to privacy, pseudonymity, and permissionless access in the labor market to a degree which would be seen as too risky by most investors or public companies.

The architecture of Sarcina optimizes for the autonomy of the user and the user's control of their data to a degree which sacrifices much of the value and revenue potential platform operators have grown to expect. Any commercial competitor who attempts to replicate Sarcina's functionality should be assumed to be engaging in some level of surveillance, suppression, or data brokerage unless proven otherwise.

The Sarcina organization intends to remain small and to maintain the core infrastructure and client engine as a basic economic utility on close to a break-even basis. Non-central functions such as developer/integrator training, user support, and encoding services will be allocated to separate trusted organizations.

Most revenues in excess of operations costs and developer or marketing salaries will be reinvested into marketing campaigns, grants to whitelabel Sarcina startups, or reduced fees. Sarcina measures it's success as a project not by profits or equity valuation but by the fraction of the labor market where norms of worker sovereignty, permissionless access, and pseudonymity reign. 

## Architecture, Security, and Privacy
A brief walkthrough of the Sarcina architecture to highlight it's security and privacy features and explain the character of the data which will be available to the Sarcina Analytic Environment: 

**The Sarcina App Front End**

The UI layer with which the user interacts is not itself trusted and it is this layer where modding and re-skinning are encouraged. The lower "engine" layer contains a limited amount of UI code so that it can "burst through" for security critical interactions such as authorizing payments.

**The Sarcina Engine**

The Sarcina Engine is a set of local services which implement the network, transaction management, key management, and rules enforcement functions which allow connections via the Sarcina Protocol. It is written in Rust and compiled to WASM and is expected to be distributed directly from a source certified the the Sarcina organization, either by itself or packaged with the reference UI. It is important that the user trusts their local installation of the Sarcina Engine since it is at this layer that their funds and identity are secured and persisted and it is the engine which enforces the user's rights according to the terms of any line they connect to.

In the reference client, only the engine connects to the internet. The engine makes all necessary connections to Sarcina's support services and holds the various peer-to-peer streams which constitute a Sarcina call. The engine also manages and persists user keys and trusted data such as copies of issued lines. The engine holds a WalletConnect connection to whichever local cryptocurrency wallet the user designates during setup.

**Sarcina Core Support Services**

Certain centralized services are required in order for Sarcina users to connect and complete calls. 

**The Sarcina Analytic Environment**



**The Sarcina Registry**.



## Machine Learning Use Cases for the Sarcina Analytic Environment


## State of Development
