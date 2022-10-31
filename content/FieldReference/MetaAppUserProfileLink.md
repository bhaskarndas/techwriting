## MetaAppUserProfileLink
| Field Label | Field Name | Field Type | Description |  
| ---- | ---- | ---- | ---- |  
| Link Id | LinkId | Guid<br/>  [Key]<br/>  [Required]<br/>  [ReadOnly] |  |  
| App Id | AppId | Guid<br/>  [ForeignKey MetaApp]<br/>  [Required] |  |  
| Profile Id | ProfileId | Guid<br/>  [ForeignKey UserProfile]<br/>  [Required] |  |  
| Visible | IsVisible | Bool | Determines whether an App is visible for users with this profile. Note: This checkbox does not grant access to the app's entities or fields. Access security for these items must be set in User Profiles.  |  
| Default | IsDefault | Bool | The Default checkbox specifies which app should be started automatically when users with this profile log in.  |  
| Custom | IsCustom | Bool |  |  
| Organization Id | OrganizationId | Guid?<br/>  [ForeignKey Organization] |  |  
| Created Date | CreatedDate | DateTime |  |  
| Created By | CreatedBy | String<br/>  [Descriptor] |  |  
| Modified Date | ModifiedDate | DateTime |  |  
| Modified By | ModifiedBy | String |  |  
| Row Version | RowVersion | Int |  |  
