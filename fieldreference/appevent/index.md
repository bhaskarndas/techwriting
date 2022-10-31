# AppEvent


## AppEvent
View the App Event history  

| Field Label | Field Name | Field Type | Description |  
| ---- | ---- | ---- | ---- |  
| Event Id | EventId | Guid<br/>  [Key]<br/>  [Required]<br/>  [ReadOnly] |  |  
| Topic | EventTopic | String<br/>  [Descriptor]<br/>  [MaxLen: 40] | A Topic is used to group AppEvent messages of the same type. The Topic for AppEvents raised by changes to entities, eg Contacts, will always be the same as the entity name. |  
| Subtopic | SubTopic | String | The SubTopic is used to further specify the type of the AppEvent message. For AppEvents raised by changes to entity records, the SubTopic will typically be 'Added', 'Updated', or 'Deleted'. |  
| Event Summary | EventSummary | String | A concise, one line summary of the app event. |  
| Payload | EventPayload | String | The Payload typically contains a JSON object with the AppEvent message. For AppEvents raised by entity changes, the JSON object contains the differences between the old and new values of the model/schema used to edit the entity. |  
| Event Description | EventDescription | String | A description users will understand. Typically a translation of the JSON payload into human readable text. |  
| User Id | UserId | String<br/>  [ForeignKey ApplicationUser] | The id of the user associated with this app event record if applicable (often, the person who caused a state change). |  
| Schema Name | SchemaName | String<br/>  [MaxLen: 60] | Schema name or model name if applicable, eg ClientEditModel. |  
| Unique Id | UniqueId | String<br/>  [MaxLen: 36] | Primary key / unique id value as a string. Will contain at max a Guid to string = 36 chars. |  
| Unique Id Type | UniqueIdType | String | Property type of the UniqueId value, eg Int, Guid or String. |  
| Date | EventDate | DateTime | Date and time the event took place. |  
| User | UserName | String | Full name of the user responsible for the app event if applicable. |  
| Organization Id | OrganizationId | Guid?<br/>  [ForeignKey Organization] |  |  

