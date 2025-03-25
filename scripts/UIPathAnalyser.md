SYNTAX
    . 'C:\scripts\UiPathAnalyzeProject.ps1' <project_path> [-analyzerTraceLevel <analyzer_trace_level>] [-stopOnRuleViolation <true|false>] [-treatWarningsAsErrors <true|false>] [-saveOutputToFile] [-ignoredRules <activity_1_id,activity_2_id,activity_3_id,activity_4_id>] [-orchestratorUrl <orchestrator_url> -orchestratorTenant <orchestrator_tenant>] [-orchestratorUsername <orchestrator_user> -orchestratorPassword <orchestrator_pass>] [-orchestratorAuthToken <auth_token> -orchestratorAccountName <account_name>] [-orchestratorFolder <folder>] [-uipathCliFilePath <uipcli_path>]

Examples:
    . 'C:\scripts\UiPathAnalyzeProject.ps1' "C:\UiPath\Project\project.json"
    . 'C:\scripts\UiPathAnalyzeProject.ps1' "C:\UiPath\Project\project.json" -analyzerTraceLevel "Error"
    . 'C:\scripts\UiPathAnalyzeProject.ps1' "C:\UiPath\Project\project.json" -analyzerTraceLevel "Error" -stopOnRuleViolation true
    . 'C:\scripts\UiPathAnalyzeProject.ps1' "C:\UiPath\Project\project.json" -analyzerTraceLevel "Error" -stopOnRuleViolation true -treatWarningsAsErrors true 
    . 'C:\scripts\UiPathAnalyzeProject.ps1' "C:\UiPath\Project\project.json" -analyzerTraceLevel "Error" -stopOnRuleViolation true -treatWarningsAsErrors true -resultPath "C:\UiPath\Project\output.json"
    . 'C:\scripts\UiPathAnalyzeProject.ps1' "C:\UiPath\Project\project.json" -analyzerTraceLevel "Error" -stopOnRuleViolation true -treatWarningsAsErrors true -resultPath "C:\UiPath\Project\output.json" -ignoredRules "ST-NMG-009,ST-DBP-020,UI-USG-011,ST-DBP-020"
    . 'C:\scripts\UiPathAnalyzeProject.ps1' "C:\UiPath\Project\project.json" -analyzerTraceLevel "Error" -stopOnRuleViolation true -treatWarningsAsErrors true -resultPath "C:\UiPath\Project\output.json" -ignoredRules "ST-NMG-009,ST-DBP-020,UI-USG-011,ST-DBP-020" -orchestratorUrl "https://orchestratorurl.com" -orchestratorTenant "default" -orchestratorUsername "username" -orchestratorPassword "\_ye5zG9(x" -orchestratorAuthToken "AuthToken" -orchestratorAccountName "AccountName" -orchestratorFolder "OrchestratorFolder"
    

#Note: if the script folder location is different, you need to replace "C:" with directory folder (e.g. '[FOLDER_VARIABLE]\scripts\UiPathPack.ps1')