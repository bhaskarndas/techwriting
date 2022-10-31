

## ApplicationUser
| Field Label | Field Name | Field Type | Description |  
| ---- | ---- | ---- | ---- |  
| Id | Id | String<br/>  [Key]<br/>  [Required]<br/>  [Unique]<br/>  [MaxLen: 36]<br/>  [ReadOnlyAfterInsert] |  |  
| User Name | UserName | String<br/>  [Descriptor] |  |  
| Normalized User Name | NormalizedUserName | String |  |  
| Email | Email | String |  |  
| Normalized Email | NormalizedEmail | String |  |  
| Email Confirmed | EmailConfirmed | Bool |  |  
| Password Hash | PasswordHash | String |  |  
| Security Stamp | SecurityStamp | String |  |  
| Concurrency Stamp | ConcurrencyStamp | String |  |  
| Phone Number | PhoneNumber | String |  |  
| Phone Number Confirmed | PhoneNumberConfirmed | Bool |  |  
| Two Factor Enabled | TwoFactorEnabled | Bool |  |  
| Lockout End | LockoutEnd | DateTimeOffset? |  |  
| Lockout Enabled | LockoutEnabled | Bool |  |  
| Access Failed Count | AccessFailedCount | Int |  |  
