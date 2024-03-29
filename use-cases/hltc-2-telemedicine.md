# HLTC-2 - Telemedicine

## Product Use Case Summary

| ID      | HLTC-2       |
| ------- | ------------ |
| Name    | Telemedicine |
| Sector  | Health       |
| Version | 1.0          |
| Status  | Published    |

Telemedicine (also referred to as telehealth) lets patients visit with a health care provider without an in-person office visit. Instead, patient-provider interaction is conducted over the phone or online through a computer, tablet, or smartphone.

The goal for modern telemedicine is to provide an alternative to in-person visits which helps improve access to health care for distant or rural populations, provides a safe experience without the risk of exposure to communicable diseases, and/or helps patients receive routine, specialty, or emergency care without the need to visit a health center. For healthcare providers telemedicine can save time in under-resourced areas, can extend the geographical reach of individual practitioners, and can meet gaps in a practitioner’s schedule.

Telemedicine is not a substitute for in-person care, but can extend the reach of traditional health systems and can help meet ambitious national health targets.

Local connectivity levels must be considered when designing a telemedicine project since there may be remote communication disadvantages in rural regions to ensure efficient remote consultations. For instance, if the internet connection is poor, software should be able to switch to audio communication using VoIP (Voice over Internet Protocol) or cellular network. If the audiovisual communication is still poor, healthcare practitioners can consult via text messages.

## Stakeholders

* Patients that want to receive accessible health services and care from anywhere, including those in hard-to-reach areas not serviced by hospitals.
* Healthcare providers (doctors, nurses, etc.) that want to provide care to patients remotely.
* Ministry of health or central government body in charge of national health outcomes that needs to track aggregate indicators of health care access.
* Administrators that need to manage payments and/or labs of patients.

## Sustainable Development Goals (SDGs)

* [**SDG 3**](https://exchange.dial.global/sdgs/good\_health\_and\_wellbeing): Good Health and Well-Being

## Building Blocks

* [**Consent**](https://govstack.gitbook.io/bb-consent/)
* [**Digital Registries**](https://govstack.gitbook.io/bb-digital-registries)
* [**E-Signature**](https://govstack.gitbook.io/bb-esignature)
* [**GIS**](https://govstack.gitbook.io/bb-gis)
* [**Identity**](https://govstack.gitbook.io/bb-identity/)
* [**Information Mediator**](https://govstack.gitbook.io/bb-information-mediation/)
* [**Messaging**](https://govstack.gitbook.io/bb-messaging/)
* [**Payments**](https://govstack.gitbook.io/bb-payments/)
* [**Scheduler**](https://govstack.gitbook.io/bb-scheduler/)
* [**Workflow**](https://govstack.gitbook.io/bb-workflow/)

## Source Documents

* [Framework for the Implementation of a Telemedicine Service](https://iris.paho.org/bitstream/handle/10665.2/28414/9789275119037\_eng.pdf)
* [Telehealth Technology: Adoption, Architecture, and Applications of Telemedicine](https://www.scnsoft.com/healthcare/telemedicine)
* [The Rise of Telemedicine](https://www.healthitoutcomes.com/doc/the-rise-of-telemedicine-0001)

## Steps

### 1 - Scoping

In cases where telemedicine is being pursued as a centralized activity to meet national health objectives, the Ministry of Health can work with Mobile Network Operators (MNOs) to map regions and districts which have broadband connectivity. Communications Satellite Networks can also be engaged to provide the required broadband bandwidth for effective delivery of telemedicine services in areas with little or no terrestrial mobile networks. In some cases, agreements between governments and MNOs need to be established in order to enable an accessible system, such as health helplines.

**Workflows**

* **Data Collection and Reporting** to facilitate the mapping and scoping of connected/under connected areas

**Building Blocks**

[**GIS**](https://govstack.gitbook.io/bb-gis)

### Step 2 - Outreach Communications

Staff from the Ministry of Health, private telehealth companies, or other intermediary organizes outreach communications to physicians, nurses, and other healthcare providers to sign up as a telehealth practitioner. Similarly, staff from the Ministry of Health, CSOs, or other intermediary organizations launch an information campaign to inform about a telehealth program aimed at potential target population/ beneficiary group and implemented via telehealth company. The campaign is conveyed via mobile messaging and/or aired on national radio/television, while a more capillary village to village campaign is performed by district / local social welfare officers. Outreach communication is intensive during the kick-off phase of the new program, but also requires ongoing touch points and additional information sharing.

**Workflows**

* **Client Education** for educating potential target beneficiaries around the approach and objective(s), benefit(s), constraint(s), partner(s), etc. of the program
* **Client Communication** to facilitate the spreading of program awareness for target audience and encouraging enrolment via mobile / media channel(s)
* **Content Management** for the backend Social Welfare staff to populate relevant educational and promotional content that local officers can use during on-the-ground outreach campaigns
* **Identification and Registration** (along with GIS) in mapping and locating households and individuals for outreach target

#### Building Blocks

[**Messaging**](https://govstack.gitbook.io/bb-messaging/)

[**Scheduler**](https://govstack.gitbook.io/bb-scheduler/)

### Step 3 - Health Provider Registration

Registration for healthcare workers can occur differently based on whether the telemedicine system is rolled out in a centralized or decentralized manner. In country contexts where a centralized authority (such as the Ministry of Health) is rolling out a telemedicine program (such as a health helpline), healthcare workers can sign up on a central roster.

In decentralized contexts, healthcare workers an sign up through participating hospitals/health care provider networks or directly through a telehealth company.

In this step, all healthcare workers will also provide information on qualifications, certifications and licenses.

**Workflows**

* **Data Collecting and Reporting** to capture provider’s demographic data, information on specialties, and information on qualifications. In return patients can provide demographic, geographic, and health history data
* **Identification and Verification** for enrolled identified healthcare providers and patients and enabling permissions
* **Client Case Management** for creating patient user records

#### Building Blocks

[**Consent**](https://govstack.gitbook.io/bb-consent/)

[**Digital Registries**](https://govstack.gitbook.io/bb-digital-registries)

[**E-Signature**](https://govstack.gitbook.io/bb-esignature)

[**Identity**](https://govstack.gitbook.io/bb-identity/)

[**Information Mediator**](https://govstack.gitbook.io/bb-information-mediation/)

### Step 4 - Patient Registration

Registration for patients can vary depending on specific country/district-level contexts. Patients can sign up directly, through their hospital systems, or via representative health workers that can register participating individuals. In the latter case, the healthcare worker can assist individuals to provide demographic, geographic, and health history data into the system.

**Workflows**

* **Data Collecting and Reporting** to capture provider’s demographic data, information on specialties, and information on qualifications. In return patients can provide demographic, geographic, and health history data
* **Client Case Management** for creating patient user records
* **Identification and Verification** for enrolled identified healthcare providers and patients and enabling permissions

#### Building Blocks

[**Consent**](https://govstack.gitbook.io/bb-consent/)

[**E-Signature**](https://govstack.gitbook.io/bb-esignature)

[**Identity**](https://govstack.gitbook.io/bb-identity/)

[**Information Mediator**](https://govstack.gitbook.io/bb-information-mediation/)

### Step 5 - Data Verification and Validation

In this step, registration data needs to be verified and validated. Healthcare provider qualifications can be checked via the licensure organization in the country and patient data can be verified with local digital identification or census database.

**Workflows**

* **Client case Management** used for verifying and validating enrollment of patients and healthcare workers
* **Data Analysis and Business Intelligence / Data Collection and Reporting** for administrators and national workers to monitor and track use and uptake of the system.

#### Building Blocks

[**Consent**](https://govstack.gitbook.io/bb-consent/)

[**Identity**](https://govstack.gitbook.io/bb-identity/)

[**Information Mediator**](https://govstack.gitbook.io/bb-information-mediation/)

### Step 6 - System Access

Patients, healthcare providers, and administrators need access to telehmedicine system using an application protocol while adhering to stringent privacy protection measures. As the front end to most telemedicine applications, it is critical to maintain available, high-performance web front end systems. When monitoring and troubleshooting issues with telemedicine systems, IT teams need to have visibility across web connections and through firewalls and load balancers.

**Workflows**

* **Client Communication** to facilitate individual communication between the system and all users (healthcare workers, patients, and administrators)

#### Building Blocks

[**Information Mediator**](https://govstack.gitbook.io/bb-information-mediation/)

### Step 7 - Schedule Appointments

Appointments can be triggered by patients (such as for a first-time visit) or by health care providers (such as for a follow-up). In either case, health care providers set a schedule of availability for patients selection. Patients can book appointments with health care providers directly or through intermediaries, based on preferences and condition (such as general, emergency, specialty, or nursing care, etc.). The system can also generate auto-notifications for receiving confirmations and/or reminders, and for approving appointments.

**Workflows**

* **Client case Management** can be either automated or through an intermediary health care worker on the ground that is responsible for coordinating appointments on a centralized system
* **Work Planning and Coordination** so healthcare providers and administrative staff can coordinate the timing/schedules of multiple patients they may be serving

#### Building Blocks

[**Information Mediator**](https://govstack.gitbook.io/bb-information-mediation/)

[**Messaging**](https://govstack.gitbook.io/bb-messaging/)

[**Scheduler**](https://govstack.gitbook.io/bb-scheduler/)

[**Workflow**](https://govstack.gitbook.io/bb-workflow/)

### Step 8 - Consultation

Depending on connectivity and device parameters, there are two main ways that a health care practitioner and patient can conduct the consultation. 1) The consultation can be done through a live phone or video chat using a personal device. In some cases, the consultation can be done using a shared device provided by a health care officer or other intermediary. 2) The consultation can also be done by sending and receiving messages using secure messaging, email, and secure file exchange.

As part of the consultation, the healthcare provider can update the patient record, diagnose the patient, recommend a treatment plan, prescribe medications, request lab work, generate a referral with a specialist, and/or recommend a follow-up.

**Workflows**

* **Client Communication** for sharing relevant updates, diagnoses, treatment plans, and follow-up with client
* **Client Case Management** for identifying and recording patient interaction with healthcare workers and for determining follow-ups and storing patient history
* **Data Collection and Reporting** for capturing changes in beneficiary information
* **Work Planning and Coordination** for referrals to specialists or connections with other hospitals, clinics, or lab and pharmacy services

#### Building Blocks

[**Consent**](https://govstack.gitbook.io/bb-consent/)

[**Information Mediator**](https://govstack.gitbook.io/bb-information-mediation/)

[**Scheduler**](https://govstack.gitbook.io/bb-scheduler/)

### Step 9 - Payment Management

Payments can be collected either pre- or post-consultation. In the context where a digital financial service system is not employed, each beneficiary would be requested to pay via mobile money or to travel to the nearest designated pay-point and pay the fees by program-specific authentication. Money is transferred to the selected payment mechanism and is subsequently verified against the provider.

**Workflows**

* **Client Case Management** for identifying and authenticating individual that is making a payment
* **Financial Services** for processing consultation fees and other fees related to tests, labs, and prescriptions

#### Building Blocks

[**Identity**](https://govstack.gitbook.io/bb-identity/)

[**Information Mediator**](https://govstack.gitbook.io/bb-information-mediation/)

[**Payments**](https://govstack.gitbook.io/bb-payments/)

### Step 10 - Ongoing Case Management

Depending on the program and on the country’s broader health policies, this step involves ongoing interaction with beneficiaries via healthcare officers to help:

* Provide ongoing care and management – In some cases, this can also be done through remote sensors that can send information to healthcare providers on the patient’s health status
* Ensure information on patients and health care providers stays up to date
* Address complaints, grievances, and appeals

**Workflows**

* **Client Case Management** for identifying and recording patient interaction with health care providers/worker and capturing reported cases on grievances
* **Data Collection and Reporting** for capturing changes in patient or health care provider information
* **Work Planning and Coordination** to potentially suggest and connect with departments / agencies offering other social benefits and services to eligible patients

#### Building Blocks

[**Consent**](https://govstack.gitbook.io/bb-consent/)

[**Identity**](https://govstack.gitbook.io/bb-identity/)

[**Information Mediator**](https://govstack.gitbook.io/bb-information-mediation/)

[**Messaging**](https://govstack.gitbook.io/bb-messaging/)

[**Workflow**](https://govstack.gitbook.io/bb-workflow/)

### Step 11 - Ongoing Monitoring and Evaluation

Administrators of the telehealth company and/or Ministry of Health analysts conduct ongoing M\&E of the programs to understand uptake and benefit of telemedicine services. In addition, they can use analysis to make decisions and management choices, such as general health outcomes of enrolled areas/patients vs. non-enrolled areas/patients, where to conduct trainings, where to prioritize budget, etc.

**Workflows**

* **Client Case Management** for ongoing monitoring and tracking of patients and health care workers usage and experience
* **Data Analysis and Business Intelligence/ Decision Support / Data Collection and Reporting** - to analyize, update, and report program output/performance information

#### Building Blocks

[**Consent**](https://govstack.gitbook.io/bb-consent/)

[**GIS**](https://govstack.gitbook.io/bb-gis)

[**Identity**](https://govstack.gitbook.io/bb-identity/)

[**Scheduler**](https://govstack.gitbook.io/bb-scheduler/)

[**Workflow**](https://govstack.gitbook.io/bb-workflow/)

## Contributors

* Wesley Brown, GovStack Product Owner, Digital Impact Alliance
* Steve Conrad, Associate Director of Technology, Digital Impact Alliance
* Sarah Farooqi, The Exchange Product Owner, Digital Impact Alliance
* Sainabou Jallow, Business Analyst, Digital Impact Alliance
* Margus Mägi, GovStack Project Lead for Estonia
* Dr. P. S. Ramkumar, GovStack, International Telecommunication Union (ITU)
* Dr. Sanjay Sood, Project and Associate Director, eSanjeevani (National Telemedicine Service)&#x20;
* Jai Ganesh Udayasankaran, Senior Manager, Healthcare Information Technology and Telehealth Sri Sathya Sai Central Trust, INDIA AeHIN
