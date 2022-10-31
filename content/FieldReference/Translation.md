## Translation
| Field Label | Field Name | Field Type | Description |  
| ---- | ---- | ---- | ---- |  
| Translation Id | TranslationId | Int<br/>  [Key]<br/>  [Required]<br/>  [ReadOnly] |  |  
| String Id | StringId | String<br/>  [ReadOnlyAfterInsert] |  |  
| English | StringEnGb | String |  |  
| String En Gb Verified | StringEnGbVerified | Bool |  |  
| Dutch | StringNlNl | String |  |  
| Verified? | StringNlNlVerified | Bool |  |  
| German | StringDeDe | String |  |  
| Verified? | StringDeDeVerified | Bool |  |  
| French | StringFrFr | String |  |  
| Verified? | StringFrFrVerified | Bool |  |  
| Orphan String | OrphanString | Bool |  |  
| Organization Id | OrganizationId | Guid?<br/>  [ForeignKey Organization] |  |  
| Created Date | CreatedDate | DateTime |  |  
| Created By | CreatedBy | String<br/>  [Descriptor] |  |  
| Modified Date | ModifiedDate | DateTime |  |  
| Modified By | ModifiedBy | String |  |  
| Row Version | RowVersion | Int |  |  
