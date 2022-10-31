## Media
The Media entity stores links to media such as PDFs, images, and spreadsheets uploaded by employees or clients. It is a system table and cannot be edited by users.  
  
| Field Label | Field Name | Field Type | Description |  
| ---- | ---- | ---- | ---- |  
| Media Id | MediaId | Guid<br/>  [Key]<br/>  [Required]<br/>  [ReadOnly] |  |  
| Blob Name | BlobName | String | Media such as images, documents and other files are stored as BLOBs (Binary Large Objects) in Azure Cloud Storage.  |  
| File Name | FileName | String<br/>  [Descriptor] | Original name of the uploaded media file.  |  
| Mime Type | MimeType | String | A media type (also known as a Multipurpose Internet Mail Extensions or MIME type) is a standard that indicates the nature and format of a document, file, or assortment of bytes, eg 'application/vnd.ms-excel'.  |  
| File Size | FileSize | Int64 | Size of the media file that has been uploaded in Bytes.  |  
| Upload Date | UploadDate | DateTime | Date and time the media file was uploaded.  |  
| File Access Security | FileAccessSecurity | FileAccessSecurity | File access security level required to access the media file, e.g. Client or Organization. <br/>  Allowable Values: <br/>  <br/>  **Subtenant**<br/>  **Tenant**<br/>  **Anonymous** |  
| Upload User Id | UserId | String | The user id of the person who uploaded the media file.  |  
| Organization Id | OrganizationId | Guid?<br/>  [ForeignKey Organization] |  |  
| Is Permanent | IsPermanent | Bool | Uploaded media files are not made permanent until a user saves the record to which the media file is linked, eg a Contact record. Media records that are not marked as permanent are deleted after 24 hours.  |  
