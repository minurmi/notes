# Healthcare interfaces



## Google Health API:
	Specialized data storing modalities
	- DICOM
	- HL7v2 - semi-structured data (difficult to parse) - protocl that predates the HTTP standard
	- PHIR - API and data standard.
	- Consent
	

## PHIR from HL7

https://cloud.google.com/healthcare-api/docs/concepts/fhir?utm_source=youtube&utm_medium=unpaidsoc&utm_campaign=CDR_ret_gcp_xkshcrvhhqg_CloudHealthcareAPI_071221&utm_content=description

https://github.com/awslabs/fhir-works-on-aws-authz-smart
http://www.hl7.org/fhir/smart-app-launch/1.0.0/
https://github.com/awslabs/fhir-works-on-aws-deployment
https://digitalhealth.folio3.com/blog/hl7-vs-fhir/
https://www.healthit.gov/sites/default/files/2019-08/ONCFHIRFSWhatIsFHIR.pdf

Fast Healthcare Interoperability Resources (FHIR) is a healthcare data standard with an application programming interface (API) for representing and exchanging electronic health records (EHR). FHIR is an information network that lets you link data across systems and a communication network that lets you exchange data between systems.

FHIR eliminates the need to individually modify the data template of every health IT system by exchanging data as resources. FHIR exposes resources such as patients, admissions, and medications as services, allowing consumer mobile apps to use GET and POST requests to retrieve and manipulate only the relevant data.

FHIR includes the following:
- An HTTP-based RESTful protocol
- Data representation that uses JSON, XML, and RDF

Both API and data standard.
- Using Moderm web-based technologies
	- OAuth
	- JSON
	- HTML
- Maps data as a graph -> human friendly searches


Authorization:
- SMART
- Cognito

AWS solution includes the following new features:
- Reading and writing Amazon OpenSearch Service documents from aliases instead of indexes.
- Cognito and role based access control 
- Using pooled infrastructure model for multi-tenancy.


## ActiveAction

ActiveAction -> acquired by Beurer
Telemedicine -> wear device for 1 week -> bring back and upload to cloud
3000 pharmacies

They want own way to start the session with their desktop application. They have desktop app that uses serial port and a web application to store the data.
Some way to set the patient identifier and settings to cloud and deliver to WD.
Client application to start the session and download the data and upload to cloud.

24h: 75-80 eur
72h: 90-100 eur