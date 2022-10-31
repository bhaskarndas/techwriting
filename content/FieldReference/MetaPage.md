
## MetaPage
Configure how entity lists and details pages are displayed  

| Field Label | Field Name | Field Type | Description |  
| ---- | ---- | ---- | ---- |  
| Page Id | PageId | Guid<br/>  [Key]<br/>  [Required]<br/>  [ReadOnly] |  |  
| Entity Id | EntityId | Guid<br/>  [ForeignKey MetaEntity]<br/>  [Required] |  |  
| Name | PageName | String<br/>  [Required]<br/>  [Descriptor] | The name of the Page as it appears on pages and forms |  
| Page API Name | PageApiName | String<br/>  [Required]<br/>  [TenantUnique]<br/>  [MinLen: 2]<br/>  [MaxLen: 50]<br/>  [Regex: ^[a-zA-Z_][a-zA-Z0-9_.-]*$]<br/>  [ReadOnlyAfterInsert] | A unique and url-safe API name for this page. It is used to refer to the page and in internal processes and in the external API. The name is derived from the page name by default and can only be edited when creating a new page.  |  
| Page Description | PageDescription | String<br/>  [Template: MultilineText] | Specify a short description of the page that appears when users hover over its icon with their mouse or tap on the info icon in Mobile.  |  
| Help Text | HelpText | String | Use this space to provide more detailed guidance to your users. Text can be formatted using Markdown which is an easy-to-read, easy-to-write syntax for formatting plain text.syntax. Markdown can also include hyperlinks,for example, to access additional help information. The help text position and display style are governed by the Help Text Position dropdown.  |  
| Page Help Text Position | PageHelpTextPosition | PageHelpTextPosition | Determines where and how the text entered in the Help Text field will be displayed on the page. See the option descriptions in the dropdown. <br/>  Allowable Values: <br/>  <br/>  **IconLink**: Displays a question mark icon in the page header. When a user clicks on the link, the help text appears in a popup window. <br/>  **HelpSection**: Displays the help text in Section of type PageHelp that can be located anywhere on the page. If no page help section is found, then one will be added to the bottom of the page. <br/>  **DoNotDisplay**: Helptext does not display. This can be overriden on individual page layouts.  |  
| Page Type | PageType | PageType | <br/>  Allowable Values: <br/>  <br/>  **Entity**: An Entity Page is typically used to display a list of entity records, for example, the list of Contacts. <br/>  **EntityArchive**: An Entity Archive Page is used to display a list of archived entity records. <br/>  **RecordDetails**: A Record Details Page is used to display and edit the contents of a single entity record, for example, a Contact record. <br/>  **Dashboard**: Dashboard pages are typically used as home pages and can contain a wide variety of components.  |  
| Page Style | PageStyle | PageStyle | <br/>  Allowable Values: <br/>  <br/>  **Modern**<br/>  **Classic** |  
| Page Layout | PageLayout | ModelElement |  |  
| Feature Keys | FeatureKeys | List<string><br/>  [Picklist: FeatureKey-Multiselect] | Select the feature keys that a user requires to access this page. If no feature keys are specified (default) here then all users with sufficient access rights will be able to view the page.  |  
| Icon | PageIconName | String | Specify the name of a FontAwesome icon to display when the entitity appears on pages and forms. For example, 'fal fa-cogs' will display a large cog and two smaller ones to the right. See the entire list at: https://fontawesome.com/icons?d=gallery&s=light |  
| Color | PageIconColor | String<br/>  [MaxLen: 7]<br/>  [Regex: #([A-Fa-f0-9]{6})] | Specify the web color used to provide the icon background when the entity icon is displayed. The web color must be specified in web hex format and must begin with a leading # sign and contain 6 additional characters consisting of the letters A-F and the numbers 0-9. For example, the code '#00204F' specifies the color we use for the main menu background. You can select a color from the color picker or enter one directly.  |  
| Classic Model Name | ModelName | String | Specify the name of the C# model class to use for classic pages. The model required depends on the Page Type, eg a details page model for pages of type DetailsPage.  |  
| Layout Model Name | LayoutModelName | String | Used when a developer wants a custom layout for an Entity (List) page. Specify the name of the C# model class whose fluent layout will be used.  |  
| Custom | IsCustom | Bool |  |  
| Default User Flags | DefaultUserFlags | DefaultUserFlags | <br/>  Allowable Values: <br/>  <br/>  **Client**<br/>  **Employee**<br/>  **Staff** |  
| Default Client | IsDefaultClient | Bool | Marks a page as the default entity page for clients.  |  
| Default Employee | IsDefaultEmployee | Bool | Marks a page as the default entity page for firm employees.  |  
| Default Staff | IsDefaultStaff | Bool | Marks a page as the default entity page for helpdesk staff.  |  
| Record Type Id | RecordTypeId | Guid?<br/>  [ForeignKey RecordType] | Linking a page layout to a specific record type makes it possible to display and edit only the fields required for a particular use.  |  
| Organization Id | OrganizationId | Guid?<br/>  [ForeignKey Organization] |  |  
| Created Date | CreatedDate | DateTime |  |  
| Created By | CreatedBy | String |  |  
| Modified Date | ModifiedDate | DateTime |  |  
| Modified By | ModifiedBy | String |  |  
| Row Version | RowVersion | Int |  |  
