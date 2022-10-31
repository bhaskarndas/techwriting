

## Country
| Field Label | Field Name | Field Type | Description |  
| ---- | ---- | ---- | ---- |  
| Country Code | CountryCode | String<br/>  [Key]<br/>  [Required]<br/>  [Unique]<br/>  [MinLen: 2]<br/>  [MaxLen: 2]<br/>  [ReadOnlyAfterInsert] | ISO 2 letter country code.  |  
| Country Name | CountryName | String<br/>  [Required]<br/>  [Descriptor] |  |  
| ISO 3 Letter Code | Iso3Code | String<br/>  [Unique]<br/>  [MaxLen: 3] | ISO 3 letter country code.  |  
| Currency Code | CurrencyCode | String<br/>  [ForeignKey Currency]<br/>  [MaxLen: 3] |  |  
| Address Template | AddressTemplate | String |  |  
| Base List | BaseList | Bool |  |  
