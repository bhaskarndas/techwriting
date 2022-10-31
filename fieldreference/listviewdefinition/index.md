# 


## ListViewDefinition
Define and manage list views to see a specific set of Clients, Leads or other entity records.

| Field Label | Field Name | Field Type | Description |  
| ---- | ---- | ---- | ---- |  
| List View Definition Id | ListViewDefinitionId | Guid<br/>  [Key]<br/>  [Required]<br/>  [ReadOnly] |  |  
| Entity Id | EntityId | Guid?<br/>  [ForeignKey MetaEntity] |  |  
| Parent List View Id | ParentListViewId | Guid? |  |  
| Organization Id | OrganizationId | Guid?<br/>  [ForeignKey Organization] |  |  
| User Id | UserId | String<br/>  [ForeignKey ApplicationUser] |  |  
| List Type | ListType | ListType | The list type determines whether the list as presented in tabular format or as a form per row. <br/>  Allowable Values: <br/>  <br/>  **Table**<br/>  **Form** |  
| Is Built In | IsBuiltIn | Bool |  |  
| Personal | Personal | Bool |  |  
| List Model | ListModel | String<br/>  [Descriptor]<br/>  [MaxLen: 100] |  |  
| View Name | ViewName | String |  |  
| Is Default | IsDefault | Bool |  |  
| Use Default Column Layout | UseDefaultColumnLayout | Bool |  |  
| Filter Expression | FilterExpression | FilterExpression |  |  
| Extension Data | ExtensionData | JObject |  |  

