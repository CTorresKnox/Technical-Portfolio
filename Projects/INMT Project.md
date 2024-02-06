# Information-Management-Project
PROPOSAL BY WINNERS CONSULTATION LLP

Prepared for
Hawkins University Fitness and Athletic Center
Wamego, Kansas

Prepared by:
- Christopher Torres
- Robert R***
- Hudson C*****
- Sam K*********

Mar 8, 2023


# Project Description 
A collaborative project aimed to design, construct, populate, and manipulate a database for a fictional University's new athletic center and programs. Project completed for Information Management 342: Introduction to Database Systems. 

# Project Narrative 
Hawkins University is a small public university located in the midwestern United States. As a public
university it provides many recreational activities in addition to all its academic programming. One of
the rapidly growing areas is the Fitness and Athletics Center, affectionately called “Hawkins U-Fit”. It
opened early in the University’s life with a pool and intramural programming. Soon after, it gained
club sports programming. Hawkins University now has many facilities and programs underneath the
Hawkins U-Fit umbrella. The high interest by the students in being physically fit and staying active has
created a demand for a large number of programs and fitness activities over the years.

# Table of Contents 
PHASE I     
- Executive Overview
- Conceptual Data Model (ERD)			       					        
- Logical Model										      
- Data Dictionary										    
- Sample Reports

PHASE II   
- Back-end Code					       					    
- Query and Report Code									  
- Report Samples										  
- User Guide     										  
- Appendix: Updates and Restatement of Phase I						  


# PHASE I

# Executive Overview
We at Winners Consultation LLP were hired for the purpose of designing a database for the Hawking University Fitness and Athletic Center (HUFAC) in hopes of automating many processes for the HUFAC. We hope for the database to be flexible and capable of quick changes in the event of departmental shifts or rising needs of the organization should maintenance need to be made. We strive for the database to simplify the hiring process within the organization as well as better coordinate communication between different programs and their leaders. Lastly we would like the database to be easily accessible and simple to use in hopes of maximizing benefits for your department.

Our initial reading of the information given left us debating on the most efficient way to design the conceptual model of the database; however, after subsequent reading and revising, we believe we have found a sufficient model for now. Revisions may – and likely will – be necessary as time goes by and will remain flexible in our work to accommodate any needs of HUFAC. 

By successfully implementing this database into your organization, we hope you will be able to accomplish easy tracking information of the many applications you receive every semester, including status of applications and relevant certifications. We would also like to help you track relevant review information regarding employees as well as information for alumni and any feedback and references they may provide. Moreover, we hope to assist you in tracking information related to the members of your Fitness Program such as personal trainer sessions. Lastly, we would like to assist you in tracking program information such as employees charged with leading their activities, participants in these programs, and their teams. 

In Phase I of this proposal, we have provided an implementable conceptual model, logical model, a data dictionary, as well as sample reports for the coming Phase II. Phase II will involve sample reports and a detailed instruction manual.

# Conceptual Data Model (ERD) 
The implementable conceptual model will provide the users of the HUFAC database with the simplified structure of the database. This model can be used to follow and quickly see what attributes are within which table of the database; however, it should be cross referenced with the logical model to receive the full picture of the database. An explanation as well as a list of any assumptions made during the process of developing the implementable conceptual model of the database will be provided.

![ERD.pdf](https://github.com/CTorresKnox/Information-Management-Project/files/12849997/ERD.pdf)

![ERD](https://github.com/CTorresKnox/Information-Management-Project/assets/144376690/236eee4a-f1b7-4976-88eb-ff7924d30538)

# Logical Model
The implementable conceptual model will provide the users of the HUFAC database with the simplified structure of the database. This model can be used to follow and quickly see what attributes are within which table of the database; however, it should be cross referenced with the logical model to receive the full picture of the database. An explanation as well as a list of any assumptions made during the process of developing the implementable conceptual model of the database will be provided.

[Logical Data Model](https://github.com/CTorresKnox/Information-Management-Project/blob/3c6807dc8a475be52154440d1d67e281a55f852d/Logical%20Data%20Model.pdf)

![Logical Model](https://github.com/CTorresKnox/Information-Management-Project/assets/144376690/bbd122dd-0fb1-4b91-8e44-776ea4939e05)


# Data Dictionary
The data dictionary is a simple, easy-to-read table that provides definitions and descriptions, data types, as well as formats for the attributes/fields in question. It is easily organized by table with listed fields belonging to each one. The dictionary is easily referenced to gain a full understanding of the relationships between tables and the information provided therein.

[Data Dictionary.xlsx](https://github.com/CTorresKnox/Information-Management-Project/files/14181386/Data.Dictionary.xlsx)

![DD1](https://github.com/CTorresKnox/Information-Management-Project/assets/144376690/e05a3c5a-cdbf-41ec-8b1d-c33bc30b368c)
![DD2](https://github.com/CTorresKnox/Information-Management-Project/assets/144376690/c82f2622-4015-457f-bc18-7b8a8fe1c6a3)
![DD3](https://github.com/CTorresKnox/Information-Management-Project/assets/144376690/9bedf986-a144-4166-b086-b989f8d40eb8)

# Sample Report Designs 
The purpose of this report is to provide an overview of the average number of hours that employees worked in each of the different programs and their respective job roles. This information is valuable as it can be used to track employee productivity and identify areas where workload balancing may be required.

This report is designed to be useful for managers and supervisors who oversee employees across different programs and different job roles.

The user of this report is able to filter by program or by job role to view the specific information regarding employee hours that is relevant to their needs.

The report is sorted first by program and then by job role within each program. Within job roles, employees are sorted in ascending order. The average hours of each job role are displayed in a calculated field derived from the average employee hours in that role. The average hours of each program are displayed in a calculated field as well which averages all of the employee hours in a given program. 

![SampleReport1](https://github.com/CTorresKnox/Information-Management-Project/assets/144376690/3a5d9a4a-be48-459f-a3d7-18aae1952b48)


This report provides information about employees pay, which includes EmployeeID, last name, first name, RoleID, standard rate, starting rate, current rate, the date of the employee’s last raise, and the number of raises that the employee has had while in that job role. This information can be used to guarantee fair compensation and to identify potential disparities among the employees.

This report is intended to be used by HR professionals and supervisors who are responsible for managing employee compensation and ensuring that it is fair across the board.

The user could filter this data by RoleID or by EmployeeID to view information about pay that is relevant to their specific needs.

This report is sorted by EmployeeID in ascending order. Alternatively. It could be sorted by grouping by RoleID. 

![SampleReport2](https://github.com/CTorresKnox/Information-Management-Project/assets/144376690/e6a73e27-735c-4085-a905-6fe0d3c0aa63)


# PHASE II 

# Back-End Code

[Back End Code.pdf](https://github.com/CTorresKnox/Information-Management-Project/files/14181502/Back.End.Code.pdf)

```
DROP TABLE PersonalTrainerTimeSlots
DROP TABLE FitnessClubMembership
DROP TABLE PersonalTrainer
DROP TABLE WorkDetails
DROP TABLE Roles
DROP TABLE Participants
DROP TABLE Involvement
DROP TABLE Raise
DROP TABLE EmployeeActivity
DROP TABLE ProgramActivities
DROP TABLE Availability
DROP TABLE Program
DROP TABLE Contact
DROP TABLE JobHistory
DROP TABLE CertificateType
DROP TABLE Certification
DROP TABLE Alumni
DROP TABLE Employee
DROP TABLE Applicant

CREATE TABLE Applicant (
	ApplicantID						VARCHAR (50) NOT NULL, 
	DateOfApplication					DATE, 
	Major							VARCHAR(20), 
	SemesterApplied					VARCHAR(20), 
	FirstJobChoice					VARCHAR(50), 
	SecondJobChoice					VARCHAR(50), 
	GraduationDate					DATE, 
	DesiredHours						INT, 
	ClassSchedule						VARCHAR(80) NOT NULL, 
	OptionalInterestEssay					VARCHAR(80), 
	OptionalEvaluationEssay				VARCHAR(80), 
	InterviewStatus					VARCHAR(20), 
	InterviewDecisionDate				DATE, 
	InterviewComments					VARCHAR(30), 
	GPA							DEC(3,2), 
	ApplicantType						VARCHAR(10) NOT NULL
	CONSTRAINT ApplicantPK PRIMARY KEY (ApplicantID)
);

CREATE TABLE Employee (
	EmployeeID						VARCHAR(50) NOT NULL,
	Position						VARCHAR(50),
	StartingPay						DEC(4,2),
	ShirtSize						VARCHAR(5),
	Transcript						VARCHAR(50),
	ApplicantID						VARCHAR(50) NOT NULL,
	CONSTRAINT EmployeePK PRIMARY KEY (EmployeeID),
	CONSTRAINT AlEmployeeFK FOREIGN KEY (ApplicantID)
		REFERENCES Applicant (ApplicantID)
		ON UPDATE CASCADE ON DELETE NO ACTION,
);

CREATE TABLE Alumni (
	AlumniID						VARCHAR(50) NOT NULL,
	ReasonForLeaving					VARCHAR(50),
	ExitInterviewComments				VARCHAR(50),
	GradDate						DATE,
	ApplicantID						VARCHAR(50) NOT NULL,
	CONSTRAINT AlumniPK PRIMARY KEY (AlumniID),
	CONSTRAINT AlApplicantFK FOREIGN KEY (ApplicantID)
		REFERENCES Applicant (ApplicantID)
		ON UPDATE CASCADE ON DELETE NO ACTION,
);

CREATE TABLE Certification (
	CertificationID					VARCHAR(50) NOT NULL,
	Certification						VARCHAR(30),
	ExpirationDate					DATE NOT NULL,
	CONSTRAINT CertificationPK PRIMARY KEY (CertificationID)
);

CREATE TABLE CertificateType (
	CertTypeID						VARCHAR(50) NOT NULL,
	ApplicantID						VARCHAR(50) NOT NULL,
	CertificationID					VARCHAR(50) NOT NULL,
	CertificationType					VARCHAR(30)
	CONSTRAINT CertificateTypePK PRIMARY KEY (CertTypeID)
	CONSTRAINT CertTypeAppFK FOREIGN KEY (ApplicantID)
		REFERENCES Applicant (ApplicantID)
		ON UPDATE CASCADE ON DELETE NO ACTION,
	CONSTRAINT CertTypeCertFK FOREIGN KEY (CertificationID)
		REFERENCES Certification (CertificationID)
		ON UPDATE CASCADE ON DELETE NO ACTION,
);

CREATE TABLE JobHistory (
	JobHistoryID						VARCHAR(50) NOT NULL, 
	Position						VARCHAR(50), 
	Department						VARCHAR(30), 
	SupervisorName					VARCHAR(30), 
	PhoneNumber						VARCHAR(30), 
	StartDate						DATE, 
	EndDate						DATE, 
	PlaceOfEmployent					VARCHAR(40), 
	ApplicantID						VARCHAR(50) NOT NULL,
	CONSTRAINT JobHistoryPK PRIMARY KEY (JobHistoryID),
	CONSTRAINT JobAppFK FOREIGN KEY (ApplicantID)
		REFERENCES Applicant (ApplicantID)
		ON UPDATE CASCADE ON DELETE NO ACTION,
);

CREATE TABLE Contact (
	ContactID						VARCHAR(50) NOT NULL, 
	ContactType						VARCHAR(20), 
	FirstName						VARCHAR(15), 
	LastName						VARCHAR(20), 
	MidInitial						VARCHAR(2), 
	StreetAddress						VARCHAR(35), 
	City							VARCHAR(30), 
	State							VARCHAR(15), 
	Zip							INT, 
	HomePhone						VARCHAR(30), 
	CellPhone						VARCHAR(30), 
	Email							VARCHAR(50), 
	ApplicantID						VARCHAR(50) NOT NULL,
	CONSTRAINT ContactPK PRIMARY KEY (ContactID),
	CONSTRAINT ContAppFK FOREIGN KEY (ApplicantID)
		REFERENCES Applicant (ApplicantID)
		ON UPDATE CASCADE ON DELETE NO ACTION,
);

CREATE TABLE Availability (
	AvailabilityID						VARCHAR(50) NOT NULL,
	MorningStart						TIME,
	MorningEnd						TIME,
	NightStart						TIME,
	NightEnd						TIME,
	SummerStart						TIME,
	SummerEnd						TIME,
	ApplicantID						VARCHAR(50) NOT NULL,
	CONSTRAINT AvailabilityPK PRIMARY KEY (AvailabilityID),
	CONSTRAINT AvailAppFK FOREIGN KEY (ApplicantID)
		REFERENCES Applicant (ApplicantID)
		ON UPDATE CASCADE ON DELETE NO ACTION,
);

CREATE TABLE Program (
	ProgramID						INT NOT NULL,
	Name							VARCHAR(35),
	Description						VARCHAR(100),
	EmployeeID						VARCHAR(50) NOT NULL,
	CONSTRAINT ProgramPK PRIMARY KEY (ProgramID),
	CONSTRAINT ProgEmpFK FOREIGN KEY (EmployeeID)
		REFERENCES Employee (EmployeeID)
		ON UPDATE CASCADE ON DELETE NO ACTION,
);

CREATE TABLE ProgramActivities (
	ActivityID						VARCHAR(50) NOT NULL,
	Name							VARCHAR(50),
	StartDate						DATETIME,
	EndDate						DATETIME,
	AdditionalCosts					DEC(4,2),
	CEmployeeID						VARCHAR(50) NOT NULL,
	ProgramID						INT NOT NULL,
	CONSTRAINT ProgramActivitiesPK PRIMARY KEY (ActivityID),
	CONSTRAINT ActEmpFK FOREIGN KEY (CEmployeeID)
		REFERENCES Employee (EmployeeID)
		ON UPDATE CASCADE ON DELETE NO ACTION,
	CONSTRAINT ProgActProgFK FOREIGN KEY (ProgramID)
		REFERENCES Program (ProgramID),
);

CREATE TABLE EmployeeActivity (
	EmployeeActivityID					VARCHAR(50) NOT NULL,
	EmployeeID						VARCHAR(50) NOT NULL,
	ActivityID						VARCHAR(50) NOT NULL,
	CONSTRAINT EmployeeActivityPK PRIMARY KEY (EmployeeActivityID),
	CONSTRAINT EmpActEmpFK FOREIGN KEY (EmployeeID)
		REFERENCES Employee (EmployeeID),
	CONSTRAINT EmpActProgFK FOREIGN KEY (ActivityID)
		REFERENCES ProgramActivities (ActivityID)
		ON UPDATE CASCADE ON DELETE NO ACTION
);

CREATE TABLE Raise (
	RaiseID						VARCHAR(50) NOT NULL,
	PayRaiseAmount					DEC(4,2),
	DateofRaise						DATE,
	NotesOnEval						VARCHAR(200),
	EmployeeID						VARCHAR(50) NOT NULL,
	CONSTRAINT RaisePK PRIMARY KEY (RaiseID),
	CONSTRAINT RaiseEmpFK FOREIGN KEY (EmployeeID)
		REFERENCES Employee (EmployeeID)
		ON UPDATE CASCADE ON DELETE NO ACTION,
);

CREATE TABLE Involvement (
	Description						VARCHAR(80) NOT NULL,
	EmployeeID						VARCHAR(50) NOT NULL,
	CONSTRAINT InvolvementPK PRIMARY KEY (EmployeeID),
	CONSTRAINT InvoleEmpFK FOREIGN KEY (EmployeeID)
		REFERENCES Employee (EmployeeID)
		ON UPDATE CASCADE ON DELETE NO ACTION,
);

CREATE TABLE Participants (
	ParticipantID						VARCHAR(50) NOT NULL,
	FirstName						VARCHAR(12),
	LastName						VARCHAR(10),
	StreetAddress						VARCHAR(35),
	City							VARCHAR(30),
	State							VARCHAR(30),
	Zip							INT,
	Phone							VARCHAR(30),
	Gender							VARCHAR(8),
	BirthDate						DATE,
	EnrollmentDateTime					DATE,
	ActivityID						VARCHAR(50) NOT NULL,
	CONSTRAINT ParticipantPK PRIMARY KEY (ParticipantID),
	CONSTRAINT PartActFK FOREIGN KEY (ActivityID)
		REFERENCES ProgramActivities (ActivityID)
		ON UPDATE CASCADE ON DELETE NO ACTION,
);

CREATE TABLE Roles (
	RoleID							VARCHAR(50) NOT NULL,
	RoleType						VARCHAR(50),
	Rate							DEC(4,2),
	Description						VARCHAR(100),
	HourlyExpectation					INT,
	CONSTRAINT RolesPK PRIMARY KEY (RoleID),
);

CREATE TABLE WorkDetails (
	WorkDetailsID					VARCHAR(50) NOT NULL,
	EmployeeID						VARCHAR(50) NOT NULL,
	RoleID							VARCHAR(50) NOT NULL,
	ProgramID						INT NOT NULL,
	ShiftTime						DATETIME,
	ShiftEnd							DateTIME,
	CONSTRAINT WorkDetailsPK PRIMARY KEY (WorkDetailsID),
	CONSTRAINT DetailsEmpFK FOREIGN KEY (EmployeeID)
		REFERENCES Employee (EmployeeID)
		ON UPDATE CASCADE ON DELETE NO ACTION,
	CONSTRAINT DetailsRoleFK FOREIGN KEY (RoleID)
		REFERENCES Roles (RoleID)
		ON UPDATE CASCADE ON DELETE NO ACTION,
	CONSTRAINT DetailsProgramFK FOREIGN KEY (ProgramID)
		REFERENCES Program (ProgramID),
);

CREATE TABLE PersonalTrainer (
	PTEmployeeID					VARCHAR(50) NOT NULL,
	Hours							INT,
	Rate							DEC(4,2),
	ProgramID						INT NOT NULL,
	CONSTRAINT PersonalTrainerPK PRIMARY KEY (PTEmployeeID),
	CONSTRAINT PTProgFK FOREIGN KEY (ProgramID)
		REFERENCES Program (ProgramID)
		ON UPDATE CASCADE ON DELETE NO ACTION,
);

CREATE TABLE FitnessClubMembership (
	MemberID						VARCHAR(50) NOT NULL,
	FirstName						VARCHAR(12),
	LastName						VARCHAR(10),
	StreetAddress						VARCHAR(35),
	City							VARCHAR(15),
	State							VARCHAR(15),
	Zip							INT,
	Phone							VARCHAR(30),
	Gender							VARCHAR(8),
	BirthDate						DATE,
	JoinDate						DATE,
	PTEmployeeID					VARCHAR(50) NOT NULL,
	CONSTRAINT FCMPK PRIMARY KEY (MemberID),
	CONSTRAINT PTFCMFK FOREIGN KEY (PTEmployeeID)
		REFERENCES PersonalTrainer (PTEmployeeID)
		ON UPDATE CASCADE ON DELETE NO ACTION,
);

CREATE TABLE PersonalTrainerTimeSlots (
	PTEmployeeID					VARCHAR(50) NOT NULL,
	MemberID						VARCHAR(50) NOT NULL,
	CONSTRAINT PTTSPK PRIMARY KEY (PTEmployeeID, MemberID),
	CONSTRAINT PTTSEmFK FOREIGN KEY (PTEmployeeID)
		REFERENCES PersonalTrainer (PTEmployeeID)
		ON UPDATE NO ACTION ON DELETE NO ACTION,
	CONSTRAINT PTTSMeFK FOREIGN KEY (MemberID)
		REFERENCES FitnessClubMembership (MemberID)
		ON UPDATE NO ACTION ON DELETE NO ACTION,
);

INSERT INTO Applicant VALUES ('1', '2022-02-20', 'Business', 'Spring', 'WaterSafety', 'OutdoorRec', '2023-05-12', '12', '[URL]', '[URL]', '[URL]', 'Approved', '2022-03-01', 'Friendly, Nice', '4', 'Alum'
)INSERT INTO Applicant VALUES ('2', '2022-02-24', 'Psychology', 'Spring', 'SportsClubManager', 'PersonalTrainer', '2024-05-15', '15', '[URL]', '', '', 'Approved', '2022-03-01', 'Hardworking', '3.8', 'Alum'
)INSERT INTO Applicant VALUES ('3', '2022-02-24', 'Biology', 'Spring', 'GroundsMaintenanceAssistant', 'PersonalTrainer', '2023-05-12', '15', '[URL]', '[URL]', '', 'Approved', '2022-03-01', 'Friendly, Nice', '3.81', 'Alum'
)INSERT INTO Applicant VALUES ('4', '2022-02-24', 'Mathematics', 'Spring', 'ComputerTech', 'PersonalTrainer', '2023-05-12', '20', '[URL]', '', '[URL]', 'Approved', '2022-03-01', 'Outgoing', '3.7', 'Alum'
)INSERT INTO Applicant VALUES ('5', '2022-02-25', 'Business', 'Spring', 'OutdoorRec', 'PersonalTrainer', '2024-05-15', '20', '[URL]', '', '', 'Approved', '2022-03-01', 'Outgoing', '3', 'Alum'
)INSERT INTO Applicant VALUES ('6', '2022-02-25', 'Biology', 'Spring', 'Receptionist', 'WaterSafety', '2024-05-15', '25', '[URL]', '[URL]', '', 'Approved', '2022-03-01', 'Friendly', '3.05', 'Emp'
)INSERT INTO Applicant VALUES ('7', '2022-05-21', 'Engineering', 'Summer', 'IntramuralAssistant', 'IntramuralOfficial', '2025-05-20', '25', '[URL]', '', '', 'Approved', '2022-06-12', 'Analytical', '2.9', 'Alum'
)INSERT INTO Applicant VALUES ('8', '2022-06-02', 'Engineering', 'Summer', 'IntramuralOfficial', 'Receptionist', '2025-05-20', '25', '[URL]', '', '', 'Approved', '2022-06-12', 'Smart', '4', 'Alum'
)INSERT INTO Applicant VALUES ('9', '2022-10-26', 'Business', 'Fall', 'BuildingManager', 'UFitAssistant', '2025-05-20', '20', '[URL]', '[URL]', '[URL]', 'Approved', '2022-11-01', 'Analytical', '4', 'Alum'
)INSERT INTO Applicant VALUES ('10', '2022-10-27', 'Business', 'Fall', 'UFitAssistant', 'OutdoorRec', '2025-05-20', '12', '[URL]', '', '', 'Approved', '2022-11-01', 'Good candidate', '4', 'Emp'
)INSERT INTO Applicant VALUES ('11', '2022-10-27', 'Psychology', 'Fall', 'MarketingGraphicDesign', 'ComputerTech', '2025-05-20', '10', '[URL]', '', '', 'Approved', '2022-11-01', 'Smart', '4', 'Emp'
)INSERT INTO Applicant VALUES ('12', '2022-10-27', 'Biology', 'Fall', 'FitnessAreaFloorTrainer', 'PersonalTrainer', '2025-05-20', '10', '[URL]', '', '[URL]', 'Denied', '2022-11-01', 'Rude', '1.5', 'Alum'
)INSERT INTO Applicant VALUES ('13', '2022-10-28', 'Education', 'Fall', 'FitnessAreaFloorSupervisor', 'PersonalTrainer', '2025-05-20', '10', '[URL]', '[URL]', '', 'Approved', '2022-11-01', 'Questionable', '3.25', 'Emp'
)INSERT INTO Applicant VALUES ('14', '2022-10-28', 'Business', 'Fall', 'GroupFitness', 'PersonalTrainer', '2025-05-20', '12', '[URL]', '', '', 'Approved', '2022-11-01', 'Friendly', '3.22', 'Alum'
)INSERT INTO Applicant VALUES ('15', '2022-10-29', 'Business', 'Fall', 'PersonalTrainer', 'GroupFitness', '2025-05-20', '25', '[URL]', '[URL]', '', 'Approved', '2022-11-01', 'Smart', '1.9', 'Emp'
)INSERT INTO Applicant VALUES ('16', '2023-01-01', 'Business', 'Spring', 'FitnessAreaFloorSupervisor', 'PersonalTrainer', '2025-05-20', '5', '[URL]', '', '[URL]', 'Approved', '2023-02-01', 'Quick learner', '3.7', 'Emp'
)INSERT INTO Applicant VALUES ('17', '2023-01-02', 'Psychology', 'Spring', 'FitnessAreaFloorSupervisor', 'GroupFitness', '2025-05-20', '25', '[URL]', '[URL]', '', 'Approved', '2023-02-01', 'Smart', '3.2', 'Emp'
)INSERT INTO Applicant VALUES ('18', '2023-01-02', 'Biology', 'Spring', 'IntramuralAssistant', 'Receptionist', '2026-05-18', '12', '[URL]', '[URL]', '', 'Denied', '2023-02-01', 'Lazy', '2.9', 'Emp'
)INSERT INTO Applicant VALUES ('19', '2023-01-02', 'Mathematics', 'Spring', 'ComputerTech', 'MarketingGraphicDesign', '2026-05-18', '15', '[URL]', '', '', 'Approved', '2023-02-01', 'Quick learner', '3', 'Emp'
)INSERT INTO Applicant VALUES ('20', '2023-01-04', 'Business', 'Spring', 'PersonalTrainer', 'WaterSafety', '2025-05-20', '15', '[URL]', '', '', 'Approved', '2023-02-01', 'Smart', '3.2', 'Emp'
)INSERT INTO Applicant VALUES ('21', '2023-01-05', 'Biology', 'Spring', 'PersonalTrainer', 'OutdoorRec', '2024-05-15', '15', '[URL]', '', '', 'Approved', '2023-02-01', 'Friendly, Nice', '3.4', 'Emp'
)INSERT INTO Applicant VALUES ('22', '2023-01-07', 'Engineering', 'Spring', 'PersonalTrainer', 'ComputerTech', '2024-05-15', '15', '[URL]', '', '[URL]', 'Approved', '2023-02-01', 'Outgoing', '3.67', 'Emp'
)INSERT INTO Applicant VALUES ('23', '2023-01-07', 'Engineering', 'Spring', 'PersonalTrainer', 'UFitAssistant', '2025-05-20', '18', '[URL]', '', '[URL]', 'Approved', '2023-02-01', 'Outgoing', '3', 'Emp'
)INSERT INTO Applicant VALUES ('24', '2023-01-20', 'Business', 'Spring', 'PersonalTrainer', 'ComputerTech', '2025-05-20', '20', '[URL]', '', '[URL]', 'Approved', '2023-02-01', 'Smart', '4', 'Emp'
)INSERT INTO Applicant VALUES ('25', '2023-01-21', 'Business', 'Spring', 'PersonalTrainer', 'BuildingManager', '2026-05-18', '25', '[URL]', '', '[URL]', 'Approved', '2023-02-01', 'Smart', '4', 'Emp'
)INSERT INTO Applicant VALUES ('26', '2023-01-21', 'Psychology', 'Spring', 'FitnessAreaFloorSupervisor', 'GroundsMaintenanceAssistant', '2026-05-18', '20', '[URL]', '', '[URL]', 'Approved', '2023-02-01', 'Friendly', '4', 'Emp'
)INSERT INTO Applicant VALUES ('27', '2023-01-25', 'Biology', 'Spring', 'PersonalTrainer', 'GroupFitness', '2026-05-18', '20', '[URL]', '[URL]', '', 'Pending', '2023-02-01', 'Good candidate', '3.1', 'Emp'
)INSERT INTO Applicant VALUES ('28', '2023-01-25', 'Education', 'Spring', 'PersonalTrainer', 'BuildingManager', '2024-05-15', '15', '[URL]', '[URL]', '', 'Approved', '2023-02-01', 'Hardworking', '3.9', 'Emp'
)INSERT INTO Applicant VALUES ('29', '2023-01-25', 'Business', 'Spring', 'PersonalTrainer', 'ComputerTech', '2026-05-18', '15', '[URL]', '[URL]', '[URL]', 'Approved', '2023-02-01', 'Good candidate', '3.85', 'Emp'
)INSERT INTO Applicant VALUES ('30', '2023-01-26', 'Business', 'Spring', 'PersonalTrainer', 'GroupFitness', '2025-05-20', '15', '[URL]', '', '[URL]', 'Pending', '2023-02-01', 'Questionable', '3.22', 'Emp'
)INSERT INTO Applicant VALUES ('31', '2023-01-27', 'Engineering', 'Spring', 'FitnessAreaFloorSupervisor', 'PersonalTrainer', '2025-05-20', '12', '[URL]', '[URL]', '', 'Approved', '2023-02-01', 'Smart', '3.5', 'Emp'
)INSERT INTO Applicant VALUES ('32', '2023-01-28', 'Business', 'Spring', 'IntramuralAssistant', 'GroupFitness', '2025-05-20', '25', '[URL]', '', '', 'Approved', '2023-02-01', 'Smart', '3.6', 'Emp'
)INSERT INTO Applicant VALUES ('33', '2023-01-29', 'Education', 'Spring', 'ComputerTech', 'PersonalTrainer', '2026-05-18', '5', '[URL]', '', '', 'Approved', '2023-02-01', 'Hardworking', '3.9', 'Emp'
)INSERT INTO Applicant VALUES ('34', '2023-01-30', 'Psychology', 'Spring', 'PersonalTrainer', 'GroupFitness', '2026-05-18', '25', '[URL]', '', '', 'Approved', '2023-02-01', 'Friendly', '4', 'Emp'
)INSERT INTO Applicant VALUES ('35', '2023-01-31', 'Biology', 'Spring', 'PersonalTrainer', 'Receptionist', '2026-05-18', '12', '[URL]', '', '[URL]', 'Approved', '2023-02-01', 'Quick learner', '3.98', 'Emp'
)
 
INSERT INTO Employee VALUES ('Em1', 'Receptionist', '15', 'M', '[URL]', '6'
)INSERT INTO Employee VALUES ('Em2', 'UFitAssistant', '18', 'L', '[URL]', '10'
)INSERT INTO Employee VALUES ('Em3', 'MarketingGraphicDesign', '12', 'M', '[URL]', '11'
)INSERT INTO Employee VALUES ('Em4', 'FitnessAreaFloorTrainer', '14', 'L', '[URL]', '13'
)INSERT INTO Employee VALUES ('Em5', 'PersonalTrainer', '12', 'XL', '[URL]', '15'
)INSERT INTO Employee VALUES ('Em6', 'PersonalTrainer', '15', 'L', '[URL]', '16'
)INSERT INTO Employee VALUES ('Em7', 'FitnessAreaFloorSupervisor', '15', 'XXL', '[URL]', '17'
)INSERT INTO Employee VALUES ('Em8', 'IntramuralAssistant', '15', 'S', '[URL]', '18'
)INSERT INTO Employee VALUES ('Em9', 'ComputerTech', '20', 'M', '[URL]', '19'
)INSERT INTO Employee VALUES ('Em10', 'PersonalTrainer', '18', 'M', '[URL]', '20'
)INSERT INTO Employee VALUES ('Em11', 'PersonalTrainer', '12', 'M', '[URL]', '21'
)INSERT INTO Employee VALUES ('Em12', 'PersonalTrainer', '12', 'L', '[URL]', '22'
)INSERT INTO Employee VALUES ('Em13', 'PersonalTrainer', '14', 'L', '[URL]', '23'
)INSERT INTO Employee VALUES ('Em14', 'PersonalTrainer', '13.5', 'L', '[URL]', '24'
)INSERT INTO Employee VALUES ('Em15', 'PersonalTrainer', '13', 'L', '[URL]', '25'
)INSERT INTO Employee VALUES ('Em16', 'GroundsMaintenanceAssistant', '12.5', 'M', '[URL]', '26'
)INSERT INTO Employee VALUES ('Em17', 'GroupFitness', '17.5', 'S', '[URL]', '27'
)INSERT INTO Employee VALUES ('Em18', 'BuildingManager', '16', 'XL', '[URL]', '28'
)INSERT INTO Employee VALUES ('Em19', 'ComputerTech', '15', 'L', '[URL]', '29'
)INSERT INTO Employee VALUES ('Em20', 'GroupFitness', '17', 'L', '[URL]', '30'
)INSERT INTO Employee VALUES ('Em21', 'PersonalTrainer', '13', 'M', '[URL]', '31'
)INSERT INTO Employee VALUES ('Em22', 'GroupFitness', '14', 'L', '[URL]', '32'
)INSERT INTO Employee VALUES ('Em23', 'MarketingGraphicDesign', '16', 'S', '[URL]', '33'
)INSERT INTO Employee VALUES ('Em24', 'PersonalTrainer', '14.5', 'L', '[URL]', '34'
)INSERT INTO Employee VALUES ('Em25', 'PersonalTrainer', '12.5', 'XL', '[URL]', '35'
)
 
INSERT INTO Alumni VALUES ('Al1', 'Pay', 'None', '2020-05-20', '2'
)INSERT INTO Alumni VALUES ('Al2', 'Pay', 'Great experience', '2020-05-20', '1'
)INSERT INTO Alumni VALUES ('Al3', 'School', 'None', '2019-05-21', '3'
)INSERT INTO Alumni VALUES ('Al4', 'School', 'Great experience', '2019-05-21', '5'
)INSERT INTO Alumni VALUES ('Al5', 'Pay', 'None', '2019-05-21', '4'
)INSERT INTO Alumni VALUES ('Al6', 'School', 'None', '2018-12-21', '7'
)INSERT INTO Alumni VALUES ('Al7', 'Personal', 'Horrible experience', '2018-05-21', '8'
)INSERT INTO Alumni VALUES ('Al8', 'School', 'None', '2018-05-21', '9'
)INSERT INTO Alumni VALUES ('Al9', 'Personal', 'None', '2017-12-22', '12'
)INSERT INTO Alumni VALUES ('Al10', 'Pay', 'None', '2017-12-22', '14'
)
 
INSERT INTO Certification VALUES ('Cert1', 'CCA', '2023-02-28'
)INSERT INTO Certification VALUES ('Cert2', 'CPR', '2024-01-01'
)INSERT INTO Certification VALUES ('Cert3', 'Lifeguard', '2023-12-31'
)INSERT INTO Certification VALUES ('Cert4', 'CPR', '2025-01-01'
)INSERT INTO Certification VALUES ('Cert5', 'FirstAid', '2025-12-31'
)INSERT INTO Certification VALUES ('Cert6', 'IT', '2027-12-31'
)INSERT INTO Certification VALUES ('Cert7', 'Yoga', '2024-06-21'
)INSERT INTO Certification VALUES ('Cert8', 'PersonalTraining', '2024-05-20'
)INSERT INTO Certification VALUES ('Cert9', 'Yoga', '2023-02-28'
)INSERT INTO Certification VALUES ('Cert10', 'FirstAid', '2024-01-01'
)INSERT INTO Certification VALUES ('Cert11', 'FirstAid', '2023-12-31'
)INSERT INTO Certification VALUES ('Cert12', 'CPR', '2025-01-01'
)INSERT INTO Certification VALUES ('Cert13', 'Lifeguard', '2025-12-31'
)
 
INSERT INTO CertificateType VALUES ('CType1', '2', 'Cert1', 'FirstAid'
)INSERT INTO CertificateType VALUES ('CType2', '5', 'Cert2', 'LEED'
)INSERT INTO CertificateType VALUES ('CType3', '8', 'Cert3', 'CPR'
)INSERT INTO CertificateType VALUES ('CType4', '13', 'Cert4', 'Lifeguard'
)INSERT INTO CertificateType VALUES ('CType5', '7', 'Cert5', 'OSHA'
)INSERT INTO CertificateType VALUES ('CType6', '10', 'Cert6', 'Yoga'
)INSERT INTO CertificateType VALUES ('CType7', '11', 'Cert7', 'PersonalTraining'
)INSERT INTO CertificateType VALUES ('CType8', '15', 'Cert8', 'Spanish'
)INSERT INTO CertificateType VALUES ('CType9', '20', 'Cert9', 'French'
)INSERT INTO CertificateType VALUES ('CType10', '3', 'Cert10', 'Teaching'
)INSERT INTO CertificateType VALUES ('CType11', '6', 'Cert11', 'Accounting'
)INSERT INTO CertificateType VALUES ('CType12', '9', 'Cert12', 'IT'
)INSERT INTO CertificateType VALUES ('CType13', '12', 'Cert13', 'CCA'
)
 
INSERT INTO JobHistory VALUES ('JH1', 'ParkRanger', 'Maintence', 'AngelineHunter', '771-730-6629', '2021-02-20', '2022-01-26', 'GrandTetonNationalPark', '1'
)INSERT INTO JobHistory VALUES ('JH2', 'StoreManager', 'Management', 'GracieStafford', '958-385-8139', '2020-02-24', '2021-11-17', 'Walgreens', '2'
)INSERT INTO JobHistory VALUES ('JH3', 'Intern', 'Sales', 'KurtisDuarte', '870-365-2905', '2019-02-24', '2022-01-03', 'Pepsico', '3'
)INSERT INTO JobHistory VALUES ('JH4', 'Cashier', 'CustomerService', 'SoniaBray', '962-847-0164', '2021-02-24', '2021-10-29', 'ShakeShack', '4'
)INSERT INTO JobHistory VALUES ('JH5', 'LandScaper', 'Maintence', 'RaleighByrd', '436-421-7264', '2021-02-25', '2021-12-13', 'BubbasLawnService', '5'
)INSERT INTO JobHistory VALUES ('JH6', 'Recepetionist', 'Adminstration', 'RhodaConway', '315-477-4515', '2020-02-25', '2020-09-09', 'ConwayLawFirm', '6'
)INSERT INTO JobHistory VALUES ('JH7', 'Server', 'CustomerService', 'OraSchmidt', '684-214-6329', '2019-05-21', '2022-02-01', 'AubreysResturaunt', '7'
)INSERT INTO JobHistory VALUES ('JH8', 'PropertyManager', 'Management', 'TylerRichard', '621-808-8839', '2020-06-02', '2022-03-24', 'ApexRealtors', '8'
)INSERT INTO JobHistory VALUES ('JH9', 'Intern', 'Marketing', 'SheliaSingleton', '951-241-6010', '2020-10-26', '2021-09-13', 'RedundantCosulting', '9'
)INSERT INTO JobHistory VALUES ('JH10', 'UFitAssistant', 'Fitness', 'DominickPetersen', '891-832-9801', '2019-05-27', '2022-07-06', 'SpeedyDrivers', '10'
)INSERT INTO JobHistory VALUES ('JH11', 'MarketingGraphicDesign', 'Administration', 'HaywoodMack', '342-243-5920', '2021-09-28', '2022-03-27', 'LosPrimosGrill', '11'
)INSERT INTO JobHistory VALUES ('JH12', 'Server', 'CustomerService', 'CandiceStuart', '308-987-2161', '2021-07-02', '2022-08-04', 'ElMezcalResturaunt', '12'
)INSERT INTO JobHistory VALUES ('JH13', 'FitnessAreaFloorTrainer', 'Fitness', 'ShadGood', '973-349-7471', '2020-10-28', '2021-12-15', 'BradentonCoEMS', '13'
)INSERT INTO JobHistory VALUES ('JH14', 'LandScaper', 'Maintence', 'EzequielLiu', '714-956-5045', '2020-03-29', '2022-04-20', 'TrueGreenLawnCare', '14'
)INSERT INTO JobHistory VALUES ('JH15', 'PersonalTrainer', 'Wellness', 'CorrineFitzgerald', '746-503-2652', '2021-10-25', '2022-09-14', 'SilversGym', '15'
)INSERT INTO JobHistory VALUES ('JH16', 'PersonalTrainer', 'Wellness', 'StephenVazquez', '476-656-4549', '2019-02-16', '2020-01-06', 'OfficeFurniturePlus', '16'
)INSERT INTO JobHistory VALUES ('JH17', 'FitnessAreaFloorTrainer', 'Fitness', 'CollinMahoney', '205-893-5686', '2020-04-03', '2022-08-19', 'Calhouns', '17'
)INSERT INTO JobHistory VALUES ('JH18', 'IntramuralAssistant', 'Fitness', 'BernieTran', '483-456-4608', '2020-06-12', '2021-11-27', 'SparklingServices', '18'
)INSERT INTO JobHistory VALUES ('JH19', 'ComputerTech', 'Information Systems', 'SammyRoss', '282-686-8205', '2021-11-13', '2022-05-04', 'CovenantMedical', '19'
)INSERT INTO JobHistory VALUES ('JH20', 'PersonalTrainer', 'Wellness', 'KristiPalmer', '672-652-2327', '2019-01-04', '2020-07-07', 'Mcdonalds', '20'
)INSERT INTO JobHistory VALUES ('JH21', 'PersonalTrainer', 'Wellness', 'SaundraShelton', '998-633-0928', '2021-06-06', '2022-03-15', 'RahleighHighSchool', '21'
)INSERT INTO JobHistory VALUES ('JH22', 'PersonalTrainer', 'Welness', 'KenyaScott', '532-520-3362', '2020-03-17', '2021-01-07', 'SouthSideOutpatientClinic', '22'
)INSERT INTO JobHistory VALUES ('JH23', 'PersonalTrainer', 'Wellness', 'SeptonFarcey', '869-723-2642', '2021-05-07', '2021-12-07', 'D3Training', '23'
)INSERT INTO JobHistory VALUES ('JH24', 'PersonalTrainer', 'Wellness', 'RoccoMcgee', '523-744-1347', '2021-09-20', '2022-02-23', 'SpineAndSport', '24'
)INSERT INTO JobHistory VALUES ('JH25', 'PersonalTrainer', 'Welness', 'MaxCastaneda', '505-606-2803', '2022-08-28', '2023-01-03', 'LePepeBistro', '25'
)INSERT INTO JobHistory VALUES ('JH26', 'GroundMaintenanceAssistant', 'Maintence', 'CaseyDaugherty', '547-263-7094', '2020-05-25', '2020-09-21', 'UniverseFitness', '26'
)INSERT INTO JobHistory VALUES ('JH27', 'GroupFitness', 'Fitness', 'CorrineFitzgerald', '746-503-2652', '2019-11-25', '2021-03-24', 'SilversGym', '27'
)INSERT INTO JobHistory VALUES ('JH28', 'BuildingManager', 'Managemet', 'MattieWagner', '794-785-6921', '2020-10-25', '2022-09-16', 'D3Training', '28'
)INSERT INTO JobHistory VALUES ('JH29', 'ComputerTech', 'Information Systems', 'WhitneyLizard', '446-803-2838', '2021-04-25', '2021-11-19', 'NorthsideRehabilitation', '29'
)INSERT INTO JobHistory VALUES ('JH30', 'GroupFitness', 'Fitness', 'DougieWilliams', '806-309-6302', '2021-12-26', '2022-10-23', 'SilversGym', '30'
)INSERT INTO JobHistory VALUES ('JH31', 'PersonalTrainer', 'Wellness', 'LucienOrtiz', '381-251-6461', '2021-07-27', '2022-04-14', 'AubreysResturaunt', '31'
)INSERT INTO JobHistory VALUES ('JH32', 'GroupFitness', 'Fitness', 'DarellBush', '745-370-5025', '2020-05-28', '2020-12-03', 'Target', '32'
)INSERT INTO JobHistory VALUES ('JH33', 'MarketingGraphicDesign', 'Administration', 'RhettGriffin', '661-928-6084', '2019-03-12', '2022-02-07', 'VideoSolutions', '33'
)INSERT INTO JobHistory VALUES ('JH34', 'PersonalTrainer', 'Wellness', 'SteveDeleon', '884-553-5665', '2021-06-20', '2021-09-12', 'StJosephHighschool', '34'
)INSERT INTO JobHistory VALUES ('JH35', 'PersonalTrainer', 'Wellness', 'GladysNunez', '249-969-9900', '2018-05-08', '2022-11-20', 'UniverseFitness', '35'
) 

INSERT INTO Contact VALUES ('Con1', 'Permanent', 'Evelyn', 'Short', 'C', '120 Monroe St.', 'Bartlett', 'IL', '60103', '555-908-7592', '555-327-9115', 'EvelynShort@hotmail.com', '1'
)INSERT INTO Contact VALUES ('Con2', 'Emergency', 'Rosemary', 'Bradshaw', 'F', '145 S. Blackburn Street', 'Wyoming ', 'MI', '49509', '', '977-948-8863', 'RosemaryBradshaw0@gmail.com', '2'
)INSERT INTO Contact VALUES ('Con3', 'Permanent', 'Leo', 'Oneill', 'E', '9864 North Shore Road', 'Macungie', 'PA', '18062', '347-913-0837', '347-619-7444', 'OneillLeo4@yahoomail.com ', '3'
)INSERT INTO Contact VALUES ('Con4', 'Permanent', 'Jimmy', 'Hays', 'A', '417 Redwood St.', 'Glendora', 'CA', '91740', '311-518-8084', '311-284-4299', 'JimmyHays2@aoc.com', '4'
)INSERT INTO Contact VALUES ('Con5', 'Permanent', 'Tasha', 'Brooks', 'B', '659 Glen Eagles St.', 'Romulus ', 'MI', '48174', '', '560-773-5557', 'TashaBrooks@gmail.com', '5'
)INSERT INTO Contact VALUES ('Con6', 'Permanent', 'Marisa', 'Baxter', 'B', '979 Race Drive', 'Cedar Rapids', 'IA', '52402', '', '931-659-2814', 'MarisaBaxter78@bing.com', '6'
)INSERT INTO Contact VALUES ('Con7', 'Permanent', 'Verna', 'Dennis', 'J', '8627 Rockville Street', 'Ozone Park', 'NY', '11417', '', '409-252-8606', 'VernaDennis23@yahoomail.com', '7'
)INSERT INTO Contact VALUES ('Con8', 'Permanent', 'Samuel', 'Walsh', 'E', '8096 Bradford Rd.', 'Morrisville', 'PA', '19067', '', '944-426-5633', 'SamuelWalsh44@outllook.com', '8'
)INSERT INTO Contact VALUES ('Con9', 'Permanent', 'Marcos', 'McCoy', 'S', '1910 Carpenter Street', 'South Plainfield', 'NJ', '27080', '', '944-951-3295', 'McCoyMarcos09@bing.com', '9'
)INSERT INTO Contact VALUES ('Con10', 'Emergency', 'Juana', 'Luna', 'Q', '227 W. Hamilton Dr.', 'Ambler ', 'PA', '19002', '971-683-9183', '971-698-3288', 'JuanaLunatn@hotmail.com', '10'
)INSERT INTO Contact VALUES ('Con11', 'Emergency', 'Rachel', 'Whitney', 'J', '451 Linda St.', 'Collierville', 'TN', '38017', '783-934-4272', '782-393-8143', 'RachelWhitney00@gmail.com', '11'
)INSERT INTO Contact VALUES ('Con12', 'Emergency', 'Holly', 'Eaton', 'E', '932 Southampton Street', 'Deland ', 'FL ', '32720', '437-683-5281', '437-260-8650', 'HollyEaton@hotmail.com', '12'
)INSERT INTO Contact VALUES ('Con13', 'Emergency', 'Brandi', 'Newton', 'M', '8600 High Point St.', 'Seattle ', 'WA', '98144', '', '979-399-2938', 'BrandiNewtonwa@outlook.com', '13'
)INSERT INTO Contact VALUES ('Con14', 'Emergency', 'Ida', 'Hanna', 'E', '980 Acacia St.', 'Winter Springs ', 'FL ', '32708', '', '679-213-9620', 'IdaHanna7@bing.com', '14'
)INSERT INTO Contact VALUES ('Con15', 'Emergency', 'Jordan', 'Stephens', 'A', '7966 Hawthorne Ave.', 'Wheaton', 'IL ', '60187', '', '642-718-1041', 'JordanStephens34@', '15'
)INSERT INTO Contact VALUES ('Con16', 'Permanent', 'Aida', 'Dillon', 'M', '201 Tunnel Lane', 'Villa Park ', 'IL ', '60181', '', '596-857-4348', 'DillonAida111@gmail.com', '16'
)INSERT INTO Contact VALUES ('Con17', 'Emergency', 'Katherine', 'Coon', 'G', '621 University Ave.', 'Jupiter ', 'FL ', '33458', '', '788-546-1125', 'CoonKatherinefl@bing.com', '17'
)INSERT INTO Contact VALUES ('Con18', 'Emergency', 'Virginia', 'Simmons', 'E', '9743 Cedarwood Dr.', 'Noblesville ', 'IN ', '46060', '821-853-4730', '821-972-7890', 'VirginiaSimmons00@outlook.com', '18'
)INSERT INTO Contact VALUES ('Con19', 'Permanent', 'Delores', 'Harvey', 'D', '9246 Cedar Street', 'Joilet ', 'IL ', '60435', '', '769-791-7763', 'DeloresHarvey@aoc.com', '19'
)INSERT INTO Contact VALUES ('Con20', 'Emergency', 'Victor', 'Ferguson', 'D', '253 Madison Ave.', 'Bridgeport', 'CT', '26606', '', '373-692-0166', 'FergusonVictor99@gmail.com', '20'
)INSERT INTO Contact VALUES ('Con21', 'Permanent', 'Owen', 'Frank', 'V', '130 Atlantic Ave.', 'Hickory', 'NC', '28601', '', '846-249-3801', 'OwenFrank22@outlook.com', '21'
)INSERT INTO Contact VALUES ('Con22', 'Emergency', 'Tommy', 'Roth', 'E', '738 South Windsor St.', 'Fargo', 'ND', '58102', '822-723-6286', '822-855-2124', 'TommyRoth89@bing.com', '22'
)INSERT INTO Contact VALUES ('Con23', 'Permanent', 'Shawna', 'Horn', 'M', '1450 Manchester Rd.', 'East Orange', 'NJ', '17017', '991-672-1371', '991-283-4115', 'ShawnaHorn@yahoomail.com', '23'
)INSERT INTO Contact VALUES ('Con24', 'Permanent', 'Renee', 'Sharp', 'D', '589 Silver Spear Rd.', 'Loxahatchee ', 'FL ', '33470', '', '380-313-6573', 'SharpRenee45@hotmail.com', '24'
)INSERT INTO Contact VALUES ('Con25', 'Permanent', 'Marcia', 'McCann', 'S', '938 Windsor Ave.', 'Enterprise', 'AL', '36330', '', '537-855-1515', 'MarciaMcCann@gmail.com', '25'
)INSERT INTO Contact VALUES ('Con26', 'Permanent', 'Corinne', 'Barrett', 'J', '8741 Crescent St.', 'Bonita Springs', 'FL ', '34135', '', '824-207-8878', 'CorinneBarrett02@yahoomail.com', '26'
)INSERT INTO Contact VALUES ('Con27', 'Emergency', 'Antoinette', 'Moses', 'K', '8391 North Paris Hill Street', 'Scarsdale', 'NY', '10583', '659-419-4865', '659-260-5825', 'AntoinetteMoses@outlook.com', '27'
)INSERT INTO Contact VALUES ('Con28', 'Emergency', 'Eunice', 'Flowers', 'P', '526 West County Street', 'Great Falls', 'MT', '59404', '', '444-916-9014', 'EuniceFlowers55@outlook.com', '28'
)INSERT INTO Contact VALUES ('Con29', 'Permanent', 'Betty', 'Wheeler', 'D', '814 Manor Station Drive', 'Valley Stream', 'NY', '11580', '', '946-796-9447', 'WheelerBetty@gmail.com', '29'
)INSERT INTO Contact VALUES ('Con30', 'Emergency', 'Angie', 'Dunlap', 'J', '747 Cambridge Ave.', 'Midlothian', 'VA', '23112', '', '950-372-7661', 'AngieDunlap08@hotmail.com', '30'
)INSERT INTO Contact VALUES ('Con31', 'Permanent', 'Mitch', 'Byers', 'R', '511 Chestnut Drive', 'Saint Charles', 'IL', '60174', '424-487-2027', '424-340-9521', 'MitchByers@yahoomail.com', '31'
)INSERT INTO Contact VALUES ('Con32', 'Permanent', 'Gordon', 'Murray', 'A', '845 Gainsway St.', 'Selden', 'NY', '11784', '', '420-296-6567', 'GordonMurray45@bing.com', '32'
)INSERT INTO Contact VALUES ('Con33', 'Permanent', 'Cathy', 'Schmitt', 'H', '864 Berkshire St.', 'Saint Joseph', 'MI', '49085', '', '348-370-9877', 'SchmittCathy@yahoomail.com', '33'
)INSERT INTO Contact VALUES ('Con34', 'Permanent', 'Charlene', 'Simons', 'E', '603 1st Court', 'Biloxi', 'MS', '39532', '', '967-301-2338', 'CharleneSimons11@gmail.com', '34'
)INSERT INTO Contact VALUES ('Con35', 'Permanent', 'Frankie', 'Maxwell', 'J', '461 Birch Hill Court', 'Miami', 'FL ', '33125', '776-821-6350', '776-212-1275', 'FrankieMaxwell21@gmail.com', '35'
) 

INSERT INTO Availability VALUES ('Avail1', '08:00:00', '11:59:00', '17:30:00', '21:00:00', '08:00:00', '12:00:00', '6'
)INSERT INTO Availability VALUES ('Avail2', '08:30:00', '10:30:00', '13:30:00', '21:00:00', '12:00:00', '16:00:00', '7'
)INSERT INTO Availability VALUES ('Avail3', '10:00:00', '11:59:00', '14:00:00', '21:00:00', '15:00:00', '18:00:00', '8'
)INSERT INTO Availability VALUES ('Avail4', '07:00:00', '10:00:00', '15:00:00', '20:00:00', '00:00:00', '00:00:00', '9'
)INSERT INTO Availability VALUES ('Avail5', '07:30:00', '09:30:00', '12:00:00', '19:00:00', '08:00:00', '12:00:00', '10'
)INSERT INTO Availability VALUES ('Avail6', '09:30:00', '11:00:00', '14:00:00', '18:00:00', '12:00:00', '16:00:00', '11'
)INSERT INTO Availability VALUES ('Avail7', '09:00:00', '11:00:00', '17:30:00', '21:00:00', '15:00:00', '18:00:00', '12'
)INSERT INTO Availability VALUES ('Avail8', '11:30:00', '11:59:00', '13:30:00', '17:00:00', '00:00:00', '00:00:00', '13'
)INSERT INTO Availability VALUES ('Avail9', '08:00:00', '11:00:00', '14:00:00', '16:00:00', '11:00:00', '15:00:00', '14'
)INSERT INTO Availability VALUES ('Avail10', '08:30:00', '11:00:00', '15:00:00', '18:00:00', '00:00:00', '00:00:00', '15'
)INSERT INTO Availability VALUES ('Avail11', '10:00:00', '11:59:00', '12:00:00', '14:00:00', '10:00:00', '14:00:00', '16'
)INSERT INTO Availability VALUES ('Avail12', '07:00:00', '11:00:00', '14:00:00', '21:00:00', '10:00:00', '14:00:00', '17'
)INSERT INTO Availability VALUES ('Avail13', '07:30:00', '11:00:00', '12:00:00', '13:00:00', '00:00:00', '00:00:00', '18'
)INSERT INTO Availability VALUES ('Avail14', '09:30:00', '11:59:00', '17:00:00', '19:00:00', '13:00:00', '17:00:00', '19'
)
 
INSERT INTO Program VALUES ('900001', 'Intramurals', 'Trains fitnessclub members in the programs they need', 'Em5'
)INSERT INTO Program VALUES ('900002', 'Aquatics', 'Trains fitnessclub members in the programs they need', 'Em6'
)INSERT INTO Program VALUES ('900003', 'HealthWellness', 'Trains fitnessclub members in the programs they need', 'Em10'
)INSERT INTO Program VALUES ('900004', 'Yoga', 'Trains fitnessclub members in the programs they need', 'Em11'
)INSERT INTO Program VALUES ('900005', 'Weightlifting', 'Trains fitnessclub members in the programs they need', 'Em12'
)INSERT INTO Program VALUES ('900006', 'Volunteer', 'Trains fitnessclub members in the programs they need', 'Em13'
)INSERT INTO Program VALUES ('900007', 'RacketSports', 'Trains fitnessclub members in the programs they need', 'Em14'
)INSERT INTO Program VALUES ('900008', 'Cardio', 'Trains fitnessclub members in the programs they need', 'Em15'
)INSERT INTO Program VALUES ('900009', 'Fundraiser', 'Trains fitnessclub members in the programs they need', 'Em21'
)INSERT INTO Program VALUES ('900010', 'Dance', 'Trains fitnessclub members in the programs they need', 'Em24'
)INSERT INTO Program VALUES ('900011', 'Outdoors', 'Trains fitnessclub members in the programs they need', 'Em25'
)INSERT INTO Program VALUES ('900012', 'FreeTrain', 'A Hawkins U-Fit program that allows for uninstructed free use of Hawkins facilities', 'Em7'
)INSERT INTO Program VALUES ('900013', 'Administration', 'A Hawkins U-Fit program that encompasses all of Hawkins U-Fits administrative needs.', 'Em19'
)INSERT INTO Program VALUES ('900014', 'Facilities ', 'A Hawkins U-Fit program that is incharge of fixing and maintaining all of Hawkins ', 'Em18'
)
 
INSERT INTO ProgramActivities VALUES ('Act1', 'Tournament', '2023-03-12', '2023-03-12', '0', 'Em10', '900001'
)INSERT INTO ProgramActivities VALUES ('Act2', 'SwimmingLessons', '2023-04-06', '2023-04-06', '10', 'Em12', '900002'
)INSERT INTO ProgramActivities VALUES ('Act3', 'DietaryClass', '2023-03-22', '2023-03-22', '25', 'Em11', '900003'
)INSERT INTO ProgramActivities VALUES ('Act4', 'YogaClass', '2022-08-20', '2022-08-20', '0', 'Em22', '900004'
)INSERT INTO ProgramActivities VALUES ('Act5', 'BenchPressandBicepsClass', '2022-08-20', '2022-08-20', '0', 'Em7', '900005'
)INSERT INTO ProgramActivities VALUES ('Act6', 'TrashCleanup', '2022-08-20', '2022-08-20', '0', 'Em17', '900006'
)INSERT INTO ProgramActivities VALUES ('Act7', 'BenchPressandBicepsClass', '2022-08-20', '2022-08-20', '0', 'Em8', '900007'
)INSERT INTO ProgramActivities VALUES ('Act8', 'SpinClass', '2022-08-20', '2022-08-20', '5', 'Em4', '900008'
)INSERT INTO ProgramActivities VALUES ('Act9', 'BasketballFundraiser', '2023-01-12', '2023-01-12', '0', 'Em15', '900009'
)INSERT INTO ProgramActivities VALUES ('Act10', 'Zumba', '2023-02-24', '2023-02-24', '50', 'Em20', '900010'
)

INSERT INTO EmployeeActivity VALUES ('EmpAct1', 'Em10', 'Act1'
)INSERT INTO EmployeeActivity VALUES ('EmpAct2', 'Em12', 'Act2'
)INSERT INTO EmployeeActivity VALUES ('EmpAct3', 'Em11', 'Act3'
)INSERT INTO EmployeeActivity VALUES ('EmpAct4', 'Em22', 'Act4'
)INSERT INTO EmployeeActivity VALUES ('EmpAct5', 'Em7', 'Act5'
)INSERT INTO EmployeeActivity VALUES ('EmpAct6', 'Em17', 'Act6'
)INSERT INTO EmployeeActivity VALUES ('EmpAct7', 'Em8', 'Act7'
)INSERT INTO EmployeeActivity VALUES ('EmpAct8', 'Em4', 'Act8'
)INSERT INTO EmployeeActivity VALUES ('EmpAct9', 'Em15', 'Act9'
)INSERT INTO EmployeeActivity VALUES ('EmpAct10', 'Em20', 'Act10'
)
 
INSERT INTO Raise VALUES ('R1', '0.5', '2023-01-01', 'Team player', 'Em10'
)INSERT INTO Raise VALUES ('R2', '1', '2023-01-01', 'Team player', 'Em11'
)INSERT INTO Raise VALUES ('R3', '2', '2023-01-01', 'Great', 'Em12'
)INSERT INTO Raise VALUES ('R4', '3', '2023-01-01', 'Phenomenal Work Ethic', 'Em13'
)INSERT INTO Raise VALUES ('R5', '4', '2023-01-01', 'Flexible', 'Em14'
)INSERT INTO Raise VALUES ('R6', '4.5', '2023-01-01', 'Vital Asset', 'Em15'
)INSERT INTO Raise VALUES ('R7', '3.5', '2023-01-01', 'Great', 'Em16'
)INSERT INTO Raise VALUES ('R8', '3.25', '2023-01-01', 'Leadership skills', 'Em17'
)INSERT INTO Raise VALUES ('R9', '5', '2023-01-01', 'Vital Asset', 'Em18'
)INSERT INTO Raise VALUES ('R10', '2.25', '2023-01-30', 'Great leader', 'Em19'
)INSERT INTO Raise VALUES ('R11', '2.5', '2023-01-30', 'Team player', 'Em20'
)INSERT INTO Raise VALUES ('R12', '3', '2023-01-30', 'Phenomenal Work Ethic', 'Em21'
)INSERT INTO Raise VALUES ('R13', '1.25', '2023-01-30', 'Flexible', 'Em22'
)
 
INSERT INTO Involvement VALUES ('Club President', 'Em15'
)INSERT INTO Involvement VALUES ('Club Treasurer', 'Em16'
)INSERT INTO Involvement VALUES ('Volunteer', 'Em17'
)INSERT INTO Involvement VALUES ('Intramurals', 'Em18'
)INSERT INTO Involvement VALUES ('Club Founder', 'Em19'
)INSERT INTO Involvement VALUES ('Volunteer', 'Em22'
)INSERT INTO Involvement VALUES ('Intramurals', 'Em23'
)INSERT INTO Involvement VALUES ('Volunteer', 'Em21'
)INSERT INTO Involvement VALUES ('Student Gov', 'Em2'
)INSERT INTO Involvement VALUES ('Student Gov', 'Em6'
)INSERT INTO Involvement VALUES ('Volunteer', 'Em5'
)

INSERT INTO Participants VALUES ('Part1', 'Karen', 'Miranda', '8384 Fifth Drive', 'Casselberry', 'FL', '32707', '697-926-6102', 'Female', '2009-02-10', '2023-01-13', 'Act10'
)INSERT INTO Participants VALUES ('Part2', 'Nelda', 'Kennedy', '46 Pine Road', 'Yonkers', 'NY', '10701', '227-369-7815', 'Female', '2009-09-03', '2023-01-02', 'Act9'
)INSERT INTO Participants VALUES ('Part3', 'Ina', 'Delgado', '337 South Courtland Avenue', 'Norwalk', 'CT', '26851', '490-469-1541', 'Female', '1994-08-15', '2023-03-26', 'Act2'
)INSERT INTO Participants VALUES ('Part4', 'Rosetta', 'Shepard', '765 Homestead Street', 'Mchenry', 'IL', '60050', '693-443-5786', 'Male', '1999-03-05', '2023-01-22', 'Act10'
)INSERT INTO Participants VALUES ('Part5', 'Ginger', 'Estes', '9448 Eagle Drive', 'King Of Prussia', 'PA', '19406', '669-609-5595', 'Female', '2012-06-28', '2022-07-23', 'Act8'
)INSERT INTO Participants VALUES ('Part6', 'Cordell', 'Rivers', '7093 Chapel St.', 'Rockaway', 'NJ', '27866', '433-945-0169', 'Male', '1996-03-11', '2022-11-19', 'Act9'
)INSERT INTO Participants VALUES ('Part7', 'Rey', 'Wells', '8178 Plumb Branch Lane', 'Endicott', 'NY', '13760', '412-295-3845', 'Female', '2000-05-20', '2023-02-17', 'Act2'
)INSERT INTO Participants VALUES ('Part8', 'Jody', 'Kemp', '151 Primrose Road', 'Elk Grove Village', 'IL', '60007', '811-884-2453', 'Male', '2010-08-23', '2022-05-25', 'Act5'
)INSERT INTO Participants VALUES ('Part9', 'Odessa', 'Conner', '7634 Peachtree Road', 'Lady Lake', 'FL', '32159', '923-514-8657', 'Male', '1990-12-02', '2022-11-24', 'Act10'
)INSERT INTO Participants VALUES ('Part10', 'Levi', 'Sheppard', '44 North Chapel St.', 'Royersford', 'PA', '19468', '454-532-8363', 'Male', '1995-12-23', '2022-06-09', 'Act8'
)INSERT INTO Participants VALUES ('Part11', 'Joey', 'Barber', '28 Essex Street', 'Medford', 'MA', '42155', '252-659-4979', 'Male', '2011-09-03', '2022-12-06', 'Act9'
)INSERT INTO Participants VALUES ('Part12', 'Gene', 'Callahan', '302 Thompson St.', 'Jacksonville Beach', 'FL', '32250', '274-593-3745', 'Male', '1992-07-25', '2022-07-21', 'Act7'
)INSERT INTO Participants VALUES ('Part13', 'Clarissa', 'Blackburn', '41 E. Wentworth Road', 'Toms River', 'NJ', '18753', '463-785-8985', 'Female ', '1996-04-17', '2023-01-09', 'Act9'
)INSERT INTO Participants VALUES ('Part14', 'Reginald', 'Donovan', '773 Yukon Lane', 'Fairhope', 'AL', '36532', '438-514-4115', 'Male', '2009-08-18', '2023-02-12', 'Act10'
)INSERT INTO Participants VALUES ('Part15', 'Tamera', 'Patton', '183 S. St Louis Street', 'Uniontown', 'PA', '15401', '653-305-9131', 'Female', '1995-12-21', '2022-05-10', 'Act7'
)
 
INSERT INTO Roles VALUES ('Role1', 'PersonalTrainer', '12', 'Trains fitnessclub members in the programs they need', '20'
)INSERT INTO Roles VALUES ('Role2', 'SwimCoach', '13', 'Coaches swim class', '20'
)INSERT INTO Roles VALUES ('Role3', 'Dietician', '12', 'Teaches diet classes', '20'
)INSERT INTO Roles VALUES ('Role4', 'YogaInstructor', '14', 'Teaches yoga classes', '15'
)INSERT INTO Roles VALUES ('Role5', 'WeightTrainer', '15', 'Leads weightlifting sessions', '10'
)INSERT INTO Roles VALUES ('Role6', 'Volunteer Leader', '12', 'Leads volunteer events', '12'
)INSERT INTO Roles VALUES ('Role7', 'TennisCoach', '12.5', 'Teaches tennis lessons', '15'
)INSERT INTO Roles VALUES ('Role8', 'PersonalTrainer', '13', 'Teaches running courses', '15'
)INSERT INTO Roles VALUES ('Role9', 'FundrasiningLeader', '11', 'Leads fundraising events', '15'
)INSERT INTO Roles VALUES ('Role10', 'DanceInstructor', '10', 'Teaches dance classes', '12'
)INSERT INTO Roles VALUES ('Role11', 'RockClimbingInstructor', '10.5', 'Teaches rock climbing classes', '20'
)INSERT INTO Roles VALUES ('Role12', 'IntramuralManager', '12', 'Organizes and oversees Intramural games and assistants ', '20'
)INSERT INTO Roles VALUES ('Role13', 'AdministrativeManager', '14', 'Oversees all of the programs administrative needs', '25'
)INSERT INTO Roles VALUES ('Role14', 'FacilitiesManager', '13', 'Oversees all of the programs administrative needs', '15'
)INSERT INTO Roles VALUES ('Role15', 'FreeTrainLead', '10', 'Supervises equipment and facilities while in use', '10'
)INSERT INTO Roles VALUES ('Role16', 'ProgramAssistant', '9.5', 'Assists Program superiors in a variety of ways', '15'
)
 
INSERT INTO WorkDetails VALUES ('WD3', 'Em10', 'Role3', '900003', '16:00:00', '20:00:00'
)INSERT INTO WorkDetails VALUES ('WD4', 'Em11', 'Role1 ', '900005', '12:00:00', '16:00:00'
)INSERT INTO WorkDetails VALUES ('WD5', 'Em12', 'Role5', '900005', '16:00:00', '20:00:00'
)INSERT INTO WorkDetails VALUES ('WD6', 'Em13', 'Role1', '900008', '12:00:00', '16:00:00'
)INSERT INTO WorkDetails VALUES ('WD7', 'Em14', 'Role7', '900007', '16:00:00', '20:00:00'
)INSERT INTO WorkDetails VALUES ('WD8', 'Em15', 'Role8', '900008', '16:00:00', '20:00:00'
)INSERT INTO WorkDetails VALUES ('WD9', 'Em21', 'Role16', '900008', '08:00:00', '12:00:00'
)INSERT INTO WorkDetails VALUES ('WD10', 'Em24', 'Role16', '900002', '08:00:00', '12:00:00'
)INSERT INTO WorkDetails VALUES ('WD11', 'Em25', 'Role11', '900011', '12:00:00', '16:00:00'
)INSERT INTO WorkDetails VALUES ('WD12', 'Em1', 'Role16', '900013', '08:00:00', '12:00:00'
)INSERT INTO WorkDetails VALUES ('WD13', 'Em2', 'Role16', '900003', '08:00:00', '12:00:00'
)INSERT INTO WorkDetails VALUES ('WD14', 'Em3', 'Role6', '900006', '16:00:00', '20:00:00'
)INSERT INTO WorkDetails VALUES ('WD15', 'Em4', 'Role16', '900012', '08:00:00', '12:00:00'
)INSERT INTO WorkDetails VALUES ('WD16', 'Em7', 'Role15', '900012', '16:00:00', '20:00:00'
)INSERT INTO WorkDetails VALUES ('WD17', 'Em8', 'Role16', '900001', '08:00:00', '12:00:00'
)INSERT INTO WorkDetails VALUES ('WD18', 'Em9', 'Role16', '900010', '08:00:00', '12:00:00'
)INSERT INTO WorkDetails VALUES ('WD19', 'Em16', 'Role16', '900014', '08:00:00', '12:00:00'
)INSERT INTO WorkDetails VALUES ('WD20', 'Em17', 'Role4', '900004', '16:00:00', '20:00:00'
)INSERT INTO WorkDetails VALUES ('WD21', 'Em18', 'Role14 ', '900014', '12:00:00', '16:00:00'
)INSERT INTO WorkDetails VALUES ('WD22', 'Em19', 'Role13', '900013', '12:00:00', '16:00:00'
)INSERT INTO WorkDetails VALUES ('WD23', 'Em20', 'Role10', '900010', '16:00:00', '20:00:00'
)INSERT INTO WorkDetails VALUES ('WD24', 'Em22', 'Role16 ', '900004', '08:00:00', '12:00:00'
)INSERT INTO WorkDetails VALUES ('WD25', 'Em23', 'Role9', '900009', '16:00:00', '20:00:00'
)
 
INSERT INTO PersonalTrainer VALUES ('Em5', '20', '12', '900001'
)INSERT INTO PersonalTrainer VALUES ('Em6', '20', '13', '900002'
)INSERT INTO PersonalTrainer VALUES ('Em10', '20', '12', '900003'
)INSERT INTO PersonalTrainer VALUES ('Em11', '15', '14', '900004'
)INSERT INTO PersonalTrainer VALUES ('Em12', '10', '15', '900005'
)INSERT INTO PersonalTrainer VALUES ('Em13', '12', '12', '900006'
)INSERT INTO PersonalTrainer VALUES ('Em14', '15', '12.5', '900007'
)INSERT INTO PersonalTrainer VALUES ('Em15', '15', '13', '900008'
)INSERT INTO PersonalTrainer VALUES ('Em21', '15', '11', '900009'
)INSERT INTO PersonalTrainer VALUES ('Em24', '12', '10', '900010'
)INSERT INTO PersonalTrainer VALUES ('Em25', '20', '10.5', '900011'
)
 
INSERT INTO FitnessClubMembership VALUES ('Mem1', 'Joe', 'Greener', '839 1st Street', 'Knoxville', 'TN', '37916', '8659274187', 'M', '1999-05-12', '2023-03-12', 'Em5'
)INSERT INTO FitnessClubMembership VALUES ('Mem2', 'Bill', 'Quick', '5692 New Street', 'Maryville', 'TN', '37804', '8652046593', 'M', '2004-11-15', '2023-04-08', 'Em6'
)INSERT INTO FitnessClubMembership VALUES ('Mem3', 'John', 'Smith', '635 Broadway Ave', 'Sevierville', 'TN', '37764', '8651096104', 'M', '2002-05-23', '2023-03-18', 'Em10'
)INSERT INTO FitnessClubMembership VALUES ('Mem4', 'Sarah', 'Reader', '025 2nd Steet', 'Knoxville', 'TN', '37916', '8652047105', 'F', '1999-10-29', '2023-03-21', 'Em11'
)INSERT INTO FitnessClubMembership VALUES ('Mem5', 'Adam', 'Savage', '92442 Greenway Drive', 'Knoxville', 'TN', '37916', '8650612973', 'M', '2002-11-09', '2023-03-16', 'Em12'
)INSERT INTO FitnessClubMembership VALUES ('Mem6', 'Bella', 'Baton', '82 Hoover Lane', 'Seveirville', 'TN', '37764', '8567242043', 'F', '2000-01-25', '2023-04-04', 'Em13'
)INSERT INTO FitnessClubMembership VALUES ('Mem7', 'Zeke', 'Vanderbilt', '138 Kappa Court', 'Maryville', 'TN', '37804', '8567529926', 'M', '1998-08-16', '2023-03-18', 'Em14'
)INSERT INTO FitnessClubMembership VALUES ('Mem8', 'Emily', 'Danger', '0384 5th Street', 'Knoxville', 'TN', '37916', '8651250275', 'F', '2001-04-30', '2023-03-27', 'Em15'
)INSERT INTO FitnessClubMembership VALUES ('Mem9', 'Sue', 'Pollin', '24 Virginia Drive', 'Oak Ridge', 'TN', '37748', '8651090254', 'F', '2003-09-11', '2023-04-20', 'Em21'
)INSERT INTO FitnessClubMembership VALUES ('Mem10', 'Elton', 'John', '56 Kentucky Ave', 'Oak Ridge', 'TN', '37748', '8652759324', 'M', '2000-05-20', '2023-03-28', 'Em24'
)INSERT INTO FitnessClubMembership VALUES ('Mem11', 'Nichole', 'Granger', '35 ParkPlace Blv', 'Oak Ridge', 'TN', '37748', '8655628253', 'F', '1999-10-18', '2023-03-22', 'Em25'
)
 
INSERT INTO PersonalTrainerTimeSlots VALUES ('Em5', 'Mem1'
)INSERT INTO PersonalTrainerTimeSlots VALUES ('Em6', 'Mem2'
)INSERT INTO PersonalTrainerTimeSlots VALUES ('Em10', 'Mem3'
)INSERT INTO PersonalTrainerTimeSlots VALUES ('Em11', 'Mem4'
)INSERT INTO PersonalTrainerTimeSlots VALUES ('Em12', 'Mem5'
)INSERT INTO PersonalTrainerTimeSlots VALUES ('Em13', 'Mem6'
)INSERT INTO PersonalTrainerTimeSlots VALUES ('Em14', 'Mem7'
)INSERT INTO PersonalTrainerTimeSlots VALUES ('Em15', 'Mem8'
)INSERT INTO PersonalTrainerTimeSlots VALUES ('Em21', 'Mem9'
)INSERT INTO PersonalTrainerTimeSlots VALUES ('Em24', 'Mem10'
)INSERT INTO PersonalTrainerTimeSlots VALUES ('Em25', 'Mem11'
)
```

# Query and Report Code
Query 1

*Relevant information about an applicant for interview purposes (i.e., any information that would help make a hiring decision). There is no need to include contact information other than the applicant’s name and email.*
```
DROP VIEW InterviewInformation_Query2

CREATE VIEW InterviewInformation_Query2 AS
(SELECT ApCoAvCtCeTbl.ApplicantID, FirstName, LastName, Email, Major, FirstJobChoice, SecondJobChoice, DesiredHours, OptionalInterestEssay, GPA, 
		MorningStart, MorningEnd, NightStart, NightEnd, SummerStart, SummerEnd, Certification, ExpirationDate, PlaceOfEmployent, Position, SupervisorName, PhoneNumber
FROM (SELECT ApCoAvCtTbl.ApplicantID, ApCoAvCtTbl.CertificationID, FirstName, LastName, Email, Major, FirstJobChoice, SecondJobChoice, DesiredHours, OptionalInterestEssay, GPA, 
		MorningStart, MorningEnd, NightStart, NightEnd, SummerStart, SummerEnd, Certification, ExpirationDate
FROM (SELECT AppConAvailTbl.ApplicantID, CertificationID, FirstName, LastName, Email, Major, FirstJobChoice, SecondJobChoice, DesiredHours, OptionalInterestEssay, GPA, MorningStart, MorningEnd, NightStart, NightEnd, SummerStart, SummerEnd
		FROM (SELECT AppConTbl.ApplicantID, FirstName, LastName, Email, Major, FirstJobChoice, SecondJobChoice, DesiredHours, OptionalInterestEssay, GPA, MorningStart, MorningEnd, NightStart, NightEnd, SummerStart, SummerEnd
				FROM Availability RIGHT OUTER JOIN (SELECT Applicant.ApplicantID, FirstName, LastName, Email, Major, FirstJobChoice, SecondJobChoice, DesiredHours, OptionalInterestEssay, GPA
													FROM Applicant INNER JOIN Contact
													ON Applicant.ApplicantID = Contact.ApplicantID) AS AppConTbl
				ON Availability.ApplicantID = AppConTbl.ApplicantID) AS AppConAvailTbl
		LEFT OUTER JOIN CertificateType
		ON CertificateType.ApplicantID = AppConAvailTbl.ApplicantID) AS ApCoAvCtTbl
LEFT OUTER JOIN Certification
ON ApCoAvCtTbl.CertificationID = Certification.CertificationID) AS ApCoAvCtCeTbl
LEFT OUTER JOIN JobHistory
ON ApCoAvCtCeTbl.ApplicantID = JobHistory.ApplicantID)

SELECT *
FROM InterviewInformation_Query2
```
Query 2

*Pay information for each employee, including standard rate for the job role, starting pay rate, current pay
rate, date of last pay raise, and number of raises the employee has had while in that job role.*
```
DROP VIEW EmployeePayInformation_Query4

CREATE VIEW EmployeePayInformation_Query4 AS
(SELECT Employee.EmployeeID, Rate, StartingPay, (StartingPay + ISNULL(PayRaiseAmount,0)) AS CurrentPayRate, DateofRaise, COUNT(RaiseID) AS NumRaises
FROM Employee LEFT OUTER JOIN WorkDetails
ON Employee.EmployeeID = WorkDetails.EmployeeID
LEFT OUTER JOIN Raise
ON Raise.EmployeeID = Employee.EmployeeID
LEFT OUTER JOIN Roles
ON Roles.RoleID = WorkDetails.RoleID
GROUP BY Employee.EmployeeID, Rate, StartingPay, (StartingPay + ISNULL(PayRaiseAmount,0)), DateofRaise
ORDER BY Employee.EmployeeID DESC
OFFSET 0 ROWS)

SELECT *
FROM EmployeePayInformation_Query4
```
Query 3

 *A list of employees who do not have First Aid or CPR certificates 
 or whose First Aid and CPR certifications expired before their last pay raise evaluation.*
```
DROP VIEW NoCPRorFirstAid

CREATE VIEW NoCPRorFirstAid AS
SELECT Employee.EmployeeID, Employee.Position, Certification.Certification, ExpirationDate, DateofRaise
FROM Certification INNER JOIN CertificateType
	ON Certification.CertificationID = CertificateType.CertificationID
INNER JOIN Applicant
	ON CertificateType.ApplicantID = Applicant.ApplicantID
RIGHT OUTER JOIN Employee
	ON Employee.ApplicantID = Applicant.ApplicantID
LEFT OUTER JOIN Raise
	ON Employee.EmployeeID = Raise.EmployeeID
WHERE CertificateType.CertificationID IS NOT NULL
	AND (Certification.Certification NOT IN('FirstAid', 'CPR')
			OR ExpirationDate < DateofRaise);
```
Query 4 

 *Each trainers daily schedule, including information about who they trained, at what time, and the rate they charged.
 --which employees are trainers?
 --schedule, trainee, time of appointment, rate*
```
SELECT *
FROM employee 
WHERE Position like '%PersonalTrainer%'

SELECT PTEmployeeID, Hours, Rate
FROM PersonalTrainer

SELECT *
FROM PersonalTrainerTimeSlots

SELECT *
FROM FitnessClubMembership

CREATE VIEW PersonalTrainerInformation AS
(SELECT PersonalTrainer.PTEmployeeID, PersonalTrainer.Hours, PersonalTrainer.Rate, FitnessClubMembership.FirstName, FitnessClubMembership.LastName
FROM PersonalTrainer INNER JOIN PersonalTrainerTimeSlots
ON PersonalTrainer.PTEmployeeID = PersonalTrainerTimeSlots.PTEmployeeID
INNER JOIN FitnessClubMembership
ON PersonalTrainerTimeSlots.MemberID = FitnessClubMembership.MemberID
);
```
Query 5

*A list of employees by program, job role, and the average hours worked per week in that job role and
program.*
```
CREATE VIEW WorkDetailsandHours_Query6 AS (
SELECT WorkDetailsID, Employee.EmployeeID,WorkDetails.ProgramID,WorkDetails.RoleID, (SELECT
DATEDIFF(HOUR, WorkDetails.ShiftEnd, WorkDetails.ShiftTime)*-5) AS WeeklyHrsWorked
FROM Employee LEFT OUTER JOIN WorkDetails
ON Employee.EmployeeID = WorkDetails.EmployeeID
Group By WorkDetailsID, WorkDetails.ProgramID,WorkDetails.RoleID,Employee.EmployeeID,
WorkDetails.ShiftEnd, WorkDetails.ShiftTime)
ORDER BY Workdetails.ProgramID ASC;
```
# Report Samples
*Report 1: Employee Pay Information*

Purpose: To provide employee pay information including EmployeeID, Rate, Starting Pay, Current Pay, Date of Last Raise, and Number of Raises.

Recipient: HR managers as well as any manager or supervisor.

Sorted by: Sorted by EmployeeID in descending order

Ex: 

![RS11](https://github.com/CTorresKnox/Information-Management-Project/assets/144376690/0f6548d4-bb5f-4e9e-a16a-3a45a5902889)



*Report 2: Interview Information*

Purpose: To provide interviewers with useful information about the applicant including but not limited to Name, Email, Major, Desired Hours, 

Interest Survey, GPA, Certifications, Job History, etc.

Recipient: Interviewers

Sorted by: No sorting used

Ex: 

![RS12](https://github.com/CTorresKnox/Information-Management-Project/assets/144376690/bc91cc04-a755-47c4-9aa5-cb55d4d943e8)



*Report 3: No CPR or First Aid Report*

Purpose: Provide employee information for those who do not have CPR certification or First Aid certification or whose certification has expired.

Recipient: Supervisors and administrators

Sorted by: No sorting

Ex: 

![RS13](https://github.com/CTorresKnox/Information-Management-Project/assets/144376690/389a1db4-4d1f-4011-ae98-eadddbe07846)



*Report 4: Personal Trainer Information Report*

Purpose: To provide information about the personal trainers, their rates, hours, and trainees.

Recipient: Personal Trainer supervisors 

Sorted by: No sorting

Ex: 

![RS14](https://github.com/CTorresKnox/Information-Management-Project/assets/144376690/78e3c528-5c79-45da-a5bf-2609bdd55282)



*Report 5: Work Details and Hours Report*

Purpose: Provide information regarding an employee, a program they work in, their role in that program, as well as the weekly hours they worked for it.

Recipient: Supervisors of programs as well as employee managers

Sorted by: No sorting

Ex: 

![RS15](https://github.com/CTorresKnox/Information-Management-Project/assets/144376690/76b9dc87-6821-447c-98c3-ac450580adce)


# User Guide
In this section, we’ll showcase a user guide to help you better understand the front-end piece presented to you. Please follow the steps provided and refer to the information presented in the guide for future reference and training.

*Step 1. Locate the file in your file explorer.*

![UG1](https://github.com/CTorresKnox/Information-Management-Project/assets/144376690/ebff7182-868a-414f-bb20-3a3bf922a9d5)

Here the file is listed as “Group Project”. Your file name will be provided by your manager with limited capabilities.

*Step 2. Open the file and double click on the “Dashboard” underneath the Forms tab in All Access Objects. This will open the Dashboard and allow you to access the reports needed for your assignments and administrative tasks.*

![UG2](https://github.com/CTorresKnox/Information-Management-Project/assets/144376690/fa6f3a42-6443-4423-8947-93477ba1d47e)

![UG3](https://github.com/CTorresKnox/Information-Management-Project/assets/144376690/37c60279-860f-47f4-b2a9-c4dc9258ef40)



*Step 3. Familiarize yourself with the buttons and their functionality.* 

![UG4](https://github.com/CTorresKnox/Information-Management-Project/assets/144376690/f654c561-053f-4b2f-8cb1-b30372895f54)


On the left is the name of the report you may be interested in. Here is a brief description of each report:
-Employee Pay Information Report: Pay information for each employee including standard rate for job role, starting pay, pay raises, current pay rate, date of last pay raise, and the number of raises received while on the job.
- Interview Information Report: Relevant information for interview purposes. Includes information such as previous positions held, name, certifications, their expirations dates, job choices, etc.
-No CPR or First Aid Report: This report lists all employees who do not have a valid CPR and First Aid certification.
- Personal Trainer Information Report: Daily schedule of Personal Trainer with trainee, time, and rate charged.
- Work Details and Hours Report: A list of employees by program, job role, and average hours worked per week.

On the right is a list of buttons that perform a variety of administrative tasks. Please also take the time to familiarize yourself with them. Below is a list of the button names and their functionality:
- Preview Report: Allows you to open the report to preview and inspect.
- Print Report: Allows you to send the report to a printer for printing.
- Mail Report: Allows you to email the report in a variety of formats including but not limited to XML, PDF, and MS Excel.
- Save Report: Allows you to save the report to your computer in a variety of formats including but not limited to XML, PDF, and MS Excel.
- Record Lookup: Allows you to lookup any records within the database the reports were formulated from. 
NOTE: This requires you to input a known identifier key for the report. Example below:

![UG5](https://github.com/CTorresKnox/Information-Management-Project/assets/144376690/3bb34fd6-be52-4574-8450-594b3b0323d3)

This is an example from the Personal Trainer Information Report. Other reports may ask for different identifiers such as WorkDetailsID.


*Step 4. Sign in to view reports and use the Dashboard.*

As you may have noticed when selecting the buttons for the Dashboard, you were prompted to sign into the SQL Server. Please log in with the credentials given to you by your database administrator. If you forget your password, your administrator can assist you in resetting it. Please write it down in a safe, secure place or, preferably, memorize it. 

![UG6](https://github.com/CTorresKnox/Information-Management-Project/assets/144376690/2ae79f59-7842-42a4-a54c-9e3734787bf3)


Note:
Please do not attempt to alter or change any of the reports’ formats or source data. Permission to do so should not be granted to anyone besides the administrator and a few of their assistants. If you are having trouble with a report, please contact your administrator. 

# Appendix: Updates and Restatement of Phase I

*CONCEPTUAL DATA MODEL (ERD)*

Updates:
- The relationship between Employee and Personal Trainer was made into a disjointed relationship to more accurately reflect the unique relationship between Personal Trainers and the services they offer to members. 
- ShiftTime and ShiftEnd were added to the WorkDetails table to provide shift times in order to answer Query 6.
- The relationship between Employee and Alumni was deleted to prevent complications. Instead, EmployeeID’s should be retired and converted into AlumniID to simplify data.

![ERD Update](https://github.com/CTorresKnox/Information-Management-Project/assets/144376690/85197c8b-0faf-49ea-adc2-320f35898dca)


*LOGICAL DATA MODEL*

Updates:
- Logical model was updated to be consistent with ERD
- Added ShiftTime and ShiftEnd to the WorkDetails table

![LDMU1](https://github.com/CTorresKnox/Information-Management-Project/assets/144376690/5fc0b5bc-fbb1-401f-ac36-56b40a5eacd5)
![LDMU2](https://github.com/CTorresKnox/Information-Management-Project/assets/144376690/4797ddc5-b465-4e0e-8387-68b8ba374e46)


*DATA DICTIONARY*

Updates:
- Data Dictionary was completed and updated to accurately represent the data within the database.

![DDU1](https://github.com/CTorresKnox/Information-Management-Project/assets/144376690/757b26ff-e8e4-4a9f-9d60-e8f395e54e66)
![DDU2](https://github.com/CTorresKnox/Information-Management-Project/assets/144376690/b66b7ce2-a428-4cd4-b013-ea3dd1ceecba)
![DDU3](https://github.com/CTorresKnox/Information-Management-Project/assets/144376690/2b7dd159-55dd-4faa-af48-9189819be6b5)
![DDU4](https://github.com/CTorresKnox/Information-Management-Project/assets/144376690/ee3ba8c3-39e8-43f9-9680-2cd120aa1081)
![DDU5](https://github.com/CTorresKnox/Information-Management-Project/assets/144376690/b2211347-91df-4fc8-b566-f4ca198b20be)
![DDU6](https://github.com/CTorresKnox/Information-Management-Project/assets/144376690/0baaa4cf-313f-41c3-b234-69eccc93ec1e)
![DDU7](https://github.com/CTorresKnox/Information-Management-Project/assets/144376690/e3145a90-0186-4c1d-8328-4536e1d176b7)
