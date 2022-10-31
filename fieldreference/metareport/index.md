# 

﻿## MetaReport
| Field Label | Field Name | Field Type | Description |  
| ---- | ---- | ---- | ---- |  
| Report Id | ReportId | Guid<br/>  [Key]<br/>  [Required]<br/>  [ReadOnly] |  |  
| Entity Id | EntityId | Guid<br/>  [ForeignKey MetaEntity]<br/>  [Required] |  |  
| Name | ReportName | String<br/>  [Required]<br/>  [Descriptor] | The name of the Report as it appears on pages and forms |  
| Report API Name | ReportApiName | String<br/>  [Required]<br/>  [TenantUnique]<br/>  [MinLen: 2]<br/>  [MaxLen: 50]<br/>  [Regex: ^[a-zA-Z_][a-zA-Z0-9_.-]*$]<br/>  [ReadOnlyAfterInsert] | A unique and url-safe API name for this report. It is used to refer to the report in processes and in the external API. The name is derived from the report name by default and can only be edited when creating a new report.  |  
| Report Description | ReportDescription | String |  |  
| Custom | IsCustom | Bool |  |  
| Organization Id | OrganizationId | Guid?<br/>  [ForeignKey Organization] |  |  
| Created Date | CreatedDate | DateTime |  |  
| Created By | CreatedBy | String |  |  
| Modified Date | ModifiedDate | DateTime |  |  
| Modified By | ModifiedBy | String |  |  
| Row Version | RowVersion | Int |  |  

