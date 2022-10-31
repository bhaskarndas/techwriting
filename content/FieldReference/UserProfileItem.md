---
title: "UserProfileItem"
date: 2022-10-29T21:38:14+05:30

---

## UserProfileItem
| Field Label | Field Name | Field Type | Description |  
| ---- | ---- | ---- | ---- |  
| Profile Item Id | ProfileItemId | Guid<br/>  [Key]<br/>  [Required]<br/>  [ReadOnly] |  |  
| Profile Id | ProfileId | Guid<br/>  [ForeignKey UserProfile]<br/>  [Required] |  |  
| Name | ProfileItemName | String<br/>  [Required]<br/>  [Descriptor]<br/>  [ReadOnlyAfterInsert] | Security Profile Name |  
| Description | ProfileItemDescription | String |  |  
| Scope Id | ScopeId | String | Scope Ids are identifiers for resources that a user wants to access. The resource can be an entity together with related tables (eg Securities including EOD Prices), an operation (eg, 'Import EOD Security Prices') or a combination of both (eg, 'Manage Portfolios'). The ScopeId with be idential to the entity name for IOwnerEntity entities. |  
| Permission Type | PermissionType | PermissionType | Specifies whether the profile item permission applies to Entities or the Application. App permissions can refer to a single menu option such as 'Import EOD Security Prices' or to a broader set of permissions such as 'Manage Portfolio' which also enables the 'Read' and 'Create' object permissions for Investment Accounts.<br/>  Allowable Values: <br/>  <br/>  **Entity**<br/>  **Action** |  
| Entity Owner Type | EntityOwnerType | EntityOwnerType | Specifies the entity ownership type for profile items that apply to single entities or groups of entities. <br/>  Allowable Values: <br/>  <br/>  **Undefined**<br/>  **SubtenantEntity**: A Subtenant Entity has records that are owned by a specific Subtenant of an organization which can be accessed in their Customer/Subtenant portal, e.g. Expenses, Fixed Assets. <br/>  **TenantEntity**: An Tenant Entity has records that are all owned by a specific organization/tenant, e.g. Employees, Leads, Opportunities, Cases. <br/>  **TenantSharedEntity**: An Tenant Shared Entity has records that are owned by a tenant/organization but can be shared with subtenants, e.g. Documents, Cases. <br/>  **AppSharedEntity**: An App Shared Entity has records that can belong to a single organization or be shared across organizations, e.g. standard picklists. These entities can also be viewed by subtenants. <br/>  **CommonEntity**: A Common Entity has records that can be viewed/selected by tenants/organizations, but are owned/managed by app administrators/helpdesk staff, e.g. Currencies, Currency Rates, Translations.<br/>  **AppEntity**: An App Entity has records that can only be viewed/edited by app administrators/helpdesk staff, e.g. the Staff entity itself. |  
| Is Record Owner Entity | IsRecordOwnerEntity | Bool |  |  
| Is Self Context | IsSelfContext | Bool |  |  
| Create | CreateEnabled | Bool | User is able to add a new record.  |  
| Read | ReadEnabled | Bool | User is able to view a record.  |  
| Edit | UpdateEnabled | Bool | User is able to edit/modify a record.  |  
| Delete | DeleteEnabled | Bool | User is able to delete a record.  |  
| Assign | AssignEnabled | Bool | User is able to transfer a record assigned to them to another user. |  
| Access Level | EntityAccess | AccessLevel | Specifies the access permissions a user has to entities and groups of entities. When an entity contains both shared and firm-specific records, such as in Picklists, then the access level shown only applies Portfolios,<br/>  Allowable Values: <br/>  <br/>  **NoAccess**: Entities, resources and procedures marked by No Access will not be selectable in user menus. Potentially, visible Users may see some records in lists but will not be view record details. |CommonEntityAccess.NoAccess<br/>  **ReadEnabled**: Users can view record details including related information, but can not modify or update the data. |CommonEntityAccess.ReadEnabled<br/>  **UpdateEnabled**: Users can view and modify records and also create new records. |CommonEntityAccess.UpdateEnabled<br/>  **FullControl**: Full control includes View, Modify and Delete permissions. |CommonEntityAccess.DeleteEnabled<br/>  **NotApplicable** |  
| Own Record | SelfAccess | SelfAccess | Specifies the access permissions a user has to their own record, for example, for a Contact accessing their own Contact record via the User Settings page or an Employee accessing their own record in the Employee List.<br/>  Allowable Values: <br/>  <br/>  **NoAccess**<br/>  **ReadOnly**<br/>  **ReadUpdate**<br/>  **FullControl** |  
| Enabled | ActionEnabled | Bool | Application permissions control what users can do within the App. For example, the 'Import EOD Prices' permission allows users to import End of Day pricing information is the Securities entity, while the 'Run Backtest' permission allows users to specify backtesting parameters and run the test. |  
| Item Icon Name | ItemIconName | String |  |  
| Item Icon Color | ItemIconColor | String |  |  
| Organization Id | OrganizationId | Guid?<br/>  [ForeignKey Organization] |  |  
| Created Date | CreatedDate | DateTime |  |  
| Created By | CreatedBy | String |  |  
| Modified Date | ModifiedDate | DateTime |  |  
| Modified By | ModifiedBy | String |  |  
| Row Version | RowVersion | Int |  |  
