## Job
| Field Label | Field Name | Field Type | Description |  
| ---- | ---- | ---- | ---- |  
| Job Id | JobId | Guid<br/>  [Key]<br/>  [Required]<br/>  [ReadOnly] |  |  
| Hangfire Job Id | HangfireJobId | String |  |  
| Hangfire Job Active | HangfireJobActive | Bool |  |  
| Job | JobDescription | String<br/>  [Required]<br/>  [Descriptor]<br/>  [Unique] |  |  
| Task Name | JobMethodCall | String | Provide the name of a class with the IBackgroundTask interface.  |  
| Schedule | ScheduleType | ScheduleType | <br/>  Allowable Values: <br/>  <br/>  **None**<br/>  **Hourly**<br/>  **Daily**<br/>  **Weekly**<br/>  **Monthly**<br/>  **Minutes**<br/>  **RunOnce** |  
| Description | ScheduleDescription | String |  |  
| Minute Interval | MinuteInterval | MinuteInterval | <br/>  Allowable Values: <br/>  <br/>  **Minute01**<br/>  **Minute02**<br/>  **Minute03**<br/>  **Minute04**<br/>  **Minute05**<br/>  **Minute10**<br/>  **Minute15**<br/>  **Minute20**<br/>  **Minute25**<br/>  **Minute30**<br/>  **Minute35**<br/>  **Minute40**<br/>  **Minute45**<br/>  **Minute50**<br/>  **Minute55** |  
| Hour Interval | HourInterval | HourInterval | <br/>  Allowable Values: <br/>  <br/>  **Hour01**<br/>  **Hour02**<br/>  **Hour03**<br/>  **Hour04**<br/>  **Hour05**<br/>  **Hour06**<br/>  **Hour07**<br/>  **Hour08**<br/>  **Hour09**<br/>  **Hour10**<br/>  **Hour11**<br/>  **Hour12** |  
| Minute Offset | MinuteOffset | MinuteOffset | <br/>  Allowable Values: <br/>  <br/>  **Offset01**<br/>  **Offset02**<br/>  **Offset03**<br/>  **Offset04**<br/>  **Offset05**<br/>  **Offset10**<br/>  **Offset15**<br/>  **Offset20**<br/>  **Offset25**<br/>  **Offset30**<br/>  **Offset35**<br/>  **Offset40**<br/>  **Offset45**<br/>  **Offset50**<br/>  **Offset55** |  
| Day Of Month | DayOfMonth | DayOfMonth | <br/>  Allowable Values: <br/>  <br/>  **Day01**<br/>  **Day02**<br/>  **Day03**<br/>  **Day04**<br/>  **Day05**<br/>  **Day06**<br/>  **Day07**<br/>  **Day08**<br/>  **Day09**<br/>  **Day10**<br/>  **Day11**<br/>  **Day12**<br/>  **Day13**<br/>  **Day14**<br/>  **Day15**<br/>  **Day16**<br/>  **Day17**<br/>  **Day18**<br/>  **Day19**<br/>  **Day20**<br/>  **Day21**<br/>  **Day22**<br/>  **Day23**<br/>  **Day24**<br/>  **Day25**<br/>  **Day26**<br/>  **Day27**<br/>  **Day28** |  
| Start Time | StartTime | TimeSpan |  |  
| Time Zone | TimeZoneId | TimeZoneIds | <br/>  Allowable Values: <br/>  <br/>  **MoroccoStandardTime**<br/>  **GMTStandardTime**<br/>  **GreenwichStandardTime**<br/>  **WEuropeStandardTime**<br/>  **CentralEuropeStandardTime**<br/>  **RomanceStandardTime**<br/>  **CentralEuropeanStandardTime**<br/>  **WCentralAfricaStandardTime**<br/>  **JordanStandardTime**<br/>  **GTBStandardTime**<br/>  **MiddleEastStandardTime**<br/>  **EgyptStandardTime**<br/>  **SouthAfricaStandardTime**<br/>  **FLEStandardTime**<br/>  **IsraelStandardTime**<br/>  **EEuropeStandardTime**<br/>  **NamibiaStandardTime**<br/>  **ArabicStandardTime**<br/>  **ArabStandardTime**<br/>  **RussianStandardTime**<br/>  **EAfricaStandardTime**<br/>  **GeorgianStandardTime**<br/>  **IranStandardTime**<br/>  **ArabianStandardTime**<br/>  **AzerbaijanStandardTime**<br/>  **MauritiusStandardTime**<br/>  **CaucasusStandardTime**<br/>  **AfghanistanStandardTime**<br/>  **EkaterinburgStandardTime**<br/>  **PakistanStandardTime**<br/>  **WestAsiaStandardTime**<br/>  **IndiaStandardTime**<br/>  **SriLankaStandardTime**<br/>  **NepalStandardTime**<br/>  **NCentralAsiaStandardTime**<br/>  **CentralAsiaStandardTime**<br/>  **MyanmarStandardTime**<br/>  **SEAsiaStandardTime**<br/>  **NorthAsiaStandardTime**<br/>  **ChinaStandardTime**<br/>  **NorthAsiaEastStandardTime**<br/>  **SingaporeStandardTime**<br/>  **WAustraliaStandardTime**<br/>  **TaipeiStandardTime**<br/>  **TokyoStandardTime**<br/>  **KoreaStandardTime**<br/>  **YakutskStandardTime**<br/>  **CenAustraliaStandardTime**<br/>  **AUSCentralStandardTime**<br/>  **EAustraliaStandardTime**<br/>  **AUSEasternStandardTime**<br/>  **WestPacificStandardTime**<br/>  **TasmaniaStandardTime**<br/>  **VladivostokStandardTime**<br/>  **CentralPacificStandardTime**<br/>  **NewZealandStandardTime**<br/>  **FijiStandardTime**<br/>  **TongaStandardTime**<br/>  **AzoresStandardTime**<br/>  **CapeVerdeStandardTime**<br/>  **MidAtlanticStandardTime**<br/>  **ESouthAmericaStandardTime**<br/>  **ArgentinaStandardTime**<br/>  **SAEasternStandardTime**<br/>  **GreenlandStandardTime**<br/>  **MontevideoStandardTime**<br/>  **NewfoundlandStandardTime**<br/>  **AtlanticStandardTime**<br/>  **SAWesternStandardTime**<br/>  **CentralBrazilianStandardTime**<br/>  **PacificSAStandardTime**<br/>  **VenezuelaStandardTime**<br/>  **SAPacificStandardTime**<br/>  **EasternStandardTime**<br/>  **USEasternStandardTime**<br/>  **CentralAmericaStandardTime**<br/>  **CentralStandardTime**<br/>  **CentralStandardTimeMexico**<br/>  **CanadaCentralStandardTime**<br/>  **USMountainStandardTime**<br/>  **MountainStandardTimeMexico**<br/>  **MountainStandardTime**<br/>  **PacificStandardTime**<br/>  **PacificStandardTimeMexico**<br/>  **AlaskanStandardTime**<br/>  **HawaiianStandardTime**<br/>  **SamoaStandardTime**<br/>  **DatelineStandardTime** |  
| Time Zone Iana Name | TimeZoneIanaName | String |  |  
| UTC Offset | TimeZoneUtcOffset | Decimal | Timezone offset in hours relative to UTC (GMT).  |  
| Sun | RunOnSunday | Bool |  |  
| Mon | RunOnMonday | Bool |  |  
| Tue | RunOnTuesday | Bool |  |  
| Wed | RunOnWednesday | Bool |  |  
| Thu | RunOnThursday | Bool |  |  
| Fri | RunOnFriday | Bool |  |  
| Sat | RunOnSaturday | Bool |  |  
| Cron Expression | CronExpression | String |  |  
| Entity Name | EntityName | String | Stores the entity name when a job record is related to a DataLoaderTask or a WorkFlow schedule trigger.  |  
| Guid Id | GuidId | Guid? | Stores the guid record id when a job record is related to a table that has a guid as its primary key.  |  
| Int Id | IntId | Int? | Stores the int record id when a job record is related to a table that has an int as its primary key.  |  
| Organization Id | OrganizationId | Guid?<br/>  [ForeignKey Organization] |  |  
| Created Date | CreatedDate | DateTime |  |  
| Created By | CreatedBy | String |  |  
| Modified Date | ModifiedDate | DateTime |  |  
| Modified By | ModifiedBy | String |  |  
| Row Version | RowVersion | Int |  |  
