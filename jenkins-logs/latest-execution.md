# Jenkins Execution Log

## Build Information
- **Job Name:** `MBP_Github_BlackduckSca_Sarif_Report/main`
- **Build Number:** #1
- **Build Status:** 🟢 **SUCCESS**
- **Duration:** 1 min 26 sec and counting
- **Timestamp:** 2025-11-11 17:10:17 UTC

---

## Console Output

```
Branch indexing
Connecting to https://api.github.com using madhusud@blackduck.com/****** (Github_Username_PAT)
Obtained nodejs-npm/Jenkinsfile from 238eb4e016bcb1d79954fd35bd4a236ea1ce01cd
Loading library blackduck-logs-publisher@main
Attempting to resolve main from remote references...
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git ls-remote -h -- https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
Found match: refs/heads/main revision e969196a63b1be83b84541b022f7aa52928bd5e5
The recommended git tool is: NONE
using credential Github_Username_PAT
Cloning the remote Git repository
Cloning with configured refspecs honoured and without tags
Cloning repository https://github.com/integrations-garage/blackduck-logs-publisher
 > git init /Users/madhusud/.jenkins/workspace/b_BlackduckSca_Sarif_Report_main@libs/a0dda568bac7bbb4a171f59ba3f2660c21c69edc6356524e9ae8bb4500c12bbb # timeout=10
Fetching upstream changes from https://github.com/integrations-garage/blackduck-logs-publisher
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/integrations-garage/blackduck-logs-publisher +refs/heads/*:refs/remotes/origin/* # timeout=10
 > git config remote.origin.url https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
 > git config --add remote.origin.fetch +refs/heads/*:refs/remotes/origin/* # timeout=10
Avoid second fetch
Checking out Revision e969196a63b1be83b84541b022f7aa52928bd5e5 (main)
 > git config core.sparsecheckout # timeout=10
 > git checkout -f e969196a63b1be83b84541b022f7aa52928bd5e5 # timeout=10
Commit message: "Phase 3 - 2"
First time build. Skipping changelog.
[Pipeline] Start of Pipeline
[Pipeline] node
Running on mac-sh in /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_BlackduckSca_Sarif_Report_main
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Declarative: Checkout SCM)
[Pipeline] checkout
The recommended git tool is: NONE
using credential Github_Username_PAT
Cloning the remote Git repository
Cloning with configured refspecs honoured and without tags
Cloning repository https://github.com/blackducksca-jenkins-samples/buildless-scan.git
 > git init /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_BlackduckSca_Sarif_Report_main # timeout=10
Fetching upstream changes from https://github.com/blackducksca-jenkins-samples/buildless-scan.git
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/blackducksca-jenkins-samples/buildless-scan.git +refs/heads/main:refs/remotes/origin/main # timeout=10
Avoid second fetch
Checking out Revision 238eb4e016bcb1d79954fd35bd4a236ea1ce01cd (main)
Commit message: "Jenkins log upload - Build #1"
First time build. Skipping changelog.
 > git config remote.origin.url https://github.com/blackducksca-jenkins-samples/buildless-scan.git # timeout=10
 > git config --add remote.origin.fetch +refs/heads/main:refs/remotes/origin/main # timeout=10
 > git config core.sparsecheckout # timeout=10
 > git checkout -f 238eb4e016bcb1d79954fd35bd4a236ea1ce01cd # timeout=10
[Pipeline] }
[Pipeline] // stage
[Pipeline] withEnv
[Pipeline] {
[Pipeline] stage
[Pipeline] { (blackduck-security-scan)
[Pipeline] script
[Pipeline] {
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_BlackduckSca_Sarif_Report_main/nodejs-npm
[Pipeline] {
[Pipeline] echo
DETECT_PROJECT_NAME will be set to: MBP_Github_BlackduckSca_Sarif_Report
[Pipeline] withEnv
[Pipeline] {
[Pipeline] security_scan
**************************** START EXECUTION OF BLACK DUCK SECURITY SCAN ****************************
[Security Scan] INFO: Jenkins Job name: MBP_Github_BlackduckSca_Sarif_Report
-------------------------------- Connection to node --------------------------------
[Security Scan] INFO: Jenkins job is running on agent node remotely
-------------------------- Parameter Validation Initiated --------------------------
[Security Scan] INFO:  --- product = [BLACKDUCKSCA]
[Security Scan] INFO: Parameters for blackducksca:
[Security Scan] INFO:  --- blackducksca_waitForScan = true
[Security Scan] INFO:  --- blackducksca_scan_full = true
[Security Scan] INFO:  --- blackducksca_token = ******************************************************************************
[Security Scan] INFO:  --- blackducksca_url = https://saastest.app.blackduck.com
------------------------------------------------------------------------------------
[Security Scan] INFO: Parameters for additional configuration:
[Security Scan] INFO:  --- mark_build_status = FAILURE
[Security Scan] INFO:  --- network_airgap = false
[Security Scan] INFO: Black Duck SCA parameters are validated successfully
[Security Scan] INFO: Bridge download parameters are validated successfully
[Security Scan] INFO: Bridge download is not required. Found installed in: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
------------------------------------------------------------------------------------
[Security Scan] INFO: Bridge CLI version is - 3.9.2
[Security Scan] INFO: Jenkins Job name: MBP_Github_BlackduckSca_Sarif_Report
[Security Scan] INFO: Jenkins Job name: MBP_Github_BlackduckSca_Sarif_Report
[Security Scan] INFO: Executable command line arguments: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm/bridge-cli --stage blackducksca --input /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_BlackduckSca_Sarif_Report_main/blackducksca_input12500039422273738661.json --out .bridge/output/scan_info_out.json

******************************* START EXECUTION OF BRIDGE CLI *******************************
2025-11-11 17:09:04.8221 IST [Bridge CLI] INFO: Using cache directory: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
2025-11-11 17:09:04.8273 IST [Bridge CLI] INFO: Found version "3.0.143" in registry for workflow "blackducksca", trying to load it from local cache
2025-11-11 17:09:04.9110 IST [Bridge CLI] INFO: Input Resources:
2025-11-11 17:09:04.9111 IST [Bridge CLI] INFO: resource = value [source]
2025-11-11 17:09:04.9111 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-11 17:09:04.9111 IST [Bridge CLI] INFO: blackducksca.scan.full = true [blackducksca_input12500039422273738661.json]
2025-11-11 17:09:04.9111 IST [Bridge CLI] INFO: blackducksca.token = ***************************************** [blackducksca_input12500039422273738661.json]
2025-11-11 17:09:04.9111 IST [Bridge CLI] INFO: blackducksca.url = https://saastest.app.blackduck.com [blackducksca_input12500039422273738661.json]
2025-11-11 17:09:04.9111 IST [Bridge CLI] INFO: blackducksca.waitForScan = true [blackducksca_input12500039422273738661.json]
2025-11-11 17:09:04.9111 IST [Bridge CLI] INFO: network.airgap = false [blackducksca_input12500039422273738661.json]
2025-11-11 17:09:04.9111 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-11 17:09:04.9111 IST [Bridge CLI] INFO: Starting adapters for stage blackducksca
2025-11-11 17:09:04.9114 IST [Bridge CLI] INFO: Starting Adapter: Blackduck SCA Controller
2025-11-11 17:09:04.9185 IST [Bridge CLI] INFO: Starting Adapter: Check pull request
2025-11-11 17:09:04.9432 IST [Check pull request] INFO: Provided value for resource 'environment.scan.pull'
2025-11-11 17:09:04.9434 IST [Check pull request] INFO: Adapter finished
2025-11-11 17:09:05.7739 IST [Blackduck SCA Controller] INFO: Found Black Duck SCA Detect jar file "detect-11.0.0.jar" in "/Users/madhusud/.blackduck/bridge/tools/blackduck-detect/11.0.0"
2025-11-11 17:09:05.7951 IST [Blackduck SCA Controller] INFO: Provided value for resource 'detect.execution.path'
2025-11-11 17:09:05.7952 IST [Bridge CLI] INFO: Starting adapters for stage blackducksca-detect
2025-11-11 17:09:05.7952 IST [Bridge CLI] INFO: Starting adapters for stage scm
2025-11-11 17:09:05.7952 IST [Bridge CLI] INFO: Starting adapters for stage blackducksca-post-processing
2025-11-11 17:09:05.7975 IST [Bridge CLI] INFO: Starting Adapter: Blackduck SCA Results
2025-11-11 17:09:05.7978 IST [Bridge CLI] INFO: Starting Adapter: SCM Checker
2025-11-11 17:09:05.7977 IST [Bridge CLI] INFO: Starting Adapter: Detect Component Locator
2025-11-11 17:09:05.7977 IST [Bridge CLI] INFO: Starting Adapter: Blackduck SCA Detect Execution
2025-11-11 17:09:05.7986 IST [Blackduck SCA Controller] INFO: Adapter finished
2025-11-11 17:09:05.8771 IST [Blackduck SCA Detect Execution] INFO: Running command /Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -jar /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/11.0.0/detect-11.0.0.jar --detect.cleanup=false --detect.bdio.file.name=scan --detect.bdio.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/b_BlackduckSca_Sarif_Report_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/bdio/blackduck_artifact --detect.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/b_BlackduckSca_Sarif_Report_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect --blackduck.offline.mode=false --blackduck.url=https://saastest.app.blackduck.com --blackduck.api.token= --detect.wait.for.results=true --detect.blackduck.scan.mode=INTELLIGENT
2025-11-11 17:09:06.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Detect-Self-Updater:  Checking https://saastest.app.blackduck.com/api/tools/detect API for centrally managed Detect version to download to /Users/madhusud/tmp.
2025-11-11 17:09:09.0000 IST [Blackduck SCA Detect Execution][main] WARNING: --- Detect-Self-Updater:  Unable to download jar from https://saastest.app.blackduck.com/api/tools/detect.
2025-11-11 17:09:09.0000 IST [Blackduck SCA Detect Execution][main] WARNING: --- Detect-Self-Updater:  Response code from https://saastest.app.blackduck.com/api/tools/detect was: 400 Bad Request
2025-11-11 17:09:09.9159 IST [Blackduck SCA Detect Execution] INFO: ______     _            _
2025-11-11 17:09:09.9159 IST [Blackduck SCA Detect Execution] INFO: |  _  \   | |          | |
2025-11-11 17:09:09.9160 IST [Blackduck SCA Detect Execution] INFO: | | | |___| |_ ___  ___| |_
2025-11-11 17:09:09.9160 IST [Blackduck SCA Detect Execution] INFO: | | | / _ \ __/ _ \/ __| __|
2025-11-11 17:09:09.9160 IST [Blackduck SCA Detect Execution] INFO: | |/ /  __/ ||  __/ (__| |_
2025-11-11 17:09:09.9160 IST [Blackduck SCA Detect Execution] INFO: |___/ \___|\__\___|\___|\__|
2025-11-11 17:09:09.9161 IST [Blackduck SCA Detect Execution] INFO: 
2025-11-11 17:09:10.0103 IST [Blackduck SCA Detect Execution] INFO: 
2025-11-11 17:09:10.0104 IST [Blackduck SCA Detect Execution] INFO: Detect Version: 11.0.0
2025-11-11 17:09:10.0104 IST [Blackduck SCA Detect Execution] INFO: 
2025-11-11 17:09:10.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 17:09:10.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Current property values:
2025-11-11 17:09:10.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- --property = value [notes]
2025-11-11 17:09:10.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ------------------------------------------------------------
2025-11-11 17:09:10.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- blackduck.api.token = **************************************************************************************************** [cmd] 
2025-11-11 17:09:10.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- blackduck.offline.mode = false [cmd] 
2025-11-11 17:09:10.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- blackduck.url = https://saastest.app.blackduck.com [cmd] 
2025-11-11 17:09:10.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.bdio.file.name = scan [cmd] 
2025-11-11 17:09:10.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.bdio.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_BlackduckSca_Sarif_Report_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/bdio/blackduck_artifact [cmd] 
2025-11-11 17:09:10.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.blackduck.scan.mode = INTELLIGENT [cmd] 
2025-11-11 17:09:10.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.cleanup = false [cmd] 
2025-11-11 17:09:10.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.excluded.directories = /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_BlackduckSca_Sarif_Report_main/nodejs-npm/.bridge [env] 
2025-11-11 17:09:10.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_BlackduckSca_Sarif_Report_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect [cmd] 
2025-11-11 17:09:10.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.project.name = MBP_Github_BlackduckSca_Sarif_Report [env] 
2025-11-11 17:09:10.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.wait.for.results = true [cmd] 
2025-11-11 17:09:10.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ------------------------------------------------------------
2025-11-11 17:09:10.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 17:09:10.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Detect build date: 2025-10-30
2025-11-11 17:09:10.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Source directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_BlackduckSca_Sarif_Report_main/nodejs-npm
2025-11-11 17:09:10.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Output directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_BlackduckSca_Sarif_Report_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect
2025-11-11 17:09:10.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Run directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_BlackduckSca_Sarif_Report_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/runs/2025-11-11-11-39-10-001
2025-11-11 17:09:10.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 17:09:16.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Successfully connected to Black Duck SCA (version 2025.7.1)!
2025-11-11 17:09:17.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 17:09:17.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Will include the Docker tool.
2025-11-11 17:09:17.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Docker actions finished.
2025-11-11 17:09:17.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 17:09:17.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Will include the Bazel tool.
2025-11-11 17:09:17.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Bazel actions finished.
2025-11-11 17:09:17.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 17:09:17.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Will include the Detectors tool.
2025-11-11 17:09:17.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Searching for detectors.
2025-11-11 17:09:17.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Evaluating detectors. This may take a while.
2025-11-11 17:09:17.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ======================================================================================================
2025-11-11 17:09:17.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Detector Report
2025-11-11 17:09:17.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ======================================================================================================
2025-11-11 17:09:17.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 	/Users/madhusud/Jenkins_Testing/Nodes/workspace/b_BlackduckSca_Sarif_Report_main/nodejs-npm (depth 0)
2025-11-11 17:09:17.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 		NPM Package Lock: SUCCESS
2025-11-11 17:09:17.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_BlackduckSca_Sarif_Report_main/nodejs-npm/package-lock.json
2025-11-11 17:09:17.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_BlackduckSca_Sarif_Report_main/nodejs-npm/package.json
2025-11-11 17:09:17.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 17:09:17.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Detectors actions finished.
2025-11-11 17:09:17.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 17:09:17.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Project name: MBP_Github_BlackduckSca_Sarif_Report
2025-11-11 17:09:17.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Project version: 1.3.0
2025-11-11 17:09:18.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- The MBP_Github_BlackduckSca_Sarif_Report project was not found, so it will be created - if a version was included, it will also be created.
2025-11-11 17:09:23.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Successfully completed package manager scan of file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_BlackduckSca_Sarif_Report_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/bdio/blackduck_artifact/scan.bdio
2025-11-11 17:09:25.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Starting the codelocation file uploads.
2025-11-11 17:09:29.0000 IST [Blackduck SCA Detect Execution][pool-1-thread-1] INFO: --- Try #1 for task bdio upload (elapsed: 00:00:00.000)...complete!
2025-11-11 17:09:29.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Completed the codelocation file uploads.
2025-11-11 17:09:29.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 17:09:29.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Will include the Signature Scanner tool.
2025-11-11 17:09:29.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- No metadata file exists, assuming this is new installation and the signature scanner should be downloaded.
2025-11-11 17:09:32.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Downloading the Black Duck Signature Scanner.
2025-11-11 17:09:32.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- If the Signature Scanner on your Black Duck server has changed, the contents of /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_BlackduckSca_Sarif_Report_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/tools/Black_Duck_Scan_Installation may change which could involve deleting files - please do not place items in the expansion directory as this directory is assumed to be under blackduck-common control.
2025-11-11 17:09:40.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Black Duck Signature Scanner downloaded successfully.
2025-11-11 17:09:40.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- The Black Duck Signature Scanner downloaded/found successfully: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_BlackduckSca_Sarif_Report_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/tools
2025-11-11 17:09:40.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- No scan targets provided - registering the source path /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_BlackduckSca_Sarif_Report_main/nodejs-npm to scan
2025-11-11 17:09:42.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Starting the Black Duck Signature Scan commands.
2025-11-11 17:09:42.0000 IST [Blackduck SCA Detect Execution][pool-3-thread-1] INFO: --- Black Duck CLI command: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_BlackduckSca_Sarif_Report_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/tools/Black_Duck_Scan_Installation/scan.cli-1.0.6/jre/Contents/Home/bin/java -Done-jar.silent=true -Done-jar.jar.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/b_BlackduckSca_Sarif_Report_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/tools/Black_Duck_Scan_Installation/scan.cli-1.0.6/lib/cache/scan.cli.impl-standalone.jar -Xmx4096m -jar /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_BlackduckSca_Sarif_Report_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/tools/Black_Duck_Scan_Installation/scan.cli-1.0.6/lib/scan.cli-1.0.6-standalone.jar --no-prompt --scheme https --host saastest.app.blackduck.com --port 443 -v --logDir /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_BlackduckSca_Sarif_Report_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/runs/2025-11-11-11-39-10-001/scan/BlackDuckScanOutput/2025-11-11_11-39-42-077_1 --statusWriteDir /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_BlackduckSca_Sarif_Report_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/runs/2025-11-11-11-39-10-001/scan/BlackDuckScanOutput/2025-11-11_11-39-42-077_1 --project MBP_Github_BlackduckSca_Sarif_Report --release 1.3.0 --name nodejs-npm/MBP_Github_BlackduckSca_Sarif_Report/1.3.0 signature --exclude /.bridge/ --scass-scan /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_BlackduckSca_Sarif_Report_main/nodejs-npm
2025-11-11 17:09:56.0000 IST [Blackduck SCA Detect Execution][pool-3-thread-1] INFO: --- 
2025-11-11 17:09:56.0000 IST [Blackduck SCA Detect Execution][pool-3-thread-1] INFO: --- Black Duck Signature Scanner return code: 0
2025-11-11 17:09:56.0000 IST [Blackduck SCA Detect Execution][pool-3-thread-1] INFO: --- Signature Scanner log output directory: '/Users/madhusud/Jenkins_Testing/Nodes/workspace/b_BlackduckSca_Sarif_Report_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/runs/2025-11-11-11-39-10-001/scan/BlackDuckScanOutput/2025-11-11_11-39-42-077_1'
2025-11-11 17:09:56.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Completed the Black Duck Signature Scan commands.
2025-11-11 17:09:56.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Signature Scanner actions finished.
2025-11-11 17:09:56.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 17:09:56.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Will include the Binary Scanner tool.
2025-11-11 17:09:56.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Binary scanner found nothing to upload.
2025-11-11 17:09:56.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Binary Scanner actions finished.
2025-11-11 17:09:56.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 17:09:56.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Will include the Container Scanner tool.
2025-11-11 17:09:56.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- No detect.container.scan.file.path property was provided. Skipping container scan.
2025-11-11 17:09:56.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Container Scanner actions finished.
2025-11-11 17:09:56.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 17:09:56.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Vulnerability Impact Analysis tool will not be run.
2025-11-11 17:09:56.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 17:09:56.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- IaC Scanner tool will not be run.
2025-11-11 17:09:56.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 17:09:56.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Try #1 for task BOM Scan Wait Job https://saastest.app.blackduck.com/api/projects/1de6d2c9-ce42-424c-8582-5e87a2a114ff/versions/31b397c3-7a73-4de6-84e2-0fdb7b89ea87/bom-status/16531a26-29d6-40d5-bd95-18128bb57af4 (elapsed: 00:00:00.000)...not done yet, waiting 1 seconds and trying again...
2025-11-11 17:09:58.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Try #2 for task BOM Scan Wait Job https://saastest.app.blackduck.com/api/projects/1de6d2c9-ce42-424c-8582-5e87a2a114ff/versions/31b397c3-7a73-4de6-84e2-0fdb7b89ea87/bom-status/16531a26-29d6-40d5-bd95-18128bb57af4 (elapsed: 00:00:01.752)...not done yet, waiting 2 seconds and trying again...
2025-11-11 17:10:01.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Try #3 for task BOM Scan Wait Job https://saastest.app.blackduck.com/api/projects/1de6d2c9-ce42-424c-8582-5e87a2a114ff/versions/31b397c3-7a73-4de6-84e2-0fdb7b89ea87/bom-status/16531a26-29d6-40d5-bd95-18128bb57af4 (elapsed: 00:00:04.541)...not done yet, waiting 3 seconds and trying again...
2025-11-11 17:10:05.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Try #4 for task BOM Scan Wait Job https://saastest.app.blackduck.com/api/projects/1de6d2c9-ce42-424c-8582-5e87a2a114ff/versions/31b397c3-7a73-4de6-84e2-0fdb7b89ea87/bom-status/16531a26-29d6-40d5-bd95-18128bb57af4 (elapsed: 00:00:08.318)...not done yet, waiting 5 seconds and trying again...
2025-11-11 17:10:11.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Try #5 for task BOM Scan Wait Job https://saastest.app.blackduck.com/api/projects/1de6d2c9-ce42-424c-8582-5e87a2a114ff/versions/31b397c3-7a73-4de6-84e2-0fdb7b89ea87/bom-status/16531a26-29d6-40d5-bd95-18128bb57af4 (elapsed: 00:00:14.082)...complete!
2025-11-11 17:10:11.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Try #1 for task BOM Scan Wait Job https://saastest.app.blackduck.com/api/projects/1de6d2c9-ce42-424c-8582-5e87a2a114ff/versions/31b397c3-7a73-4de6-84e2-0fdb7b89ea87/bom-status/fd1e6943-35a1-4ab8-b14a-cbf924ccc835 (elapsed: 00:00:00.000)...complete!
2025-11-11 17:10:11.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Checking to see if Detect should check policy for violations.
2025-11-11 17:10:12.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 17:10:12.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 17:10:12.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Creating status file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_BlackduckSca_Sarif_Report_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/runs/2025-11-11-11-39-10-001/status/status.json
2025-11-11 17:10:12.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 17:10:12.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Skipping cleanup, it is disabled.
2025-11-11 17:10:13.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 17:10:13.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 17:10:13.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ======== Detect Result ========
2025-11-11 17:10:13.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 17:10:13.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Black Duck SCA Project BOM: https://saastest.app.blackduck.com/api/projects/1de6d2c9-ce42-424c-8582-5e87a2a114ff/versions/31b397c3-7a73-4de6-84e2-0fdb7b89ea87/components
2025-11-11 17:10:13.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 17:10:13.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ======== Detect Status ========
2025-11-11 17:10:13.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 17:10:13.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- NPM: SUCCESS
2025-11-11 17:10:13.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 17:10:13.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Signature scan / Snippet scan on /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_BlackduckSca_Sarif_Report_main/nodejs-npm: SUCCESS
2025-11-11 17:10:13.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Overall Status: SUCCESS - Detect exited successfully.
2025-11-11 17:10:13.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 17:10:13.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ===============================
2025-11-11 17:10:13.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 17:10:13.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Detect duration: 00h 01m 06s 991ms
2025-11-11 17:10:13.3677 IST [Blackduck SCA Detect Execution] INFO: Provided value for resource 'detect.completed'
2025-11-11 17:10:13.3678 IST [Blackduck SCA Detect Execution] INFO: Provided value for resource 'detect.results.path'
2025-11-11 17:10:13.3680 IST [Blackduck SCA Detect Execution] INFO: Adapter finished
2025-11-11 17:10:13.4040 IST [Blackduck SCA Results] INFO: Skipping Blackduck SCA issues retrieval as "blackducksca.fixpr.enabled" is configured to false
2025-11-11 17:10:13.4094 IST [Blackduck SCA Results] INFO: Adapter finished
2025-11-11 17:10:13.4545 IST [SCM Checker] INFO: Provided value for resource 'jenkins.enabled'
2025-11-11 17:10:13.4545 IST [Bridge CLI] INFO: Starting adapters for stage blackducksca-policy-violations-fetcher
2025-11-11 17:10:13.4550 IST [Bridge CLI] INFO: Starting Adapter: Blackduck SCA Policy Violations Fetcher
2025-11-11 17:10:13.4551 IST [SCM Checker] INFO: Adapter finished
2025-11-11 17:10:13.4972 IST [Detect Component Locator] INFO: skipping fix pull requests creation as "blackducksca.fixpr.enabled" is configured to false
2025-11-11 17:10:13.5022 IST [Detect Component Locator] INFO: Adapter finished
2025-11-11 17:10:13.9114 IST [Blackduck SCA Policy Violations Fetcher] INFO: Detected Intelligent scan, will fetch Intelligent scan policy violations data
2025-11-11 17:10:14.8865 IST [Blackduck SCA Policy Violations Fetcher] INFO: Bearer token retrieved successfully
2025-11-11 17:10:15.2387 IST [Blackduck SCA Policy Violations Fetcher] INFO: Project data retrieved successfully
2025-11-11 17:10:15.6172 IST [Blackduck SCA Policy Violations Fetcher] INFO: Version data retrieved successfully
2025-11-11 17:10:15.9764 IST [Blackduck SCA Policy Violations Fetcher] INFO: Detected 5 policy violations
2025-11-11 17:10:16.3367 IST [Blackduck SCA Policy Violations Fetcher] INFO: Added entry to resource 'blackducksca.policy.rules.violations'
2025-11-11 17:10:16.3369 IST [Blackduck SCA Policy Violations Fetcher] INFO: Provided value for resource 'blackducksca.policy.status.issues.critical'
2025-11-11 17:10:16.3371 IST [Blackduck SCA Policy Violations Fetcher] INFO: Provided value for resource 'blackducksca.policy.status.issues.ok'
2025-11-11 17:10:16.3372 IST [Blackduck SCA Policy Violations Fetcher] INFO: Provided value for resource 'blackducksca.policy.status.issues.unspecified'
2025-11-11 17:10:16.3373 IST [Blackduck SCA Policy Violations Fetcher] INFO: Provided value for resource 'blackducksca.policy.status.issues.blocker'
2025-11-11 17:10:16.3374 IST [Blackduck SCA Policy Violations Fetcher] INFO: Provided value for resource 'blackducksca.policy.status.issues.major'
2025-11-11 17:10:16.3375 IST [Blackduck SCA Policy Violations Fetcher] INFO: Provided value for resource 'blackducksca.policy.status.issues.minor'
2025-11-11 17:10:16.3376 IST [Blackduck SCA Policy Violations Fetcher] INFO: Provided value for resource 'blackducksca.policy.status.issues.trivial'
2025-11-11 17:10:16.3377 IST [Blackduck SCA Policy Violations Fetcher] INFO: Provided value for resource 'blackducksca.projectBomUrl'
2025-11-11 17:10:16.3380 IST [Blackduck SCA Policy Violations Fetcher] INFO: Adapter finished
******************************* END EXECUTION OF BRIDGE CLI *******************************
[Security Scan] INFO: Retrieving the issue count from the scan results
[Security Scan] INFO: Total issues found: 1095
[Security Scan] INFO: Security Scan execution is successful
[Security Scan] INFO: Marking build status as FAILURE is ignored since exit code is: 0
**************************** END EXECUTION OF BLACK DUCK SECURITY SCAN ****************************
[Pipeline] }
[Pipeline] // withEnv
[Pipeline] }
[Pipeline] // dir
[Pipeline] }
[Pipeline] // script
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (Declarative: Post Actions)
[Pipeline] echo
Black Duck Logs Publisher - Starting log upload process
[Pipeline] echo
Configuration: [githubOrg:blackducksca-jenkins-samples, repoName:buildless-scan, credentialsId:github-pat-logs-publisher, maxRetries:3, retentionCount:5, jobNamePrefixes:[MBP_Github_, MBP_, Github_, Pipeline_, Job_, Build_]]
[Pipeline] echo
Job Name: MBP_Github_BlackduckSca_Sarif_Report/main
[Pipeline] echo
Build Number: 1
[Pipeline] echo
GitHub Organization: blackducksca-jenkins-samples
[Pipeline] withCredentials
Masking supported pattern matches of $GITHUB_TOKEN
[Pipeline] {
[Pipeline] echo
Using configured repository name: buildless-scan
[Pipeline] echo
Target repository: blackducksca-jenkins-samples/buildless-scan
[Pipeline] echo
LogProcessor: captureJenkinsLogs called
```

---

*Log generated by Black Duck Logs Publisher*