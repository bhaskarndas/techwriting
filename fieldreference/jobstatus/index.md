# 

﻿## JobStatus
| Field Label | Field Name | Field Type | Description |  
| ---- | ---- | ---- | ---- |  
| Job Status Id | JobStatusId | Guid<br/>  [Key]<br/>  [Required]<br/>  [ReadOnly] |  |  
| Job Name | JobName | String<br/>  [Descriptor] |  |  
| Job Messages | JobMessages | String |  |  
| Job State | JobState | JobState | <br/>  Allowable Values: <br/>  <br/>  **NotStarted**<br/>  **Running**<br/>  **CompletedSuccessfully**<br/>  **CompletedWithError**<br/>  **CancellationRequested**<br/>  **CancelledByUser** |  
| Percent Complete | PercentComplete | Int? |  |  
| Sub Job Description | SubJobDescription | String |  |  
| Run Summary | RunSummary | String |  |  
| Start Time | StartTime | DateTime? |  |  
| End Time | EndTime | DateTime? |  |  
| Elapsed Time | ElapsedTime | TimeSpan? |  |  
| Hangfire Job Id | HangfireJobId | String |  |  
| User Id | UserId | String |  |  
| Developer Info | DeveloperInfo | String |  |  
| Organization Id | OrganizationId | Guid? |  |  

