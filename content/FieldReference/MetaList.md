## MetaList
Configure how lists of entities are displayed  
  
| Field Label | Field Name | Field Type | Description |  
| ---- | ---- | ---- | ---- |  
| List Id | ListId | Guid<br/>  [Key]<br/>  [Required]<br/>  [ReadOnly] |  |  
| Entity Id | EntityId | Guid<br/>  [ForeignKey MetaEntity]<br/>  [Required] |  |  
| List API Name | ListApiName | String<br/>  [Required]<br/>  [TenantUnique]<br/>  [MinLen: 2]<br/>  [MaxLen: 50]<br/>  [Regex: ^[a-zA-Z_][a-zA-Z0-9_.-]*$]<br/>  [ReadOnlyAfterInsert] | A unique and url-safe API name for this list. It is used to refer to the list in processes and in the external API. The name is derived from the list label by default and can only be edited when creating a new list.  |  
| List Name | ListName | String<br/>  [Required]<br/>  [Descriptor] | The name of the list as it appears in the List View dropdown menu and elsewhere .  |  
| List Description | ListDescription | String<br/>  [Template: MultilineText] |  |  
| List Type | ListType | ListType | The list type determines whether the list as presented in tabular format or as a form per row. <br/>  Allowable Values: <br/>  <br/>  **Table**<br/>  **Form** |  
| Form Id | FormId | Guid?<br/>  [ForeignKey MetaForm] |  |  
| Custom | IsCustom | Bool |  |  
| Organization Id | OrganizationId | Guid?<br/>  [ForeignKey Organization] |  |  
| Created Date | CreatedDate | DateTime |  |  
| Created By | CreatedBy | String |  |  
| Modified Date | ModifiedDate | DateTime |  |  
| Modified By | ModifiedBy | String |  |  
| Row Version | RowVersion | Int |  |  
