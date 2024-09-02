# LLM-IR-Dataset

This repository contains a synthetic Incident Response Process Activities and Communication data Log dataset generated using an LLM. An exisiting anonymised publicly available Incident managament Process Log dataset was augmented to include additional fields and textual data.

## Dataset Description

The dataset includes detailed records of various Incident Response cases, corresponding actions, processes, and communication. Each record represents an individual incident and contains information relevant to the response actions and resolution of security incidents.

### Field Description

number: incident identifier; <br>
incident state: eight levels controlling the incident management process transitions from opening until closing the case;
active: boolean attribute that shows whether the record is active or closed/canceled;
reassignment_count: number of times the incident has the group or the support analysts changed;
reopen_count: number of times the incident resolution was rejected by the caller;
sys_mod_count: number of incident updates until that moment;
made_sla: boolean attribute that shows whether the incident exceeded the target SLA;
caller_id: identifier of the user affected;
opened_by: identifier of the user who reported the incident;
opened_at: incident user opening date and time;
sys_created_by: identifier of the user who registered the incident;
sys_created_at: incident system creation date and time;
sys_updated_by: identifier of the user who updated the incident and generated the current log record;
sys_updated_at: incident system update date and time;
contact_type: categorical attribute that shows by what means the incident was reported;
location: identifier of the location of the place affected;
category: first-level description of the affected service;
subcategory: second-level description of the affected service (related to the first level description, i.e., to category);
u_symptom: description of the user perception about service availability;
impact: description of the impact caused by the incident (values: 1â€“High; 2â€“Medium; 3â€“Low);
urgency: description of the urgency informed by the user for the incident resolution (values: 1â€“High; 2â€“Medium; 3â€“Low);
priority: calculated by the system based on 'impact' and 'urgency';
assigned_to: identifier of the user in charge of the incident;
knowledge: boolean attribute that shows whether a knowledge base document was used to resolve the incident;
u_priority_confirmation: boolean attribute that shows whether the priority field has been double-checked;
notify: categorical attribute that shows whether notifications were generated for the incident;
rfc: (request for change) identifier of the change request associated with the incident;
Case ID: Unique identifier for each case;
Case Title: Title or brief description of the case;
Creation Date: Date when the case was created;
Description: Detailed description of the case;
Case Task (Array): [Case Tasks Title: Title or brief description of the task within the case, Case Task Start Date: Start date of the task, Case Task Assignee: User assigned to the task, Case Task Status: Current status of the task, Case Task Duration: Duration of the task, Case Attribute Data: Additional attributes or metadata associated with the case];
Analyst Investigative Activities / Observables (Array): [Analysis Type: Specifies the type of analysis conducted, Analysis ID: A unique identifier for this specific analysis, Timestamp: The date and time when the analysis was performed, Data Value: The specific data being analyzed or a key piece of information about the analysis, Details: Additional information or results from the analysis, Status: The final outcome or status of the analysis];
Ticketing System Chat Log: Chat Data fron ticketing system
Ticketing system Chat response Data  - Keywords: Keywords extracted from chat responses related to investigation and diagnosis.
Chat Response Overall Sentiment Determination: (Positive Sentiment: Most chat interactions reflect confidence, effective communication, and positive language) or (Negative Sentiment: Most interactions reflect frustration, challenges, or negative emotions) or (Neutral Sentiment: The conversation is balanced, with no strong emotional tone either way);
Event ID: Unique identifier for each event;
Distribution: How the information within an event or attribute is shared with other organizations or participants in the MISP community;
Event Information (Description): Detailed description of the event;
Threat Level: Assessed threat level of the event;
Event Attributes: Various attributes related to the event;
close_code: identifier of the resolution of the incident;
resolved_by: identifier of the user who resolved the incident;
resolved_at: incident user resolution date and time (dependent variable);
closed_at: incident user close date and time (dependent variable);
