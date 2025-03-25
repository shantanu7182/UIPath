SYNTAX
    . 'C:\scripts\UiPathJobRun.ps1' <process_name> <orchestrator_url> <orchestrator_tenant> [-input_path <input_path>] [-jobscount <jobscount>] [-result_path <result_path>] [-priority <priority>] [-robots <robots>] 
    [-fail_when_job_fails <do_not_fail_when_job_fails>] [-timeout <timeout>] [-wait <do_not_wait>] [-orchestrator_user <orchestrator_user> -orchestrator_pass <orchestrator_pass>] [-userKey <auth_token> -accountName <account_name>] [-accountForApp <account_for_app> -applicationId <application_id> -applicationSecret <application_secret> -applicationScope <applicationScope>] [-folder_organization_unit <folder_organization_unit>] [-language <language>] [-user <robotUser>] [-machine <robotMachine>] [-job_type <Unattended, NonProduction>] [-uipathCliFilePath <uipcli_path>]

Example 1:

. 'C:\scripts\UiPathJobRun.ps1' "ProcessName" "https://uipath-orchestrator.myorg.com" default -orchestrator_user admin -orchestrator_pass 123456
. 'C:\scripts\UiPathJobRun.ps1' "ProcessName" "https://uipath-orchestrator.myorg.com" default -orchestrator_user admin -orchestrator_pass 123456 -orchestrator_pass -priority Low
. 'C:\scripts\UiPathJobRun.ps1' "ProcessName" "https://uipath-orchestrator.myorg.com" default -orchestrator_user admin -orchestrator_pass 123456 -orchestrator_pass -priority Normal -folder_organization_unit MyFolder
. 'C:\scripts\UiPathJobRun.ps1' "ProcessName" "https://uipath-orchestrator.myorg.com" default -orchestrator_user admin -orchestrator_pass 123456 -orchestrator_pass -priority High -folder_organization_unit MyFolder
. 'C:\scripts\UiPathJobRun.ps1' "ProcessName" "https://uipath-orchestrator.myorg.com" default -userKey a7da29a2c93a717110a82 -accountName myAccount -fail_when_job_fails false -timeout 0
. 'C:\scripts\UiPathJobRun.ps1' "ProcessName" "https://uipath-orchestrator.myorg.com" default -userKey a7da29a2c93a717110a82 -accountName myAccount -orchestrator_pass -priority High -jobscount 3 -wait false -machine ROBOTMACHINE
. 'C:\scripts\UiPathJobRun.ps1' "ProcessName" "https://cloud.uipath.com/" default -userKey a7da29a2c93a717110a82 -accountName myAccount -orchestrator_pass -priority Low -robots robotName -result_path C:\Temp
. 'C:\scripts\UiPathJobRun.ps1' "ProcessName" "https://uipath-orchestrator.myorg.com" default -userKey a7da29a2c93a717110a82 -accountName myAccount -robots robotName -result_path C:\Temp\status.json
. 'C:\scripts\UiPathJobRun.ps1' "ProcessName" "https://uipath-orchestrator.myorg.com" default -accountForApp accountForExternalApp -applicationId myExternalAppId -applicationSecret myExternalAppSecret -applicationScope "OR.Folders.Read OR.Settings.Read" -robots robotName -result_path C:\Temp\status.json
 

#Note: if script folder location is different you need to replace C: with directory folder (e.g. '[FOLDER_VARIABLE]\scripts\UiPathPack.ps1')