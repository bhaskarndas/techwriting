# 

﻿## MetaAppMetaEntityLink
| Field Label | Field Name | Field Type | Description |  
| ---- | ---- | ---- | ---- |  
| Link Id | LinkId | Guid<br/>  [Key]<br/>  [Required]<br/>  [ReadOnly] |  |  
| App Id | AppId | Guid<br/>  [ForeignKey MetaApp]<br/>  [Required] |  |  
| Entity Id | EntityId | Guid<br/>  [ForeignKey MetaEntity]<br/>  [Required] |  |  
| Display In Menu | DisplayInMenu | Bool |  |  
| Display In Launcher | DisplayInLauncher | Bool |  |  
| Custom | IsCustom | Bool |  |  
| Display Order | DisplayOrder | Int |  |  
| Organization Id | OrganizationId | Guid?<br/>  [ForeignKey Organization] |  |  
| Created Date | CreatedDate | DateTime |  |  
| Created By | CreatedBy | String<br/>  [Descriptor] |  |  
| Modified Date | ModifiedDate | DateTime |  |  
| Modified By | ModifiedBy | String |  |  
| Row Version | RowVersion | Int |  |  

