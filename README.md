# PublicCSMM_Logs
Raw logs from "Civil Status Management Module" (CSMM) of "Software for public services" (SFPS).


The data are available under the ODC Open Database License (ODbL)
[click here for more details](https://github.com/FM-BL/PublicCSMM_Logs#odc-open-database-license-odbl)

------
## Data set description
### Logs
Data set consists of 29 log files. Each file starts and ends with the `dataroot` tags.<br/>
Between these tags, events are listed by the `ExportList` tags. 
The event list is sorted in reverse chronological order (the most recent first, the oldest at the end).<br/>

### Event
An event has four fileds (tags).
1. `FormName` : represents a unique form code
1. `UserID` : indicates the user id performing the action
1. `OpeningTimestamp` : the form opening dates
1. `ClosingTimestamp` : the form closing dates. _Note : in some cases, the closing field might be missing. It means either that the form encountered an error, making it impossible to write the closing date or that the form was not closed before leaving the application._

### Forms hierarchy
* `LEVEL1_HOME_FORM` : the home page
  * `LEVEL2_FORM_1 | LEVEL2_FORM_2 | ... | LEVEL2_FORM_11` : the 11 sub-forms, they describe the 2nd level of navigation
    * `otherForm_0` to `otherForm_739` : the other forms
    
------

## ODC Open Database License (ODbL)

### Preamble

The Open Database License (ODbL) is a license agreement intended to
allow users to freely share, modify, and use this Database while
m
