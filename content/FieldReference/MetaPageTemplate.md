
## MetaPageTemplate
Configure templates used when creating new pages  

| Field Label | Field Name | Field Type | Description |  
| ---- | ---- | ---- | ---- |  
| Template Id | TemplateId | Guid<br/>  [Key]<br/>  [Required]<br/>  [ReadOnly] |  |  
| Name | TemplateName | String<br/>  [Required]<br/>  [Descriptor] | The name of the Template as it appears on pages and forms |  
| Page Template API Name | TemplateApiName | String<br/>  [Required]<br/>  [TenantUnique]<br/>  [MinLen: 2]<br/>  [MaxLen: 50]<br/>  [Regex: ^[a-zA-Z_][a-zA-Z0-9_.-]*$]<br/>  [ReadOnlyAfterInsert] | A unique and url-safe API name for this page template. It is used to refer to the template in processes and in the external API. The name is derived from the template label by default and can only be edited when creating a new template.  |  
| Template Description | TemplateDescription | String |  |  
| Template Layout | TemplateLayout | ModelElement |  |  
| Custom | IsCustom | Bool |  |  
| Organization Id | OrganizationId | Guid?<br/>  [ForeignKey Organization] |  |  
| Created Date | CreatedDate | DateTime |  |  
| Created By | CreatedBy | String |  |  
| Modified Date | ModifiedDate | DateTime |  |  
| Modified By | ModifiedBy | String |  |  
| Row Version | RowVersion | Int |  |  
