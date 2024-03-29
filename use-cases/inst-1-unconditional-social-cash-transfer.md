# INST-1 - Unconditional Social Cash Transfer

## Product Use Case Summary

| ID      | INST-1                             |
| ------- | ---------------------------------- |
| Name    | Unconditional Social Cash Transfer |
| Sector  | Institution                        |
| Version | 2.0                                |
| Status  | Published                          |

This use case profiles specifically the digital integration steps within the delivery journey of a generalized unconditional social cash transfer service. Unconditional cash transfers are cash payments provided to financially disadvantaged or vulnerable people or households without requiring anything in return (i.e. without conditionality). This is different from a conditional payment where the benefit needs to be applied on the basis of achieving a certain result (e.g. higher school attendance, or prenatal care visit), or to be expended specifically on a type of resource (e.g. housing, or agricultural equipment). Governments in low- and middle-income countries increasingly use these benefit schemes in attempt to reduce poverty or other vulnerabilities, such as those related to health.

## Stakeholders

* Ministry or national government body in charge of social welfare, community development and/or implementing social assistance and cash transfer programmes.
* Local social welfare officers in charge of identifying potential beneficiaries that meet eligibility criteria, and facilitating allocation of cash transfers to eligible beneficiaries.
* Vulnerable population/households - beneficiaries, that comply with pre-defined conditionalities and meet the eligibility criteria.

## Sustainable Development Goals (SDGs)

* [**SDG 1**](https://exchange.dial.global/sdgs/no\_poverty): No Poverty
* [**SDG 16**](https://exchange.dial.global/sdgs/peace\_justice\_and\_strong\_institu): Peace, Justice and Strong Institutions

## Building Blocks

* [**Consent**](https://govstack.gitbook.io/bb-consent)
* [**Identity**](https://govstack.gitbook.io/bb-identity)
* [**Information Mediator**](https://govstack.gitbook.io/bb-information-mediation)
* [**Messaging**](https://govstack.gitbook.io/bb-messaging/)
* [**Payments**](https://govstack.gitbook.io/bb-payments)
* [**Registration**](https://govstack.gitbook.io/bb-registration)
* [**Scheduling**](https://govstack.gitbook.io/bb-scheduler/)
* [**Workflow**](https://govstack.gitbook.io/bb-workflow)

## Source Documents

* [Digital Impact Exchange - Unconditional Social Cash Transfer](https://exchange.dial.global/use\_cases/unconditional\_social\_cash\_transf)

## Steps

### 1 - Outreach Communications

Staff from the Ministry of Social Welfare or another leading agency / organization organizes an information campaign to inform about a social assistance programme aimed at potential target population / beneficiary group(s) and implemented via predefined approaches and partners. The campaign is conveyed via mobile messaging and/or aired on national radio/television, while a more capillary village to village campaign is performed by district / local social welfare officers. Outreach communication is intensive during the kick-off phase of the new programme, but also requires ongoing touchpoints and additional information sharing, e.g. on grievance procedures, rights and responsibilities, behavioural change communication, etc.

**Workflows**

* **Client communication** to facilitate the spreading of programme awareness for target audience and encouraging enrolment via mobile / media channel(s)
* **Client education** for educating potential target beneficiaries around the approach and objective(s), benefit(s), constraint(s), partner(s), etc. of the programme
* **Content management** for the backend Social Welfare staff to populate relevant educational and promotional content that local officers can use during on-the-ground outreach campaigns
* **Identification and Registration** (with aid of geographic information services tool for potential use) in mapping and locating households and individuals for outreach target

**Building Blocks**

[**Messaging**](https://govstack.gitbook.io/bb-messaging/)

[**Scheduling**](https://govstack.gitbook.io/bb-scheduler/)

### 2 - Registration

Registration is the process of collecting information on potential beneficiaries for assessment of their needs and conditions. Depending on specific country context, registration works in very different ways – either through mass-census survey, or on-demand at local offices (either approach potentially building on interoperability existing data sources). While the practicalities of data collection differ across the two, with very different implications for data quality, currency and completeness, the underlying digital processes are broadly the same: Mass census survey registration is sometimes carried out in-house, other times by statistics agency or trained enumerators. A percentage\* of households across the country are interviewed on a periodic basis to collect socio-economic data (especially if to target population in poverty), geo-location data, and key documentation. On-demand registration is primarily carried out in-house via capacity at local levels of implementation (e.g. social welfare offices or municipalities) and involves people pro-actively applying when in need. In either case data (both at individual and household-levels) is entered into a registry that serves one social assistance programme alone or several: the Social Registry\*\* (SRIS). This is sometimes done directly at the moment of interview via computer assisted interview methods (CAPI), other times subsequently post-enumeration.

\* Percentage varies greatly across countries; 10-95% range depending on prior policy choices, etc.

\*\* The Social Registry collects, organizes, stores, processes, transforms, creates, and distributes information necessary to support intake and registration of potential beneficiaries (gateway function). It is part of a broader Social Assistance Information System, further discussed below and in subsequent steps.

**Workflows**

* **Client Case Management** for creating beneficiary user records
* **Data Collection and Reporting** for capturing interview responses or observation during registration process
* **Identification and Registration** for enrolled identified beneficiaries in the system and enabling possible permissions for interaction with the SRIS, and (with aid of geographic information services tool) to potentially locate and track households during the interview process

**Building Blocks**

[**Consent**](https://govstack.gitbook.io/bb-consent/)

[**Identity**](https://govstack.gitbook.io/bb-identity/)

[**Information Mediator**](https://govstack.gitbook.io/bb-information-mediation)

[**Registration**](https://govstack.gitbook.io/bb-registration/)

### 3 - Data Verification and Validation

Data within the SRIS Social Registry Information System (SRIS) is generally checked\* by central level Social Welfare Ministry managers, against other government databases (eg. ID, tax, land cadastre, etc.) in order to fill in any missing gaps, verify and validate collected information, including authentication of all records. \*Data checking approaches also vary: sometimes batch-sharing via CD, sometimes full interoperability

**Workflows**

* **Client Case Management** for storing and reviewing identification records and eligibility information of potential beneficiaries
* **Data Analysis and Business Intelligence** for cross-referencing and verifying records across multiple registry sources, and reconciling gaps / overlaps

**Building Block Workflows**

[**Consent**](https://govstack.gitbook.io/bb-consent/)

[**Identity**](https://govstack.gitbook.io/bb-identity/)

[**Information Mediator**](https://govstack.gitbook.io/bb-information-mediation)

### 4 - Eligibility Determination and Benefit Package(s) Design

NOTE: Depending on the country and programme, eligibility determination takes different forms e.g. categorical by age without income screening , poverty-targeted, etc. often via “Proxy Means Test” calculation to screen and rank households by ‘inferred’ income. "Clean" data from a Social Registry that have undergone the data verification and validation step is used to screen eligible beneficiaries and establish the recommended benefit and services ‘package’. The amount of transfer often varies depending on household composition, and beneficiaries may qualify for other add-on services based on analyzed socioeconomic / demographic information being used for other welfare or social programmes.

**Workflows**

* **Client Case Management** for determining and assigning benefit packages and benefit levels to specific user groups
* **Data Analysis and Business Intelligence / Decision Support** potentially for identifying different benefit levels / types in correlation to target groups’ socioeconomic / demographic information, based on existing eligibility criteria (e.g. via proxy means test, means test or category-based)

**Building Blocks**

[**Identity**](https://govstack.gitbook.io/bb-identity/)

[**Information Mediator**](https://govstack.gitbook.io/bb-information-mediation)

### 5 - Enrollment

Eligible beneficiaries are re-contacted and asked to enroll onto the programme. During enrolment, further data can be collected (depending on programme design) e.g. bank account details, biometrics, etc.. Further information is exchanged and, in certain program design or context, beneficiaries are issued with a programme card (depending on system setup by country). Programme specific data is often entered into a separate Beneficiary Registry associated with a Beneficiary Operations Management System (BOMS)\*, not the Social Registry used during Step 1. Registration. Non-eligible households are also contacted and informed, depending on program and context.

* Much of the literature on the topic refers to this as the programme’s Management Information System (MIS). In practice, this is a tailored software application that supports beneficiary management functions (e.g. enrolment, payments, case management, M\&E etc.).

**Workflows**

* **Client Case Management** for storing program specific data for tracking
* **Data Collection and Reporting** for capturing additional programmatic information on the beneficiaries during enrolment
* **Financial Services** for staging beneficiary account details for cash transfer processing
* **Identification and Registration** for identifying beneficiaries and confirming enrolment

**Building Blocks**

[**Identity**](https://govstack.gitbook.io/bb-identity/)

[**Information Mediator**](https://govstack.gitbook.io/bb-information-mediation)

[**Payments**](https://govstack.gitbook.io/bb-payments/)

[**Registration**](https://govstack.gitbook.io/bb-registration/)

### 6 - Payment

If a social cash transfer programme has enabled electronic payment processes (e.g. via banks, mobile money, etc.), payments are subsequently paid cyclically according to the programme schedule e.g. often bi-monthly. In the context where a digital financial service system is not employed, each beneficiary would be requested to travel to the nearest designated pay-point\* and collect money by programme-specific authentication. In either case, the money is transferred to the selected payment provider as per generated payroll and is subsequently verified against the individual’s identification of program enrollment. Other possible add-on intervention activities at this step: behaviour change communication; triggering of add-on benefits (or widening of beneficiary pool) in emergency context using GIS data, etc.

* These vary depending on design / implementation choices: banks, armoured vehicles, post offices, schools, etc.

**Workflows**

* **Client Case Management** for identifying and authenticating individual that is making a withdrawal, or to recall / verify deposit account information prior to payment transaction
* **Financial Services** for processing beneficiary payment directly to their account, or for generating payroll to deposit payment amounts for withdrawal by beneficiary from designated banking institution(s) / pay-point(s) thereafter

**Building Blocks**

[**Payments**](https://govstack.gitbook.io/bb-payments/)

### 7 - Ongoing Case Management

Depending on the programme and on the country’s broader social protection policies, this step involves ongoing interaction with beneficiaries via local social welfare officers to help: Ensure information on beneficiaries stays up to date Address complaints, grievances, and appeals Address multi-dimensional risks via connecting beneficiaries to other programmes and services e.g. child protection, etc. Carry out assessment of co-responsibilities / conditionalities, if any (this is achieved in some countries via data integration into e.g. school management system from Education ministry on attendance, or HIS from Health ministry on check-up, etc.) Note that this step also requires clarity, clear decisions, and protocols regarding whose data (or subset of such) is to be updated by which programme personnel or role and at what time.

**Workflows**

* **Client Case Management** for identifying and recording beneficiary interaction with local officers and capturing reported cases on grievances / appeals etc., and for determining risks / conditionality by reviewing individual beneficiary client case
* **Data Collection and Reporting** for capturing changes in beneficiary information
* **Work Planning and Coordination** to potentially suggest and connect with departments / agencies offering other social benefits and services to eligible beneficiaries

**Building Blocks**

[**Consent**](https://govstack.gitbook.io/bb-consent/)

[**Identity**](https://govstack.gitbook.io/bb-identity/)

[**Scheduler**](https://govstack.gitbook.io/bb-scheduler/)

[**Workflow**](https://govstack.gitbook.io/bb-workflow)

### 8 - Ongoing M\&E

Central level managers and local social welfare officers base decisions and management choices (e.g. where to conduct add-on training, re-registration camps, where to prioritise budget, etc.) on up-to-date data on the programme/s (e.g. who receives what, when, what areas are performing better, etc). Note that countries that do this effectively ensure programme BOMS data is connected / integrated via an Integrated Beneficiary Registry\* and develop effective reporting functions, including GIS enabled spatial reporting. \*This is a Registry that integrates data across existing Beneficiary registries and their associated BOMS to give an overview of who is receiving what across programmes.

**Workflows**

* **Client Case Management** for ongoing monitoring and tracking of client performance, and integration to other registries for holistic view and reporting
* **Identification and Registration** (with aid of geographic information services tool for potential use) in tracking / locating areas in relation to level of activities and adherence, or client household location
* **Data Analysis and Business Intelligence** / **Decision Support** / **Data Collection and Reporting** to analyze, update, and report programme output / performance information

**Building Blocks**

[**Consent**](https://govstack.gitbook.io/bb-consent/)

[**Identity**](https://govstack.gitbook.io/bb-identity/)

[**Scheduler**](https://govstack.gitbook.io/bb-scheduler/)

[**Workflow**](https://govstack.gitbook.io/bb-workflow)

### 9 - Updating

Ensuring data is up to date to trigger: Programme exit for those who are no longer eligible e.g. when a beneficiary dies, migrates, exceeds eligible age or no longer qualifies for other reasons. This is achieved via a combination of recertification campaigns, automated data updates, and data-sharing with other government databases e.g. civil registration for death. Programme entry for newly eligible beneficiaries, via new data collection or analysis etc. Other changes to entitlements (e.g. benefit type of transfer size) due to changes in household composition, incomes, etc. Note that this step also requires clarity, clear decisions, and protocols regarding whose data (or subset of such) is to be updated by which programme personnel or role and at what time.

**Workflows**

* **Client Case Management** for ongoing review of beneficiary case information
* **Data Analysis and Business Intelligence** / **Decision Support** to support identification of individuals for exit or entry based on analyzing change in programme-specific / socioeconomic data
* **Data Collection and Reporting** for routine update of information on the beneficiary client base, and integration of other databases and systems for automated data update on client cases overtime

**Building Blocks**

[**Consent**](https://govstack.gitbook.io/bb-consent/)

[**Identity**](https://govstack.gitbook.io/bb-identity/)

[**Scheduler**](https://govstack.gitbook.io/bb-scheduler/)

[**Workflow**](https://govstack.gitbook.io/bb-workflow)

## Contributors

* Wesley Brown, GovStack Product Owner, Digital Impact Alliance
* Steve Conrad, Associate Director of Technology, Digital Impact Alliance
* Jaume Dubois, Digital ID Lead, GovStack
* Sarah Farooqi, The Exchange Product Owner, Digital Impact Alliance
* Sainabou Jallow, Business Analyst, Digital Impact Alliance
* Dr. P. S. Ramkumar, GovStack, International Telecommunication Union (ITU)
* Max Carlson, GovStack
* Uwe Washer, GovStack
* Raul Kaidro, GovStack
* Saurav Bhatta, GovStack
