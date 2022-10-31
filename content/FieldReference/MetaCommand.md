## MetaCommand
| Field Label | Field Name | Field Type | Description |  
| ---- | ---- | ---- | ---- |  
| Command Id | CommandId | Guid<br/>  [Key]<br/>  [Required]<br/>  [ReadOnly] |  |  
| Entity Id | EntityId | Guid?<br/>  [ForeignKey MetaEntity] |  |  
| App Id | AppId | Guid?<br/>  [ForeignKey MetaApp] |  |  
| Command Name | CommandName | String<br/>  [Required]<br/>  [Descriptor] | The name of the Command as it appears on pages and forms |  
| Command API Name | CommandApiName | String<br/>  [Required]<br/>  [TenantUnique]<br/>  [MinLen: 2]<br/>  [MaxLen: 50]<br/>  [Regex: ^[a-zA-Z_][a-zA-Z0-9_.-]*$]<br/>  [ReadOnlyAfterInsert] | A unique and url-safe API name for this command. It is used to refer to the command in processes and in the external API. The name is derived from the command name by default and can only be edited when creating a new command.  |  
| Exection Type | ExectionType | ExecutionType | Set what happens when the command is selected. Options: Run C# Code, Navigate to a Url, or run a JavaScript snippet. <br/>  Allowable Values: <br/>  <br/>  **CSharp**<br/>  **Url**<br/>  **JavaScript** |  
| Command Description | CommandDescription | String<br/>  [Template: MultilineText] |  |  
| Help Page | HelpPage | String<br/>  [Template: Url] |  |  
| Custom | IsCustom | Bool |  |  
| Organization Id | OrganizationId | Guid?<br/>  [ForeignKey Organization] |  |  
| Created Date | CreatedDate | DateTime |  |  
| Created By | CreatedBy | String |  |  
| Modified Date | ModifiedDate | DateTime |  |  
| Modified By | ModifiedBy | String |  |  
| Row Version | RowVersion | Int |  |  
