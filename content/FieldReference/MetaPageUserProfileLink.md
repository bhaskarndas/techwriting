## MetaPageUserProfileLink
| Field Label | Field Name | Field Type | Description |  
| ---- | ---- | ---- | ---- |  
| Link Id | LinkId | Int<br/>  [Key]<br/>  [Required]<br/>  [ReadOnly] |  |  
| Page Id | PageId | Guid<br/>  [ForeignKey MetaPage]<br/>  [Required] |  |  
| Profile Id | ProfileId | Guid<br/>  [ForeignKey UserProfile]<br/>  [Required] |  |  
| Default | IsDefaultForProfile | Bool | When multiple pages have been linked to the same User Profile, then this field can be used to indicate which page should appear by default. If no default has been set, then the first page will appear based on its name in alphabetical order.  |  
| Custom | IsCustom | Bool |  |  
| Organization Id | OrganizationId | Guid?<br/>  [ForeignKey Organization] |  |  
| Created Date | CreatedDate | DateTime |  |  
| Created By | CreatedBy | String<br/>  [Descriptor] |  |  
| Modified Date | ModifiedDate | DateTime |  |  
| Modified By | ModifiedBy | String |  |  
| Row Version | RowVersion | Int |  |  
