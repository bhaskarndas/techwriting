# 


## MetaForm
| Field Label | Field Name | Field Type | Description |  
| ---- | ---- | ---- | ---- |  
| Form Id | FormId | Guid<br/>  [Key]<br/>  [Required]<br/>  [ReadOnly] |  |  
| Entity Id | EntityId | Guid<br/>  [ForeignKey MetaEntity]<br/>  [Required]<br/>  [ReadOnlyAfterInsert] |  |  
| Name | FormName | String<br/>  [Required]<br/>  [Descriptor] | The name of the Form as it appears on pages and forms |  
| Entity Name | EntityName | String<br/>  [ReadOnly] | The name of the entity linked to this form. The list of potential fields are derived from this entity and those linked toit with lookup relationships.  |  
| Form API Name | FormApiName | String<br/>  [Required]<br/>  [TenantUnique]<br/>  [MinLen: 2]<br/>  [MaxLen: 50]<br/>  [Regex: ^[a-zA-Z_][a-zA-Z0-9_.-]*$]<br/>  [ReadOnlyAfterInsert] | A unique and url-safe API name for this form. It is used to refer to the form in processes and in the external API. The name is derived from the form name by default and can only be edited when creating a new form.  |  
| Form Description | FormDescription | String |  |  
| Help Text | HelpText | String | Use this space to provide more detailed guidance to your users.  |  
| Form Help Text Position | FormHelpTextPosition | FormHelpTextPosition | Determines where and how the text entered in the Help Text field will be displayed. See the option descriptions in the dropdown. <br/>  Allowable Values: <br/>  <br/>  **IconLink**: Displays a question mark icon in the form header for forms where help text is available. When a user clicks on the link, the help text appears in a popup window. <br/>  **PanelTop**: The help text will be displayed in a shaded box above the form fields. <br/>  **PanelBottom**: The help text will be displayed in a shaded box below the form fields. <br/>  **PanelRight**: The help text will be displayed in a shaded box to the right of the form fields. This means that the space available for the form fields will be reduced potentially causing the layout to become crowded. In this case, youcould consider moving to a 1 column or narrower layout.  |  
| Form Layout | FormLayout | String |  |  
| Custom | IsCustom | Bool |  |  
| Organization Id | OrganizationId | Guid?<br/>  [ForeignKey Organization] |  |  
| Created Date | CreatedDate | DateTime |  |  
| Created By | CreatedBy | String |  |  
| Modified Date | ModifiedDate | DateTime |  |  
| Modified By | ModifiedBy | String |  |  
| Row Version | RowVersion | Int |  |  

