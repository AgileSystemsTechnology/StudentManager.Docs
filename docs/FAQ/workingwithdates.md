## **Dates in Student Manager(SM)**

### **Date Relationships**
- Intake Enrolment dates can affect groups which are displayed
- Enrolment dates can create edu-dex errors
- Application Open and Close date can affect whether an Intake is displayed on the New Applications page
- Registration Open and Close dates can affect when registrations can occur
- Registration Group Scope dates will determine which groups are displayed
- Assessment dates have a relationship with Group Start and End dates
- Assessment Attempts are related to each other

###**Enrolment Dates**
- The enrolment date is when the learner started studying the qualification, so remember this being the learners first day on campus or the first day of lectures/learning
- So if this is their first day of learning or being on-site, it would be reasonable to assume that the group they are enrolled it can't start before they we enrolled
	- So for an intake year of a given student, all related module groups should start on or after the enrolment date
	- e.g. if the enrolment date is 02/07/2013, the group start dates for their first year of study should be 02/07/2013 or later
- This is the same logic for **edu-dex**, a learner can only be enrolled for a qualification which started before their enrolment date 
	- i.e. if their enrolment date is 02/07/2013 and the accreditation start date for the qualification is 20/01/2015, there will be an edu-dex error 

###**Application Open and Close Dates**
- The application open and close dates are there as a rule to say when someone can apply to gain entry into an intake for a qualification
	- so for this reason, if my application open and close  dates are 02/07/2012 to 31/01/2013 on the 1st of February the intake will not be selectable for applicants, becuase applications are closed

###**Registration Open and Close Dates**
- The registration open and close dates determine when a learner can be registered in a qualification
	- e.g. If the registration open and close dates are 31/01/2013 - 28/02/2013 and a staff attempt to register a learner on 30/01/2013 or 01/03/2013 the system will now allow registration to occur  

###**Registration Group Scope Dates**	
- The registration scope group dates determine which group can be selected during registration
	- e.g. 	If the registration groups scope date are set to start on 01/01/2013 and set to end on 30/06/2013 and I'm at an institution which uses semesters, when attempting to register student modules, groups with the dates 01/07/2013 - 31/12/2013 will not display on the registrations page


###**Module Groups Dates**
- Module group start and end dates are important because everything which a learner does is in the context of the group
	- We've already covered that group start dates should match or follow after enrolment dates for learners in their first year of study, for the groups to be accessible
	- All assessments must fall within the start and end date of the group to be accessible
	- All calendar events for a group must also fall within the start and end date of that group to be accessible

###**Module Group: Student Joined and Left Dates**
- If a learner is registered into a module's group before the group start date or on the day that the group starts, they will get a joined and left date which matches the groups start and end date
- If a learner is registered into a module's group after the group start date, the date that they have joined the group will be the same as the registration date and the date left will be the same as the group end date
	- The reason for this is that if the student joins the group late any assessments and events which had occurred prior to them entering the group, they will automatically be excluded from it because they were not available when the event occurred

###**Assessment Dates**
- All assessments start and end dates must fall within the group start and end dates to be accessible
	- It is ideal to have realistic start and end dates for assessments when they are created, but it understood that this is not always the case
	- Please bear in mind that assessment dates will appear on the learner and institutions calendar, so having an assessment for the whole year could be confusing to read on groups calendar


###**Assessment Attempts**
- When an assessment is added, the date which is added is related to the first assessment attempt for that assessment
- A many subsequent attempts can be created
	- Please note that each attempt for an assessment should have different start and end dates and times if they are exactly the same, the system will not know how to best calculate the results for that learner, as results calculations are related to the "Grade Symbol Range" in the System Settings
- Assessment attempt start and end dates are also linked to online assessments (these can also link to e-Learning)
	- If you have an assessment attempt start and end date which is the entire year and you then have it as online assessment, this means that learners can start this assessment anytime in the year
	- If you have e-Learning at that must be completed before the assessment attempt can be accessed, ensure that the dates are laid out appropriately to not have any clashes
