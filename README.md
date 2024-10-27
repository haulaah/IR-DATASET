# LLM-IR-Dataset

This repository contains a synthetic Incident Response Process Activities and Communication data Log dataset generated using an LLM.

## Dataset Description

The dataset includes detailed records of different unique Incident Response cases, corresponding actions, processes, and communication data.

### Field Description

-**number**: incident identifier; <br>
-**incident state**: eight levels controlling the incident management process transitions from opening until closing the case;<br>
-**active**: boolean attribute that shows whether the record is active or closed/canceled;<br>
-**reassignment_count**: number of times the incident has had the group or the support analysts changed;<br>
-**reopen_count**: number of times the incident resolution was rejected by the caller;<br>
-**sys_mod_count**: number of incident updates until that moment;<br>
-**made_sla**: boolean attribute that shows whether the incident exceeded the target SLA;<br>
-**caller_id**: identifier of the user affected;<br>
-**opened_by**: identifier of the user who reported the incident;<br>
-**opened_at**: incident user opening date and time;<br>
-**sys_created_by**: identifier of the user who registered the incident;<br>
-**sys_created_at**: incident system creation date and time;<br>
-**sys_updated_by**: identifier of the user who updated the incident and generated the current log record;<br>
-**sys_updated_at**: incident system update date and time;<br>
-**contact_type**: categorical attribute that shows by what means the incident was reported;<br>
-**category**: first-level description of the affected service;<br>
-**subcategory**: second-level description of the affected service (related to the first level description, i.e., to category);<br>
-**u_symptom**: description of the user perception about service availability;<br>
-**impact**: description of the impact caused by the incident (values: 1-High; 2-Medium; 3-Low);<br>
-**urgency**: description of the urgency informed by the user for the incident resolution (values: 1-High; 2-Medium; 3-Low);<br>
-**priority**: calculated by the system based on 'impact' and 'urgency';<br>
-**assigned_to**: identifier of the user in charge of the incident;<br>
-**knowledge**: boolean attribute that shows whether a knowledge base document (Case Template / IR Playbook) was used to resolve the incident;<br>
-**notify**: categorical attribute that shows whether notifications were generated for the incident;<br>
-**rfc**: (request for change) identifier of the change request associated with the incident;<br>
-**case ID**: Unique identifier for each case;<br>
-**case Title**: Title or brief description of the case;<br>
-**creation Date**: Date when the case was created;<br>
-**Description**: Detailed description of the case;<br>
-**case Task (Array)**: [Case Tasks Title: Title or brief description of the task within the case, Case Task Start Date: Start date of the task, Case Task Assignee: User assigned to the task, Case Task Status: Current status of the task, Case Task Duration: Duration of the task, Case Attribute Data: Additional attributes or metadata associated with the case];<br>
-**Observables Analysis (Array)**: [Analysis Type: Specifies the type of analysis conducted, Analysis ID: A unique identifier for this specific analysis, Timestamp: The date and time when the analysis was performed, Data Value: The specific data being analyzed or a key piece of information about the analysis, Details: Additional information or results from the analysis, Status: The final outcome or status of the analysis];<br>
-**ticketing System Chat Log**: Chat data from the ticketing system;<br>
-**ticketing System Chat Data Keywords**: Keywords extracted from chat responses related to investigation and diagnosis;<br>
-**chat Response Overall Sentiment Determination**: (Positive Sentiment: Most chat interactions reflect confidence, effective communication, and positive language) or (Negative Sentiment: Most interactions reflect frustration, challenges, or negative emotions) or (Neutral Sentiment: The conversation is balanced, with no strong emotional tone either way);<br>
-**event ID**: Unique identifier for each event;<br>
-**distribution**: How the information within an event or attribute is shared with other organizations or participants in the MISP community;<br>
-**event Information (Description)**: Detailed description of the event;<br>
-**threat Level**: Assessed threat level of the event;<br>
-**event Attributes**: Various attributes related to the event;<br>
-**close_code**: identifier of the resolution of the incident;<br>
-**resolved_by**: identifier of the user who resolved the incident;<br>
-**resolved_at**: incident user resolution date and time (dependent variable);<br>
-**closed_at**: incident user close date and time (dependent variable);<br>


## Paper Publication IEEE
