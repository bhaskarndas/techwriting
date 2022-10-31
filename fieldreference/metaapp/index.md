# 

﻿## MetaApp
Configure applications, related entities, pages and profiles 
  
| Field Label | Field Name | Field Type | Description |  
| ---- | ---- | ---- | ---- |  
| App Id | AppId | Guid<br/>  [Key]<br/>  [Required]<br/>  [ReadOnly] |  |  
| App Name | AppName | String<br/>  [Required]<br/>  [Descriptor] | The name of the App as it appears on pages and forms |  
| App API Name | AppApiName | String<br/>  [Required]<br/>  [TenantUnique]<br/>  [MinLen: 2]<br/>  [MaxLen: 50]<br/>  [Regex: ^[a-zA-Z_][a-zA-Z0-9_.-]*$]<br/>  [ReadOnlyAfterInsert] | A unique and url-safe API name for this app. It is used to refer to the app and in internal processes and in the external API.  |  
| App Description | AppDescription | String |  |  
| Icon | AppIconName | String | Specify the name of a FontAwesome icon to display when the entitity appears on pages and forms. For example, 'fal fa-cogs' will display a large cog and two smaller ones to the right. See the entire list at: https://fontawesome.com/icons?d=gallery&s=light |  
| Color | AppIconColor | String<br/>  [MaxLen: 7]<br/>  [Regex: #([A-Fa-f0-9]{6})] | Specify the web color used to provide the icon background when the entity icon is displayed. The web color must be specified in web hex format and must begin with a leading # sign and contain 6 additional characters consisting of the letters A-F and the numbers 0-9. For example, the code '#00204F' specifies the color we use for the main menu background. You can select a color from the color picker or enter one directly.  |  
| Help Text | HelpText | String | Use this space to provide more detailed guidance to your users. Text can be formatted using Markdown which is an easy-to-read, easy-to-write syntax for formatting plain text.syntax. Markdown can also include hyperlinks to access additional information. The help text position and display style are governed by the Help Text Position dropdown.  |  
| Feature Keys | FeatureKeys | List<string><br/>  [Picklist: FeatureKey-Multiselect] | Select the feature keys that a user requires to access this app. If no feature keys are specified (default) here then all users with sufficient access rights will be able to select the app in the App Launcher.  |  
| Custom | IsCustom | Bool |  |  
| Organization Id | OrganizationId | Guid?<br/>  [ForeignKey Organization] |  |  
| Created Date | CreatedDate | DateTime |  |  
| Created By | CreatedBy | String |  |  
| Modified Date | ModifiedDate | DateTime |  |  
| Modified By | ModifiedBy | String |  |  
| Row Version | RowVersion | Int |  |  

