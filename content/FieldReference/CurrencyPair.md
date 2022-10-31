## CurrencyPair
| Field Label | Field Name | Field Type | Description |  
| ---- | ---- | ---- | ---- |  
| Currency Pair Id | CurrencyPairId | Int<br/>  [Key]<br/>  [Required]<br/>  [ReadOnly] |  |  
| Base Currency Code | BaseCurrencyCode | String<br/>  [ForeignKey Currency]<br/>  [Descriptor]<br/>  [MaxLen: 3] |  |  
| Quote Currency Code | QuoteCurrencyCode | String<br/>  [ForeignKey Currency]<br/>  [MaxLen: 3] |  |  
| Data Source | DataSource | String |  |  
| Data Set | DataSet | String |  |  
