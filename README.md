# Sarcina and it's Analytic Environment
An introduction to the Sarcina Project, it's mission, and a discussion of Data Privacy, Data Analytics, and Machine Learning in Sarcina's Analytic Backend and the Sarcina Registry.


## Project Overview

* **Organization** Sarcina is a privately held corporation founded in 2017 by Marcus Zuech and undisclosed collaborators/partners.

* **Mission** Sarcina's mission is to enhance economic justice and freedom by creating tools which facillitate self-employment and agile distributed business organizations.

* **Origins** The germ of the idea for Sarcina came in 2008, when Marcus observed the burden and duplicative effort imposed on job seekers by conventional corporate recruitment. During that same period, Marcus' brother was struggling to re-establish himself after a series of minor legal troubles, highlighting the degree to which administrative and logistical burdens hamper the lives of low-skilled and economically precarious workers.

* **Initial Product Concept** Mr. Zuech's original vision for what later became the Sarcina Registry imagined a service of impeccable trustworthiness workers might use to cache verified records of their work, education, hobby and volunteer activities as well as the results of often duplicated employment screenings such as drug tests and criminal background checks. Mr. Zuech believed that with enough such data, it would be possible to derive a set of statistically valid and reliable attributes and skills to describe human capital, making the problem of matching workers to jobs simpler and saving both workers and employers substantial friction and cost.

* **Evolution** The design of the Sarcina Protocol and Sarcina Registry have evolved significantly over the years. The concept of the Registry predates the release of Bitcoin, the build-out of cloud computing, and the current generation of big data and machine learning technologies. While conception, research, design, and development towards Sarcina has been ongoing since 2008, Sarcina's current architecture which finally allows for a full realization of the projects vision has only become possible very recently. 

* **Alignment Security** Sarcina's mission has always entailed subverting and disrupting the current system of employment relations and labor discipline. While the proposed systems are in every respect legal and compliant under US law, Sarcina assumes it will face political and commercial pushback for attempting to invalidate deep assumptions of the current economic system. It is critically important to the core project team that the platform not become a tool for surveillance and control as has happened with competing labor platforms, social networks, and cryptocurrency exchanges. As such, Sarcina intends to remain forever a closely held corporation under a mission-driven leader who is at liberty to sacrifice personal and pecuniary interests in order to safeguard the project's vision.

* **Funding** In order to maintain the aforementioned independance, Sarcina does not seek venture capital which would rely on an eventual IPO or acquisition and so Sarcina is funded by the founding team directly until such a time as it becomes self-sustaining through operational revenues.

## Problems:

Sarcina seeks to address several systemic problems in the labor market and in business administration:

### **Problem 1: *Property Rights in Human Capital***
#### **Problem:**
> Modern ethics, public opinion, and the 13th Ammendment agree that it is not permissable for one person to own the labor potential of another.

> Yet there is no reliable mechanism which establishes an individual's effective control of their *own* human capital. Records pertaining to a person's reputation, skill, trustworthiness, and suitability for a given role may be the moral property of the individual, but are typically held by widely distributed custodians such as schools, former employers, and personal references.
#### **Solution:**
> Create a trustworthy, persistent repository of human capital related data where the worker can submit records for validation and forever retain control of those records' visibility while the content of those records may not be altered by either the worker or the platform operator once the record's veracity is validated to some known standard.

### **Problem 2: *Trusted Signals and Search Costs***
#### **Problem:**
> In the current system of labor recruiting, a combination of credentials and experience are used as a proxy for a worker's ability to perform a given job. One year of work or an entire degree program are crude, poorly defined units of measure which are non-fungible and difficult to compare across employers, industries, and educational institutions.

> Workers are incentivised to inflate qualifications while employers are incentivsed to define jobs defensively, assuming the minimum level of competence for the experience and credentials they demand. The overall result is that workers invest time and effort into often wasteful signalling activities while employers paint themselves into a corner where the pool of "qualified" applicants is highly restricted compared to the population of workers who might in fact perform a given job well
#### **Solution:**
> Given sufficiently granular and structured data about high-frequency labor transactions, it should be possible to impute a model of abstracted skills and labor quality measures which are comparable across different schools, employers, and industries. 

> With this model in place, a worker's experience and education can be used to infer a "charachter sheet" of granular skills and work habits. Employers will then be able to search the whole space of available workers and adjust the terms and weightings of that search in response to trade-offs between the availability and cost of different factors. Such a model will also give workers feedback on the present market value of their already-proven skills and guidance as to the expected value of additional training or targeted work experience while allowing workers, employers, and education providers to observe trends in the supply and demand of various skills.

#### **Problem 3: *Hiring Risk***
#### **Problem:**
> Because workers do not properly "own" their human capital in the sense of their value as a contributor being losslessly portable between employer-customers, the labor market has fallen into a pattern where workers attach to a single employer for long periods of time. This puts workers in a condition of low-grade peonage where they are far more dependant on their employer then the employer is on them.

> The two solutions to this condition which have previously been found are unionization and regulation. Both solutions serve to increase the administrative burden and business risk an employer faces when hiring a worker, creating a feedback loop where the labor market slows and employers engage in ever more elaborate practices to protect themselves from liability and maintain discipline over their workforce.

> A slow and defensive labor market presuming long-term, full-time, and exclusive employment means the wages a worker can realise for an hour or day of their time is tied to the amortized value of their contribution across entire months or years. Many workers fill critical roles in their organization which are only periodically performed. If an employer needs a certain skillset for only an hour a day or one day in a week, the pay they can offer a full-time worker to perform that task will be only a tiny fraction of value created by that worker during the minutes or hours they are actually needed.

> The economy as a whole and workers themselves suffer from the resulting underutilization of their talents as the highest best use of their labor is idled most of the time.
##### **Second-Order Problems:**
> Incremental employment of independant contractors can itself go a long way towards reducing employer risk and the efficiency of labor allocation. However, this "gig economy" has heretofor earned a poor reputation for two reasons:
> 1. "Gig Apps" are typically created as standalone platforms which target a single type of job. The gig app will usually need to structure and formalize this work to a point where individual gig workers are fungible. As a consequence, gig apps typically target unskilled or low-skill work and are most associated with desperate or precarious workers.
> 2. Because gig apps and freelancing platforms are isolated centralized systems where work history and performance data is seen as an asset of the platform operator rather than the worker, the worker's career advancement from engaging in gig work or freelancing is captive to the platform and confined to whatever rating system or gamification features the platform operator chooses to provide.
#### **Solution:**
> The Sarcina Protocol is a crytocurrency-based labor transaction protocol which cryptographically enforces workers and employers control over the use of their respective transaction histories and the portability of these records across both temporary and long-term employment.

> The Sarcina reference app can, with sufficient configuration, be used to intermediate any form of employment relationship. More importantly, Sarcina's client-side engine which implements the Sarcina Protocol and enforces the user(worker or employer)'s rights during the transaction exposes a local API on top of which any number of domain-specific apps can be built.

> This means barriers to entry for a gig app developer are drastically reduced, since building on top of Sarcina provides payment integration, session management, transactional data persistence, user identity management, fraud detection, peer-to-peer networking, and infrastructure hosting at no cost or effort to the developer. All that remains for a developer to do is to analyse some particular job or business function and create the interface and default business rules which will effectively "gigify" it.

> Workers meanwhile can use any Sarcina-based app with a single sign on and persistent identity, secure in the knowledge that they are accumulating experience and reputational credit which will enhance their employment prospects in the future.

#### **Problem 4: *Administrative Bloat***
#### **Problem:**
> In the first place, the long-running arms race between employers, employees, regulators, and unions to address the fundamental power imbalance of the employment relationship has imposed upon employers a requirement to maintain a parallel workforce of administrators and lawyers merely to protect themselves from the risk of having employees at all. Work roles are often excessively specialized due to the periodic need to formally adjudicate work performance.

> In the second place, narrow job roles and the systematic underutilization of full-time workers described above mean that in order to conduct a certain business at a certain scale, an employer has to take on and manage a larger body of full-time workers than they can beneficially employ at any given moment. The "Span of Control" problem means that the layers of management necessary to coordinate an organization grows as a consequence of headcount, whether or not those employees are actively contributing to the value-generating processes of the business.

> Companies in our economy are larger, more bloated, and less efficient than they ought to be in large part because the culture of full-time permanent employment imposes additional administrative and managerial overhead which is not implicit in those companies' domains or business models.
#### **Solution:**
> With a standardised, low-friction employment protocol like Sarcina, it will be possible to streamline companies according to their core business activities, with managers allocated funds to hire workers as needed on a minute-by-minute or task-by-task basis. While this will not increase a manager's attentional resources or span of control, it will be possible to maximise the useful output generated within that span. Furthermore, Sarcina automates many of the human resource management, payroll, and accounting functions for which companies currently maintain seperate support departments or pay for expensive SAAS solutions. Use of the Sarcina Registry to find and hire workers can reduce the latency from identifying a labor need to getting a qualified worker on-task from months to minutes.

> Furthermore, the Sarcina protocol, while optimised for labor transactions, can also intermediate B2B or B2C service transactions, software licensing, API access, subscription services, and commission/royalty schemes. This feature can aid in the decentralization of large enterprises into more independant cost and revenue centers without a loss in efficiency or coordination.

## Addressable Market:
There are at least three distinct ways to conceptualize the addressable market of Sarcina. From smallest to largest:

### *"Sarcina is a Gig or Freelancing Platform"*
#### Addressable Market: **~$455 Billion**
* If you concieve of Sarcina as a Gig/Freelancing platform, as a marketplace for such platforms, or as infrastructure for such platforms, then the addressable market is the current transacted value on all such platforms.
* According to [Statista](https://www.statista.com/statistics/1034564/gig-economy-projected-gross-volume/), the projected gross volume in the freelance business in 2023 will be $455.2B.
* This perspective is the most useful to understand the market Sarcina is seeking to enter in the near term following it's initial public release.

### *"Sarcina is a New Standard for Employment"*
#### Addressable Market: **~$10 Trillion**
* If you conceive of Sarcina as a general model for employment relations to compete with conventional employment, then the addressable market for Sarcina is the total wages of all workers.
* In the US in 2021, total wages were $9,709,991,000,000 according to [The St. Lois Fed](https://fred.stlouisfed.org/series/BA06RC1A027NBEA)
* This perspective is useful to understand the upper bounds of potential transacted value Sarcina might facillitate in the long term

### *"Sarcina is a Property Registrar for Human Capital"*
#### Addressable Market: **~$263 Trillion Assets Under Custody**
* Because of the systemic issues described in the "problems" section above, we aren't accustomed to thinking about "Human Capital" as an actual asset class with a formal valuation. But if you concieve of the Sarcina Registry as a sort of banking system or stock exchange where human capital is registered to it's owners and labor values are determined by market exchange, then you can calculate the present value of all existing human capital based on it's expected future cash flows.
> * A typical career lasts approximately 40 years from the end of formal education until the age of retirement, so the pool of all workers can be assumed to have an average of 20 years of remaining working life.
> * From [the same Fed data](https://fred.stlouisfed.org/series/BA06RC1A027NBEA) as before, we can see that our present cash flow to labor is ~$10T/year and that this has grown at an average annual rate of 9% from 1985 to 2021. From the [FRB website](https://www.frbdiscountwindow.org/en/PAges/Discount-Rates/Current-Discount-Rates.aspx) we can see a current discount rate of 5.25% (June, 2023).
> * From these figures, a linear projection suggests that Total Wages in 20 years from our benchmark year of 2021 will be $49.9T with a discounted present value of $17.3T.
* Based on the above assumptions, we can calculate the present value of existing human capital in the US to be $262,864,836,109,208.
* **This measure is not intended to give a realistic estimate of Sarcina's potential growth**, but the fact that the value of human capital thus derived vastly exceeds all other asset classes in the US economy combined goes to underline the points made above about the severe economic miscalculations which are possible under the current regime of ambiguity around property rights in human capital.

## Architecture, Security, and Privacy
Sarcina has two primary products **The Sarcina Protocol and it's Reference Client** and **The Sarcina Registry**.



## Products, Customers, and Business Models:




## Machine Learning Use Cases for the Sarcina Analytic Environment



