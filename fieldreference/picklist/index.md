# 


## Picklist
Modify user-defined picklists, eg Client Categories or Marketing Segments

| Field Label | Field Name | Field Type | Description |  
| ---- | ---- | ---- | ---- |  
| Picklist Id | PicklistId | Guid<br/>  [Key]<br/>  [Required]<br/>  [ReadOnly] |  |  
| Picklist Name | PicklistName | String<br/>  [Descriptor]<br/>  [Unique]<br/>  [MinLen: 2]<br/>  [MaxLen: 50]<br/>  [Regex: ^[a-zA-Z_]\w*$]<br/>  [ReadOnlyAfterInsert] | A unique and url-safe name for this picklist. It is used to refer to the picklist in processes and in the external API. The name is derived from the picklist label by default and can only be edited when creating a new picklist.  |  
| Picklist Label | PicklistLabel | String | The name of the picklist as it appears on pages and forms.  |  
| Description | PicklistDescription | String<br/>  [Template: MultilineText] | It is useful to describe the Picklist's purpose and for which entities it intended for when it is a global Picklist.  |  
| Sorted | AutoSort | Bool | Indicates whether values should be sorted (true), or not (false). By default this value is false.  |  
| Color Source | ColorSource | ColorSource | <br/>  Allowable Values: <br/>  <br/>  **None**: Items not given a color |ColorSource.None<br/>  **Dynamic**: Assign colors to values dynamically assigns colors when a chart is generated. For example, if you need only certain Picklist values to have fixed colors in charts, manually assign colors to those values and leave the rest to be assigned dynamically. |ColorSource.Dynamic<br/>  **Fixed**: Assigns a fixed color to each value from the standard set of chart colors. The Chart Colors column shows the assigned colors. For example, if you want Closed Lost values always to be red in charts grouped by Opportunity Stage, assign red to that Picklist value. |ColorSource.Fixed |  
| Organization Id | OrganizationId | Guid?<br/>  [ForeignKey Organization] |  |  
| Created | CreatedBy | String | Indicates the user who created the record, along with the record creation date and time. Read only.  |  
| Created Date | CreatedDate | DateTime |  |  
| Last Modified By | ModifiedBy | String | Indicates the user who last changed the record, along with the record modification date and time. This field is read only.  |  
| Modified Date | ModifiedDate | DateTime |  |  
| Row Version | RowVersion | Int |  |  

