
## PicklistItem
| Field Label | Field Name | Field Type | Description |  
| ---- | ---- | ---- | ---- |  
| Picklist Item Id | PicklistItemId | Guid<br/>  [Key]<br/>  [Required]<br/>  [ReadOnly] |  |  
| Item Name | PicklistItemName | String<br/>  [Descriptor]<br/>  [MinLen: 2]<br/>  [MaxLen: 100]<br/>  [Regex: ^[\w_\-&/.,':<>+%()$€£ ]*$]<br/>  [ReadOnlyAfterInsert] | Once created, picklist items can only be renamed with the Rename menu option.  |  
| Picklist Id | PicklistId | Guid<br/>  [ForeignKey Picklist]<br/>  [Required] |  |  
| Picklist Name | PicklistName | String<br/>  [MaxLen: 50]<br/>  [ReadOnly] | The name of the picklist this item is a member of.  |  
| Help Text | HelpText | String | Admins can add additional information for their users on a picklist item here and include guidance on the correct use of picklist items.  |  
| Controlling Field Values | ControllingFieldValues | String | A list of values in the controlling field for dependent picklists that determine whether a picklist item is displayed. If any value is specified in ControllingFieldValues, then this picklist item will only be visible if the fully specified value of the controlling field occurs in ControllingFieldValues. If ControllingFieldValues is empty, then all picklist items will be displayed.  |  
| Record Type | RecordTypeId | Guid?<br/>  [ForeignKey RecordType] | Use record types to enable different different picklists for the same field. For example, you can link an opportunity stage picklist item to a particular record type in order to tailer the list of stages that appears per opportunity record type. Corporate opportunities can then have a longer and more complex series of stages than SMB opportunities.  |  
| Item Icon | ItemIcon | String |  |  
| Is Closed | IsClosed | Bool | Indicates whether this picklist value is associated with a closed status. This field is relevant for the standard Opportunity Stage field in opportunities and the standard Status field in cases and tasks. It field makes it possible to have multiple stages and status picklist items that will be lead to the relevant record being marked as closed.  |  
| Is Completed | IsCompleted | Bool | Indicates whether this picklist value is associated with a completed status. This field is relevant for only the standard TransferStage field in PackControl.Transfer. This field makes it possible to have multiple different Transfer Stages that will be lead to the relevant record being marked as completed.  |  
| Is Converted | IsConverted | Bool | Indicates whether this picklist value is associated with a converted status. This field is relevant for only the standard Prospect Status field in Leads and makes it possible to have multiple Prospect status picklist items that will be cause a lead to be marked as converted.  |  
| Probability | Probability | Decimal<br/>  [Template: Percentage] | Specifies the likelihood that opportunity will close stated as a percentage. This field is only relevant for the Stage field in opportunities.  |  
| Is High Priority | IsHighPriority | Bool | Indicates whether this value is a high priority item (true), or not (false). This field is only relevant for the standard TaskPriority field in Activities.  |  
| Cash Security | CashSecurity | Bool | Indicates whether this value is considered a cash security item (true), or not (false). This field is only relevant for the standard SecurityType field in Securities.  |  
| Display Order | DisplayOrder | Int |  |  
| Archived | IsArchived | Bool | Use the Archive checkbox to hide inactive records without deleting them. Archiving will prevent them from being selected in dropdown lists or appearing on list pages. Usage in existing records will not be affected. Archived records are stored indefinitely and be viewed in the archived items app group where they can be unarchived if needed again.  |  
| Created | CreatedBy | String | Indicates the user who created the record, along with the record creation date and time. Read only.  |  
| Created Date | CreatedDate | DateTime |  |  
| Last Modified By | ModifiedBy | String | Indicates the user who last changed the record, along with the record modification date and time. This field is read only.  |  
| Modified Date | ModifiedDate | DateTime |  |  
| Organization Id | OrganizationId | Guid?<br/>  [ForeignKey Organization] |  |  
| Row Version | RowVersion | Int |  |  
