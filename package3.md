
Goal by Tuesday 16th is to produce documents for the following areas:
- Tool qualification
- Development process descriptions
- Supplier documents
- ? Manufacturing process
- ? Post-release process descriptions
- ? Plans for software verification/validation

# TOC <!-- omit in toc -->
- [Tool qualification](#tool-qualification)
  - [Steps to follow](#steps-to-follow)
  - [Tools to qualify](#tools-to-qualify)
- [Plans and Process Descriptions](#plans-and-process-descriptions)
- [Risk management](#risk-management)
- [Outsourcing](#outsourcing)
- [Package 4](#package-4)

# Tool qualification

Regulatory guidance: [ISO-TR 80002-2 Medical device software - Part 2 Validation of Software for Medical Device Quality Systems](https://pulseonfi.sharepoint.com/sites/medical/_layouts/15/DocIdRedir.aspx?ID=PODMS-942620546-2376)

## Steps to follow

There is a Jira project [Equipment & SW Qualification](https://pulseon.atlassian.net/secure/RapidBoard.jspa?rapidView=45) for storing the SW Qualification requirements and testing information. Each tool has a component assigned and a corresponding Kanban board.

Select the Kanban board from the left side.

When creating a Jira issue (Requirement, Story, Test, etc.) for each tool, remember to select the correct component for the tool, otherwise the issue will not appear on the board. If you "lose" the issue, you can always find it by going to the Issues view, also from the left toolbar, where you can filter the issues by Reporter.

On the Sharepoint documentation side, there are 3 documents that need to be created:
- The Type Qualification Form (template [PODMS-686774966-4216](https://pulseonfi.sharepoint.com/sites/medical/_layouts/15/DocIdRedir.aspx?ID=PODMS-686774966-4216)), which includes the Design Qualification. This is one document per tool.
- The Item Qualification Form (template [PODMS-686774966-4215](https://pulseonfi.sharepoint.com/sites/medical/_layouts/15/DocIdRedir.aspx?ID=PODMS-686774966-4215)), which includes the Installation Qualification, Operational and Performance Qualification. One document per installation is required.
- The Maintenance Register (template [PODMS-686774966-4168](https://pulseonfi.sharepoint.com/sites/medical/_layouts/15/DocIdRedir.aspx?ID=PODMS-686774966-4168)). One document per installation is required. Note that there is a bug in the template, in column R ("IC?") which should be a Yes/No column, rather than Passed/Failed column. It's fixed in the Jenkins drafts below.

If you plan to use Xray and Jira, you can check, as an example, the drafts I created for Jenkins in Sharepoint, under:
`Medical > Resource Management > Software > Continuous Integration > Jenkins > Qualification`

HINTS:
- Define only minimal number of requirements
- Don't list all the features, just the **absolutely necessary** ones

## Tools to qualify
- [x] Adrian: Xray
- [ ] Tuomas: Matlab and Matlab scripts
- [ ] Ole: Data synchronization Python scripts
- [ ] Adrian: Jenkins
- [ ] Kuisma: GNU Arm Embedded Toolchain
- [ ] Balaz: Segger J-Link
- [ ] Marko: Jira
  - Used for defect management, project management
  - What records does Jira produce for these that are part of QMS?
    - Anomaly reports
- [ ] Jukka: Git
- [ ] GitHub
- [ ] Python3 and packages
- [ ] Factory testing tools (qualified as part of factory testing process and not individually)
  - [ ] pts_client.py, ftsclient.py, settingsclient.py
  - [ ] combo_image.py, factory_image.py
  - [ ] afe_config.py
  - [ ] decoder (own software that is verified)
- [ ] R&D script tools
  - [ ] aino_plot_data.py
  - [ ] visclient.py, scs_client.py
  - [ ] clinical_session.sh
  - [ ] sanity_check.py (include more checks for etc WARNING or ERROR messages)

# Plans and Process Descriptions
- [x] [PODMS-782466528-20](https://pulseonfi.sharepoint.com/sites/medical/_layouts/15/DocIdRedir.aspx?ID=PODMS-782466528-20) — Aino Software Development Plan
- [ ] Adrian: [PODMS-1378432600-5404](https://pulseonfi.sharepoint.com/sites/medical/_layouts/15/DocIdRedir.aspx?ID=PODMS-1378432600-5404) — Aino WD Software Test Plan
- [ ] Marko?: Aino Software Test Plan (see Aino Design Verification Plan PODMS-1378432600-918)
- [ ] Package 4? Software Verification Plan
- [ ] Package 4? [PODMS-1378432600-3674](https://pulseonfi.sharepoint.com/sites/medical/_layouts/15/DocIdRedir.aspx?ID=PODMS-1378432600-3674) — Firmware release process
- [ ] Package 4? [PODMS-1378432600-5349](https://pulseonfi.sharepoint.com/sites/medical/_layouts/15/DocIdRedir.aspx?ID=PODMS-1378432600-5349) — Anomaly Lifecycle Process (part of Non-Conforming Product Procedure) 

# Risk management
- [ ] Marko: [PODMS-1416440729-2836](https://pulseonfi.sharepoint.com/sites/medical/_layouts/15/DocIdRedir.aspx?ID=PODMS-1416440729-2836) Aino Risk Management Register

# Outsourcing
- [x] [PODMS-477950017-4343](https://pulseonfi.sharepoint.com/sites/medical/_layouts/15/DocIdRedir.aspx?ID=PODMS-477950017-4343) DMS URS
- [x] [PODMS-477950017-4345](https://pulseonfi.sharepoint.com/sites/medical/_layouts/15/DocIdRedir.aspx?ID=PODMS-477950017-4345) Win app URS
- [x] [PODMS-477950017-4343](https://pulseonfi.sharepoint.com/sites/medical/_layouts/15/DocIdRedir.aspx?ID=PODMS-1378432600-5349) Gateway URS

# Package 4
- [ ] Aino Unit Verification Procedure
- [ ] Aino Unit Verification Report(s)
- [ ] Aino SW Unit Integration Test Plan(s)
- [ ] Aino SW Unit Integration Test Data
- [ ] Aino SW Unit Integration Test Report(s)
- [ ] Aino SW Identifier Verification Record
- [ ] Aino Design Verification Report