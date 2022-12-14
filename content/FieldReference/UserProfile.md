

## UserProfile
Configure access permissions for each user profile  

| Field Label | Field Name | Field Type | Description |  
| ---- | ---- | ---- | ---- |  
| Profile Id | ProfileId | Guid<br/>  [Key]<br/>  [Required]<br/>  [ReadOnly] |  |  
| Profile Name | ProfileName | String<br/>  [Required]<br/>  [Descriptor] | User access security profile name |  
| Profile Description | ProfileDescription | String |  |  
| User Type | UserType | UserType<br/>  [ReadOnlyAfterInsert] | <br/>  Allowable Values: <br/>  <br/>  **Anonymous**<br/>  **Contact**<br/>  **Employee**<br/>  **TenantApiToken**<br/>  **TenantAgent**<br/>  **Staff**<br/>  **System** |  
| View All Data | CanViewAllData | Bool | Enable for users who need access to all of a firm's data but do not need to modify it. Caution: this setting overrides any other data viewing limitation in a user profile including those limiting access rights to record owners.  |  
| Modify All Data | CanModifyAllData | Bool | This setting which gives full Create/Read/Update/Delete rights to all data is enabled System Administrators. It canalso be enabled for employees as needed, for example to enable data cleansing, deduplication, mass deletion, and mass transferring. Caution: this setting overrides any other data access and editing limitation in a user profile.  |  
| Adminstrator | IsAdministrator | Bool | Enable for System Administrators and similar employees.  |  
| Primary Group Access Permission Type | PrimaryGroupAccess | PrimaryGroupAccess | These access permissions apply to contacts where they are linked to the same primary group. Eg, as person contacts who work for a company contact, or family members who who are related to the same Household. <br/>  Allowable Values: <br/>  <br/>  **None**: No access to contact records linked to a contact via relationships. <br/>  **ParentContactOnly**: Contact user can access the primary contact only, eg, an employee can view company they work for including related opportunities and other records (if permitted), but not drill down to see other employees working for the same firm. In a household, a spouse could see their partner's record and related financial information, but not the records of any children or others related to the primary contact as their primary group. <br/>  **EntireGroup**: Contact user can access both the primary contact and the records of other contacts related to the primary contact. In a household, a spouse could see both their partner's record and related financial information and the records of any children or others related to the primary contact as their primary group. In a context where the primary contact is a company and the contact user has been related to the company as an employee, then the user could access both the record of the company they work for and the records of any other persons working for the same company.  |  
| Group Access Type | GroupAccessType | GroupAccessType | Specifies which User Profile will apply when a contact is accessing related contacts in their primary group. <br/>  Allowable Values: <br/>  <br/>  **UsersOwnProfile**: For example, a partner/spouse in a Household with read-only access permission for their own record, would then have the same permissions for other family members when they have group access to the entire group. <br/>  **ParentContactUserProfile**: This option effectively gives the contact group member the same access permissions as the Primary Group Member for contact records belonging to the same primary group. This could be useful for spouses and adult children who have been given log in credentials for a household group. <br/>  **RelationshipSpecificUserProfile**: Selecting this option enables the option to specify a profile name per relationship in a primary group. This gives very fine-grained access controle but does require more work to set up.  |  
| Custom | IsCustom | Bool |  |  
| Organization Id | OrganizationId | Guid?<br/>  [ForeignKey Organization] |  |  
| Created Date | CreatedDate | DateTime |  |  
| Created By | CreatedBy | String |  |  
| Modified Date | ModifiedDate | DateTime |  |  
| Modified By | ModifiedBy | String |  |  
| Row Version | RowVersion | Int |  |  
