# Staff


## Staff
| Field Label | Field Name | Field Type | Description |  
| ---- | ---- | ---- | ---- |  
| Staff Id | StaffId | Guid<br/>  [Key]<br/>  [Required]<br/>  [ReadOnly] |  |  
| User Id | UserId | String<br/>  [ForeignKey ApplicationUser] |  |  
| User Profile | ProfileId | Guid<br/>  [ForeignKey UserProfile]<br/>  [Required] |  |  
| First Name | FirstName | String |  |  
| Last Name | LastName | String |  |  
| Staff Name | StaffName | String<br/>  [Descriptor] |  |  
| Notes | StaffNotes | String |  |  
| Image | MediaId | Guid?<br/>  [ForeignKey Media]<br/>  [Template: Image] |  |  
| LinkedIn | LinkedInPage | String<br/>  [Template: Url] |  |  
| Facebook | FacebookPage | String<br/>  [Template: Url] |  |  
| Telephone | Telephone1 | String<br/>  [Template: Telephone] |  |  
| Secondary Telephone | Telephone2 | String<br/>  [Template: Telephone] |  |  
| Email | Email1 | String<br/>  [Template: Email]<br/>  [ReadOnlyAfterInsert] | This email address is used to log into the system. Use the Change Login Email link below to modify the this email address. |  
| Secondary Email | Email2 | String<br/>  [Template: Email] |  |  
| Archived | IsArchived | Bool | Use the Archive checkbox to hide inactive records without deleting them. Archiving will prevent them from being selected in dropdown lists or appearing on list pages. Usage in existing records will not be affected. Archived records are stored indefinitely and be viewed in the archived items app group where they can be unarchived if needed again.  |  
| Created Date | CreatedDate | DateTime |  |  
| Created By | CreatedBy | String |  |  
| Modified Date | ModifiedDate | DateTime |  |  
| Modified By | ModifiedBy | String |  |  
| Row Version | RowVersion | Int |  |  

