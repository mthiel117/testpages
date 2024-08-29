# Validate State Report

**Table of Contents:**

- [Validate State Report](validate-state-report)
  - [Test Results Summary](#test-results-summary)
  - [Failed Test Results Summary](#failed-test-results-summary)
  - [All Test Results](#all-test-results)

## Test Results Summary

### Summary Totals

| Total Tests | Total Tests Passed | Total Tests Failed | Total Tests Skipped |
| ----------- | ------------------ | ------------------ | ------------------- |
| 918 | 845 | 99 | 73 |

### Summary Totals Device Under Test

| Device Under Test | Total Tests | Tests Passed | Tests Failed | Tests Skipped | Categories Failed | Categories Skipped |
| ------------------| ----------- | ------------ | ------------ | ------------- | ----------------- | ------------------ |
| HRAO-CORE-1 | 56 | 52 | 0 | 4 | - | Hardware |
| HRAO-CORE-10 | 56 | 52 | 0 | 4 | - | Hardware |
| HRAOISD1-1-0 | 78 | 74 | 0 | 4 | - | Hardware |
| HRAOISD1-1-1 | 78 | 74 | 0 | 4 | - | Hardware |
| HRAOISD1-1-2 | 68 | 61 | 0 | 7 | - | Hardware, MLAG |
| HRAOISD1-1-3 | 68 | 61 | 0 | 7 | - | Hardware, MLAG |
| HRAOISD2-1-0 | 87 | 83 | 0 | 4 | - | Hardware |
| HRAOISD2-1-1 | 87 | 83 | 0 | 4 | - | Hardware |
| HRAOISD2-1-2 | 68 | 61 | 0 | 7 | - | Hardware, MLAG |
| HRAOISD2-1-3 | 68 | 61 | 0 | 7 | - | Hardware, MLAG |
| HRAOISD2-1-4 | 68 | 61 | 0 | 7 | - | Hardware, MLAG |
| HRAOISD2-1-5 | 68 | 61 | 0 | 7 | - | Hardware, MLAG |
| HRAOISD2-1-6 | 68 | 61 | 0 | 7 | - | Hardware, MLAG |

### Summary Totals Per Category

| Test Category | Total Tests | Tests Passed | Tests Failed | Tests Skipped |
| ------------- | ----------- | ------------ | ------------ | ------------- |
| Configuration | 26 | 26 | 0 | 0 |
| Connectivity | 59 | 59 | 0 | 0 |
| Hardware | 52 | 0 | 0 | 52 |
| Interfaces | 690 | 690 | 0 | 0 |
| MLAG | 39 | 18 | 0 | 21 |
| Routing | 13 | 13 | 0 | 0 |
| Software | 26 | 26 | 0 | 0 |
| System | 13 | 13 | 0 | 0 |

## Failed Test Results Summary

| ID | Device Under Test | Categories | Test | Description | Inputs | Result | Messages |
| -- | ----------------- | ---------- | ---- | ----------- | ------ | -------| -------- |

## All Test Results

| ID | Device Under Test | Categories | Test | Description | Inputs | Result | Messages |
| -- | ----------------- | ---------- | ---- | ----------- | ------ | -------| -------- |
| 1 | HRAO-CORE-1 | Configuration | VerifyRunningConfigDiffs | Verifies there is no difference between the running-config and the startup-config | - | PASS | - |
| 2 | HRAO-CORE-1 | Configuration | VerifyZeroTouch | Verifies ZeroTouch is disabled | - | PASS | - |
| 3 | HRAO-CORE-1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet103/1 - Remote: HRAO-CORE-10 Ethernet103/1 | PASS | - |
| 4 | HRAO-CORE-1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet104/1 - Remote: HRAO-CORE-10 Ethernet104/1 | PASS | - |
| 5 | HRAO-CORE-1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet5 - Remote: HRAOISD2-1-0 Ethernet49 | PASS | - |
| 6 | HRAO-CORE-1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet6 - Remote: HRAOISD1-1-0 Ethernet49 | PASS | - |
| 7 | HRAO-CORE-1 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on vEOS-lab. |
| 8 | HRAO-CORE-1 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on vEOS-lab. |
| 9 | HRAO-CORE-1 | Hardware | VerifyTemperature | Verifies the device temperature. | - | SKIPPED | VerifyTemperature test is not supported on vEOS-lab. |
| 10 | HRAO-CORE-1 | Hardware | VerifyTransceiversManufacturers | Verifies if all transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on vEOS-lab. |
| 11 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet101/1 - Juniper-Cores_xe1/2/0 = 'up' | PASS | - |
| 12 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet102/1 - Juniper-Cores_xe1/2/1 = 'up' | PASS | - |
| 13 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet103/1 - MLAG_PEER_HRAO-CORE-10_Ethernet103/1 = 'up' | PASS | - |
| 14 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet104/1 - MLAG_PEER_HRAO-CORE-10_Ethernet104/1 = 'up' | PASS | - |
| 15 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet5 - HRAOISD2-1-0_Ethernet49 = 'up' | PASS | - |
| 16 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet6 - HRAOISD1-1-0_Ethernet49 = 'up' | PASS | - |
| 17 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Loopback0 - Router_ID = 'up' | PASS | - |
| 18 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel1011 - Juniper-Cores = 'up' | PASS | - |
| 19 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel1031 - MLAG_PEER_HRAO-CORE-10_Po1031 = 'up' | PASS | - |
| 20 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel5 - ISD2-SPINES_Po49 = 'up' | PASS | - |
| 21 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel6 - ISD1-SPINES_Po49 = 'up' | PASS | - |
| 22 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan154 - 154_isd1-1-core2_172.16.13.97/29 = 'adminDown' | PASS | - |
| 23 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan155 - 155_isd2-1-core2_172.16.13.105/29 = 'adminDown' | PASS | - |
| 24 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan1600 - 1600_voice-isd1-1_172.16.164.62/26 = 'adminDown' | PASS | - |
| 25 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan1602 - 1602_voice-isd2-1_172.16.138.126/25 = 'adminDown' | PASS | - |
| 26 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan200 - 200_wireless_172.16.207.254/21 = 'adminDown' | PASS | - |
| 27 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan202 - 202_wireless2_172.16.183.254/21 = 'adminDown' | PASS | - |
| 28 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan2200 - 2200_camera-bldg2_172.16.69.78/28 = 'adminDown' | PASS | - |
| 29 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan2201 - 2201_camera-bldg3_172.16.69.158/28 = 'adminDown' | PASS | - |
| 30 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan2202 - 2202_camera-bldg3a_172.16.69.174/28 = 'adminDown' | PASS | - |
| 31 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan2203 - 2203_camera-bldg7_172.16.69.190/28 = 'adminDown' | PASS | - |
| 32 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan2204 - 2204_camera-bldg8_172.16.68.222/27 = 'adminDown' | PASS | - |
| 33 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan2205 - 2205_camera-bldg5-dyno_172.16.68.30/27 = 'adminDown' | PASS | - |
| 34 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan2206 - 2206_camera-bldg13-dyno_172.16.68.62/27 = 'adminDown' | PASS | - |
| 35 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan2508 - 2508_cam-isd1_10.107.64.254/27 = 'adminDown' | PASS | - |
| 36 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan2600 - 2600_fac-isd_10.107.80.94/27 = 'adminDown' | PASS | - |
| 37 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan4093 - MLAG_PEER_L3_PEERING = 'up' | PASS | - |
| 38 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan4094 - MLAG_PEER = 'up' | PASS | - |
| 39 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan5 - Inband Management = 'adminDown' | PASS | - |
| 40 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan600 - 600_isd-a_172.16.240.254/24 = 'adminDown' | PASS | - |
| 41 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan601 - 601_isd-b_172.16.241.254/24 = 'adminDown' | PASS | - |
| 42 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan602 - 602_isd-c_172.16.242.254/24 = 'adminDown' | PASS | - |
| 43 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan603 - 603_isd-d_172.16.243.254/24 = 'adminDown' | PASS | - |
| 44 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan629 - 629_closet10-c_172.16.154.254/24 = 'adminDown' | PASS | - |
| 45 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan681 - 681_dot212_172.16.212.254/24 = 'adminDown' | PASS | - |
| 46 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan682 - 682_dot220_172.16.220.254/24 = 'adminDown' | PASS | - |
| 47 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan703 - 703_pcaim_172.16.3.254/24 = 'adminDown' | PASS | - |
| 48 | HRAO-CORE-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan704 - 704_security_172.16.4.254/24 = 'adminDown' | PASS | - |
| 49 | HRAO-CORE-1 | Interfaces | VerifyLoopbackCount | Verifies the number of loopback interfaces and their status. | - | PASS | - |
| 50 | HRAO-CORE-1 | MLAG | VerifyMlagConfigSanity | Verifies there are no MLAG config-sanity inconsistencies. | - | PASS | - |
| 51 | HRAO-CORE-1 | MLAG | VerifyMlagInterfaces | Verifies there are no inactive or active-partial MLAG ports. | - | PASS | - |
| 52 | HRAO-CORE-1 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 53 | HRAO-CORE-1 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | - | PASS | - |
| 54 | HRAO-CORE-1 | Software | VerifyEOSVersion | Verifies the EOS version of the device. | - | PASS | - |
| 55 | HRAO-CORE-1 | Software | VerifyTerminAttrVersion | Verifies the TerminAttr version of the device. | - | PASS | - |
| 56 | HRAO-CORE-1 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | PASS | - |
| 57 | HRAO-CORE-10 | Configuration | VerifyRunningConfigDiffs | Verifies there is no difference between the running-config and the startup-config | - | PASS | - |
| 58 | HRAO-CORE-10 | Configuration | VerifyZeroTouch | Verifies ZeroTouch is disabled | - | PASS | - |
| 59 | HRAO-CORE-10 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet103/1 - Remote: HRAO-CORE-1 Ethernet103/1 | PASS | - |
| 60 | HRAO-CORE-10 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet104/1 - Remote: HRAO-CORE-1 Ethernet104/1 | PASS | - |
| 61 | HRAO-CORE-10 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet5 - Remote: HRAOISD2-1-1 Ethernet49 | PASS | - |
| 62 | HRAO-CORE-10 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet6 - Remote: HRAOISD1-1-1 Ethernet49 | PASS | - |
| 63 | HRAO-CORE-10 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on vEOS-lab. |
| 64 | HRAO-CORE-10 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on vEOS-lab. |
| 65 | HRAO-CORE-10 | Hardware | VerifyTemperature | Verifies the device temperature. | - | SKIPPED | VerifyTemperature test is not supported on vEOS-lab. |
| 66 | HRAO-CORE-10 | Hardware | VerifyTransceiversManufacturers | Verifies if all transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on vEOS-lab. |
| 67 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet101/1 - Juniper-Cores_xe1/2/0 = 'up' | PASS | - |
| 68 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet102/1 - Juniper-Cores_xe1/2/1 = 'up' | PASS | - |
| 69 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet103/1 - MLAG_PEER_HRAO-CORE-1_Ethernet103/1 = 'up' | PASS | - |
| 70 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet104/1 - MLAG_PEER_HRAO-CORE-1_Ethernet104/1 = 'up' | PASS | - |
| 71 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet5 - HRAOISD2-1-1_Ethernet49 = 'up' | PASS | - |
| 72 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet6 - HRAOISD1-1-1_Ethernet49 = 'up' | PASS | - |
| 73 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Loopback0 - Router_ID = 'up' | PASS | - |
| 74 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel1011 - Juniper-Cores = 'up' | PASS | - |
| 75 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel1031 - MLAG_PEER_HRAO-CORE-1_Po1031 = 'up' | PASS | - |
| 76 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel5 - ISD2-SPINES_Po49 = 'up' | PASS | - |
| 77 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel6 - ISD1-SPINES_Po49 = 'up' | PASS | - |
| 78 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan154 - 154_isd1-1-core2_172.16.13.97/29 = 'adminDown' | PASS | - |
| 79 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan155 - 155_isd2-1-core2_172.16.13.105/29 = 'adminDown' | PASS | - |
| 80 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan1600 - 1600_voice-isd1-1_172.16.164.62/26 = 'adminDown' | PASS | - |
| 81 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan1602 - 1602_voice-isd2-1_172.16.138.126/25 = 'adminDown' | PASS | - |
| 82 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan200 - 200_wireless_172.16.207.254/21 = 'adminDown' | PASS | - |
| 83 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan202 - 202_wireless2_172.16.183.254/21 = 'adminDown' | PASS | - |
| 84 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan2200 - 2200_camera-bldg2_172.16.69.78/28 = 'adminDown' | PASS | - |
| 85 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan2201 - 2201_camera-bldg3_172.16.69.158/28 = 'adminDown' | PASS | - |
| 86 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan2202 - 2202_camera-bldg3a_172.16.69.174/28 = 'adminDown' | PASS | - |
| 87 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan2203 - 2203_camera-bldg7_172.16.69.190/28 = 'adminDown' | PASS | - |
| 88 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan2204 - 2204_camera-bldg8_172.16.68.222/27 = 'adminDown' | PASS | - |
| 89 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan2205 - 2205_camera-bldg5-dyno_172.16.68.30/27 = 'adminDown' | PASS | - |
| 90 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan2206 - 2206_camera-bldg13-dyno_172.16.68.62/27 = 'adminDown' | PASS | - |
| 91 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan2508 - 2508_cam-isd1_10.107.64.254/27 = 'adminDown' | PASS | - |
| 92 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan2600 - 2600_fac-isd_10.107.80.94/27 = 'adminDown' | PASS | - |
| 93 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan4093 - MLAG_PEER_L3_PEERING = 'up' | PASS | - |
| 94 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan4094 - MLAG_PEER = 'up' | PASS | - |
| 95 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan5 - Inband Management = 'adminDown' | PASS | - |
| 96 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan600 - 600_isd-a_172.16.240.254/24 = 'adminDown' | PASS | - |
| 97 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan601 - 601_isd-b_172.16.241.254/24 = 'adminDown' | PASS | - |
| 98 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan602 - 602_isd-c_172.16.242.254/24 = 'adminDown' | PASS | - |
| 99 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan603 - 603_isd-d_172.16.243.254/24 = 'adminDown' | PASS | - |
| 100 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan629 - 629_closet10-c_172.16.154.254/24 = 'adminDown' | PASS | - |
| 101 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan681 - 681_dot212_172.16.212.254/24 = 'adminDown' | PASS | - |
| 102 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan682 - 682_dot220_172.16.220.254/24 = 'adminDown' | PASS | - |
| 103 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan703 - 703_pcaim_172.16.3.254/24 = 'adminDown' | PASS | - |
| 104 | HRAO-CORE-10 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan704 - 704_security_172.16.4.254/24 = 'adminDown' | PASS | - |
| 105 | HRAO-CORE-10 | Interfaces | VerifyLoopbackCount | Verifies the number of loopback interfaces and their status. | - | PASS | - |
| 106 | HRAO-CORE-10 | MLAG | VerifyMlagConfigSanity | Verifies there are no MLAG config-sanity inconsistencies. | - | PASS | - |
| 107 | HRAO-CORE-10 | MLAG | VerifyMlagInterfaces | Verifies there are no inactive or active-partial MLAG ports. | - | PASS | - |
| 108 | HRAO-CORE-10 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 109 | HRAO-CORE-10 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | - | PASS | - |
| 110 | HRAO-CORE-10 | Software | VerifyEOSVersion | Verifies the EOS version of the device. | - | PASS | - |
| 111 | HRAO-CORE-10 | Software | VerifyTerminAttrVersion | Verifies the TerminAttr version of the device. | - | PASS | - |
| 112 | HRAO-CORE-10 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | PASS | - |
| 113 | HRAOISD1-1-0 | Configuration | VerifyRunningConfigDiffs | Verifies there is no difference between the running-config and the startup-config | - | PASS | - |
| 114 | HRAOISD1-1-0 | Configuration | VerifyZeroTouch | Verifies ZeroTouch is disabled | - | PASS | - |
| 115 | HRAOISD1-1-0 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet49 - Remote: HRAO-CORE-1 Ethernet6 | PASS | - |
| 116 | HRAOISD1-1-0 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet51 - Remote: HRAOISD1-1-1 Ethernet51 | PASS | - |
| 117 | HRAOISD1-1-0 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet52 - Remote: HRAOISD1-1-1 Ethernet52 | PASS | - |
| 118 | HRAOISD1-1-0 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet53/1 - Remote: HRAOISD1-1-2 Ethernet49 | PASS | - |
| 119 | HRAOISD1-1-0 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet53/2 - Remote: HRAOISD1-1-3 Ethernet49 | PASS | - |
| 120 | HRAOISD1-1-0 | Connectivity | VerifyReachability | Test the network reachability to one or many destination IP(s). | TEST PING TO INTERNET 8.8.8.8 | PASS | - |
| 121 | HRAOISD1-1-0 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on vEOS-lab. |
| 122 | HRAOISD1-1-0 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on vEOS-lab. |
| 123 | HRAOISD1-1-0 | Hardware | VerifyTemperature | Verifies the device temperature. | - | SKIPPED | VerifyTemperature test is not supported on vEOS-lab. |
| 124 | HRAOISD1-1-0 | Hardware | VerifyTransceiversManufacturers | Verifies if all transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on vEOS-lab. |
| 125 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet1 - 3/201/12 = 'up' | PASS | - |
| 126 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet10 - 2/2/207-2d = 'up' | PASS | - |
| 127 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet11 - 2/2/208-1d = 'up' | PASS | - |
| 128 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet12 - CCC-CLK = 'up' | PASS | - |
| 129 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet13 - APP-NETA = 'up' | PASS | - |
| 130 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet14 - 2/2/209-2d = 'up' | PASS | - |
| 131 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet15 - 2/3/210/4 = 'up' | PASS | - |
| 132 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet16 - OUTSIDE-BLDG1-CAM1 = 'up' | PASS | - |
| 133 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet17 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 134 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet18 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 135 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet19 - 2/210/5 = 'up' | PASS | - |
| 136 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet2 - 2/228/lieb-01 = 'up' | PASS | - |
| 137 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet20 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 138 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet21 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 139 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet22 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 140 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet23 - AP3700_SRR3_AP1 = 'up' | PASS | - |
| 141 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet24 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 142 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet25 - 558-2D = 'up' | PASS | - |
| 143 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet26 - 2/222/3/1 = 'up' | PASS | - |
| 144 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet27 - MOD-DISP-B-DATA = 'up' | PASS | - |
| 145 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet28 - MOD-DISP-A-DATA = 'up' | PASS | - |
| 146 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet29 - CCB-Vid-CONF = 'up' | PASS | - |
| 147 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet3 - 2/3/202/65 = 'up' | PASS | - |
| 148 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet30 - CCC-Vid-CONF = 'up' | PASS | - |
| 149 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet31 - ISD-VIDEO-CONF-DATA = 'up' | PASS | - |
| 150 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet32 - 2/210/18 = 'up' | PASS | - |
| 151 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet33 - 2/210/19 = 'up' | PASS | - |
| 152 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet34 - 2/210/20 = 'up' | PASS | - |
| 153 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet35 - 2/214/1 = 'up' | PASS | - |
| 154 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet36 - 2/214/2 = 'up' | PASS | - |
| 155 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet37 - 210/22/CCA = 'up' | PASS | - |
| 156 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet38 - 2/226D-4D = 'up' | PASS | - |
| 157 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet39 - 2/226D-6D = 'up' | PASS | - |
| 158 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet4 - 2/3/202/66 = 'up' | PASS | - |
| 159 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet40 - 20/2/228/298 = 'up' | PASS | - |
| 160 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet41 - Travel_Office_VPN-Netgear_Pt4 = 'up' | PASS | - |
| 161 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet42 - 2/226D-5D(Main_Video_CR) = 'up' | PASS | - |
| 162 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet43 - 2/214/9_CCC_-_Outlet_in_back_corner_-_Top_Right_Port = 'up' | PASS | - |
| 163 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet44 - 2/214/10_CCC_-_Outlet_in_back_corner_-_Top_Left_Port = 'up' | PASS | - |
| 164 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet45 - 2/227//CGI-01 = 'up' | PASS | - |
| 165 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet46 - 2/214A/2 = 'up' | PASS | - |
| 166 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet47 - 2/214A/3 = 'up' | PASS | - |
| 167 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet48 - 2/214A/4 = 'up' | PASS | - |
| 168 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet49 - HRAO-CORE-1_Ethernet6 = 'up' | PASS | - |
| 169 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet5 - 2/3/202/99(Model_Display_A) = 'up' | PASS | - |
| 170 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet51 - MLAG_PEER_HRAOISD1-1-1_Ethernet51 = 'up' | PASS | - |
| 171 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet52 - MLAG_PEER_HRAOISD1-1-1_Ethernet52 = 'up' | PASS | - |
| 172 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet53/1 - HRAOISD1-1-2_Ethernet49 = 'up' | PASS | - |
| 173 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet53/2 - HRAOISD1-1-3_Ethernet49 = 'up' | PASS | - |
| 174 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet6 - Conf_-_A-CLK = 'up' | PASS | - |
| 175 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet7 - 2/210/17 = 'up' | PASS | - |
| 176 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet8 - CCD-CLK = 'up' | PASS | - |
| 177 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet9 - CCB-CLK = 'up' | PASS | - |
| 178 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel49 - CORES_Po6 = 'up' | PASS | - |
| 179 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel51 - MLAG_PEER_HRAOISD1-1-1_Po51 = 'up' | PASS | - |
| 180 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel531 - HRAOISD1-1-2_Po49 = 'up' | PASS | - |
| 181 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel532 - HRAOISD1-1-3_Po49 = 'up' | PASS | - |
| 182 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan4094 - MLAG_PEER = 'up' | PASS | - |
| 183 | HRAOISD1-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan5 - Inband Management = 'up' | PASS | - |
| 184 | HRAOISD1-1-0 | MLAG | VerifyMlagConfigSanity | Verifies there are no MLAG config-sanity inconsistencies. | - | PASS | - |
| 185 | HRAOISD1-1-0 | MLAG | VerifyMlagInterfaces | Verifies there are no inactive or active-partial MLAG ports. | - | PASS | - |
| 186 | HRAOISD1-1-0 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 187 | HRAOISD1-1-0 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | - | PASS | - |
| 188 | HRAOISD1-1-0 | Software | VerifyEOSVersion | Verifies the EOS version of the device. | - | PASS | - |
| 189 | HRAOISD1-1-0 | Software | VerifyTerminAttrVersion | Verifies the TerminAttr version of the device. | - | PASS | - |
| 190 | HRAOISD1-1-0 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | PASS | - |
| 191 | HRAOISD1-1-1 | Configuration | VerifyRunningConfigDiffs | Verifies there is no difference between the running-config and the startup-config | - | PASS | - |
| 192 | HRAOISD1-1-1 | Configuration | VerifyZeroTouch | Verifies ZeroTouch is disabled | - | PASS | - |
| 193 | HRAOISD1-1-1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet49 - Remote: HRAO-CORE-10 Ethernet6 | PASS | - |
| 194 | HRAOISD1-1-1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet51 - Remote: HRAOISD1-1-0 Ethernet51 | PASS | - |
| 195 | HRAOISD1-1-1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet52 - Remote: HRAOISD1-1-0 Ethernet52 | PASS | - |
| 196 | HRAOISD1-1-1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet53/1 - Remote: HRAOISD1-1-2 Ethernet50 | PASS | - |
| 197 | HRAOISD1-1-1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet53/2 - Remote: HRAOISD1-1-3 Ethernet50 | PASS | - |
| 198 | HRAOISD1-1-1 | Connectivity | VerifyReachability | Test the network reachability to one or many destination IP(s). | TEST PING TO INTERNET 8.8.8.8 | PASS | - |
| 199 | HRAOISD1-1-1 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on vEOS-lab. |
| 200 | HRAOISD1-1-1 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on vEOS-lab. |
| 201 | HRAOISD1-1-1 | Hardware | VerifyTemperature | Verifies the device temperature. | - | SKIPPED | VerifyTemperature test is not supported on vEOS-lab. |
| 202 | HRAOISD1-1-1 | Hardware | VerifyTransceiversManufacturers | Verifies if all transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on vEOS-lab. |
| 203 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet1 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 204 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet10 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 205 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet11 - 558-D1 = 'up' | PASS | - |
| 206 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet12 - 2/214A/8_CCB_Floor = 'up' | PASS | - |
| 207 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet13 - security_panel_rm_2-217 Panel 3 = 'up' | PASS | - |
| 208 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet14 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 209 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet15 - 2/2/226-SEC1 = 'up' | PASS | - |
| 210 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet16 - 2/2/226-SEC2 = 'up' | PASS | - |
| 211 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet17 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 212 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet18 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 213 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet19 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 214 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet2 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 215 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet20 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 216 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet21 - 2/2-209/1D = 'up' | PASS | - |
| 217 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet22 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 218 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet23 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 219 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet24 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 220 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet25 - UPS = 'up' | PASS | - |
| 221 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet26 - UPS = 'up' | PASS | - |
| 222 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet27 - 2/2-222A-No-PoE = 'up' | PASS | - |
| 223 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet28 - 2/2-217-2D = 'up' | PASS | - |
| 224 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet29 - 2/2/210A-No-PoE = 'up' | PASS | - |
| 225 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet3 - 2/222-5D = 'up' | PASS | - |
| 226 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet30 - 2/214A = 'up' | PASS | - |
| 227 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet31 - 2/2/210A-No-PoE = 'up' | PASS | - |
| 228 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet32 - 2/209-No-PoE = 'up' | PASS | - |
| 229 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet33 - 2/2-214B = 'up' | PASS | - |
| 230 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet34 - 2/2-No-PoE = 'up' | PASS | - |
| 231 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet35 - 2/2 = 'up' | PASS | - |
| 232 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet36 - 20/2/226-No-PoE = 'up' | PASS | - |
| 233 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet37 - 20/2/226-No-POE = 'up' | PASS | - |
| 234 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet38 - 20/2/226-No-POE = 'up' | PASS | - |
| 235 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet39 - 20/2/226-AP4(AP3700_ISD_AP5) = 'up' | PASS | - |
| 236 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet4 - 2/222-6D = 'up' | PASS | - |
| 237 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet40 - 20/2/226-No-POE = 'up' | PASS | - |
| 238 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet41 - 20/2/226-No-POE = 'up' | PASS | - |
| 239 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet42 - 20/2/226-No-POE = 'up' | PASS | - |
| 240 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet43 - 2/2-210A-No-PoE = 'up' | PASS | - |
| 241 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet44 - 2/2-221-No-PoE = 'up' | PASS | - |
| 242 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet45 - 2/2-214A = 'up' | PASS | - |
| 243 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet46 - 2/2-Lobby-AP1(AP3700_LOBBY_AP1) = 'up' | PASS | - |
| 244 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet47 - Outside_Lobby_CAM = 'up' | PASS | - |
| 245 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet48 - VACANT = 'up' | PASS | - |
| 246 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet49 - HRAO-CORE-10_Ethernet6 = 'up' | PASS | - |
| 247 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet5 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 248 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet51 - MLAG_PEER_HRAOISD1-1-0_Ethernet51 = 'up' | PASS | - |
| 249 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet52 - MLAG_PEER_HRAOISD1-1-0_Ethernet52 = 'up' | PASS | - |
| 250 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet53/1 - HRAOISD1-1-2_Ethernet50 = 'up' | PASS | - |
| 251 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet53/2 - HRAOISD1-1-3_Ethernet50 = 'up' | PASS | - |
| 252 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet6 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 253 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet7 - VACANT_SINCE_07-19-2016 = 'up' | PASS | - |
| 254 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet8 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 255 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet9 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 256 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel49 - CORES_Po6 = 'up' | PASS | - |
| 257 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel51 - MLAG_PEER_HRAOISD1-1-0_Po51 = 'up' | PASS | - |
| 258 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel531 - HRAOISD1-1-2_Po49 = 'up' | PASS | - |
| 259 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel532 - HRAOISD1-1-3_Po49 = 'up' | PASS | - |
| 260 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan4094 - MLAG_PEER = 'up' | PASS | - |
| 261 | HRAOISD1-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan5 - Inband Management = 'up' | PASS | - |
| 262 | HRAOISD1-1-1 | MLAG | VerifyMlagConfigSanity | Verifies there are no MLAG config-sanity inconsistencies. | - | PASS | - |
| 263 | HRAOISD1-1-1 | MLAG | VerifyMlagInterfaces | Verifies there are no inactive or active-partial MLAG ports. | - | PASS | - |
| 264 | HRAOISD1-1-1 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 265 | HRAOISD1-1-1 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | - | PASS | - |
| 266 | HRAOISD1-1-1 | Software | VerifyEOSVersion | Verifies the EOS version of the device. | - | PASS | - |
| 267 | HRAOISD1-1-1 | Software | VerifyTerminAttrVersion | Verifies the TerminAttr version of the device. | - | PASS | - |
| 268 | HRAOISD1-1-1 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | PASS | - |
| 269 | HRAOISD1-1-2 | Configuration | VerifyRunningConfigDiffs | Verifies there is no difference between the running-config and the startup-config | - | PASS | - |
| 270 | HRAOISD1-1-2 | Configuration | VerifyZeroTouch | Verifies ZeroTouch is disabled | - | PASS | - |
| 271 | HRAOISD1-1-2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet49 - Remote: HRAOISD1-1-0 Ethernet53/1 | PASS | - |
| 272 | HRAOISD1-1-2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet50 - Remote: HRAOISD1-1-1 Ethernet53/1 | PASS | - |
| 273 | HRAOISD1-1-2 | Connectivity | VerifyReachability | Test the network reachability to one or many destination IP(s). | TEST PING TO INTERNET 8.8.8.8 | PASS | - |
| 274 | HRAOISD1-1-2 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on vEOS-lab. |
| 275 | HRAOISD1-1-2 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on vEOS-lab. |
| 276 | HRAOISD1-1-2 | Hardware | VerifyTemperature | Verifies the device temperature. | - | SKIPPED | VerifyTemperature test is not supported on vEOS-lab. |
| 277 | HRAOISD1-1-2 | Hardware | VerifyTransceiversManufacturers | Verifies if all transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on vEOS-lab. |
| 278 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet1 - 2/221-05 = 'up' | PASS | - |
| 279 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet10 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 280 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet11 - VACANT_SINCE_04-18-2017 = 'up' | PASS | - |
| 281 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet12 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 282 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet13 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 283 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet14 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 284 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet15 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 285 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet16 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 286 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet17 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 287 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet18 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 288 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet19 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 289 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet2 - 2/221-08 = 'up' | PASS | - |
| 290 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet20 - 2/2-207-AP1(AP3700_SRR3_AP1) = 'up' | PASS | - |
| 291 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet21 - 2/2-208/2D = 'up' | PASS | - |
| 292 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet22 - 3/201A/4 = 'up' | PASS | - |
| 293 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet23 - 3/201B/1(HRA-O_PROJ_RM1) = 'up' | PASS | - |
| 294 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet24 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 295 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet25 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 296 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet26 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 297 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet27 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 298 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet28 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 299 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet29 - 3/202/1 = 'up' | PASS | - |
| 300 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet3 - 2/221-09 = 'up' | PASS | - |
| 301 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet30 - 3/202/2 = 'up' | PASS | - |
| 302 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet31 - 3/202/3(Model_Display_B) = 'up' | PASS | - |
| 303 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet32 - 3/202/4 = 'up' | PASS | - |
| 304 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet33 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 305 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet34 - 210/1() = 'up' | PASS | - |
| 306 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet35 - 3/202/7 = 'up' | PASS | - |
| 307 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet36 - 3/202/8 = 'up' | PASS | - |
| 308 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet37 - 3/202/9 = 'up' | PASS | - |
| 309 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet38 - 210/2() = 'up' | PASS | - |
| 310 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet39 - 2/2-lobby-cam1 = 'up' | PASS | - |
| 311 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet4 - 2/221-11 = 'up' | PASS | - |
| 312 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet40 - 3/202/14/1 = 'up' | PASS | - |
| 313 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet41 - 3/202/14/2 = 'up' | PASS | - |
| 314 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet42 - 210/11/-AP1(AP3700_ISD_AP1) = 'up' | PASS | - |
| 315 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet43 - 2/2-215-01D(Board-Room) = 'up' | PASS | - |
| 316 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet44 - 2/2-215-02D(Board-Room) = 'up' | PASS | - |
| 317 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet45 - 2/2-215-03D(Board-Room) = 'up' | PASS | - |
| 318 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet46 - 2/2-215-04D(Board-Room) = 'up' | PASS | - |
| 319 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet47 - 2/2-215-05D(Board-Room) = 'up' | PASS | - |
| 320 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet48 - 2/2-215-06D(Board-Room) = 'up' | PASS | - |
| 321 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet49 - HRAOISD1-1-0_Ethernet53/1 = 'up' | PASS | - |
| 322 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet5 - 2/221-16 = 'up' | PASS | - |
| 323 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet50 - HRAOISD1-1-1_Ethernet53/1 = 'up' | PASS | - |
| 324 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet6 - 2/221-18 = 'up' | PASS | - |
| 325 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet7 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 326 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet8 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 327 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet9 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 328 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel49 - ISD1-SPINES_Po531 = 'up' | PASS | - |
| 329 | HRAOISD1-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan5 - Inband Management = 'up' | PASS | - |
| 330 | HRAOISD1-1-2 | MLAG | VerifyMlagConfigSanity | Verifies there are no MLAG config-sanity inconsistencies. | - | SKIPPED | MLAG is disabled |
| 331 | HRAOISD1-1-2 | MLAG | VerifyMlagInterfaces | Verifies there are no inactive or active-partial MLAG ports. | - | SKIPPED | MLAG is disabled |
| 332 | HRAOISD1-1-2 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | SKIPPED | MLAG is disabled |
| 333 | HRAOISD1-1-2 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | - | PASS | - |
| 334 | HRAOISD1-1-2 | Software | VerifyEOSVersion | Verifies the EOS version of the device. | - | PASS | - |
| 335 | HRAOISD1-1-2 | Software | VerifyTerminAttrVersion | Verifies the TerminAttr version of the device. | - | PASS | - |
| 336 | HRAOISD1-1-2 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | PASS | - |
| 337 | HRAOISD1-1-3 | Configuration | VerifyRunningConfigDiffs | Verifies there is no difference between the running-config and the startup-config | - | PASS | - |
| 338 | HRAOISD1-1-3 | Configuration | VerifyZeroTouch | Verifies ZeroTouch is disabled | - | PASS | - |
| 339 | HRAOISD1-1-3 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet49 - Remote: HRAOISD1-1-0 Ethernet53/2 | PASS | - |
| 340 | HRAOISD1-1-3 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet50 - Remote: HRAOISD1-1-1 Ethernet53/2 | PASS | - |
| 341 | HRAOISD1-1-3 | Connectivity | VerifyReachability | Test the network reachability to one or many destination IP(s). | TEST PING TO INTERNET 8.8.8.8 | PASS | - |
| 342 | HRAOISD1-1-3 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on vEOS-lab. |
| 343 | HRAOISD1-1-3 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on vEOS-lab. |
| 344 | HRAOISD1-1-3 | Hardware | VerifyTemperature | Verifies the device temperature. | - | SKIPPED | VerifyTemperature test is not supported on vEOS-lab. |
| 345 | HRAOISD1-1-3 | Hardware | VerifyTransceiversManufacturers | Verifies if all transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on vEOS-lab. |
| 346 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet1 - WL913459_server = 'up' | PASS | - |
| 347 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet10 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 348 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet11 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 349 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet12 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 350 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet13 - InterWorkingLabs(KMAX) = 'up' | PASS | - |
| 351 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet14 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 352 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet15 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 353 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet16 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 354 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet17 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 355 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet18 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 356 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet19 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 357 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet2 - APP-NETA = 'up' | PASS | - |
| 358 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet20 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 359 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet21 - 2/2-207/1D = 'up' | PASS | - |
| 360 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet22 - UPS-307552-TEST = 'up' | PASS | - |
| 361 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet23 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 362 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet24 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 363 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet25 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 364 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet26 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 365 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet27 - Hall_AP1(AP3700_GENERALMR_AP1) = 'up' | PASS | - |
| 366 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet28 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 367 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet29 - AP3700_CCA_AP2 = 'up' | PASS | - |
| 368 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet3 - AppNetta = 'up' | PASS | - |
| 369 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet30 - AP3700_CCC_AP1 = 'up' | PASS | - |
| 370 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet31 - AP3700_CCA_AP1 = 'up' | PASS | - |
| 371 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet32 - ap3700_fso_office_ap1 = 'up' | PASS | - |
| 372 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet33 - AP3700_CCB_AP1 = 'up' | PASS | - |
| 373 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet34 - lobby-cam1 = 'up' | PASS | - |
| 374 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet35 - vaccant = 'up' | PASS | - |
| 375 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet36 - AP3700_ISD_AP8 = 'up' | PASS | - |
| 376 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet37 - AP3700_ISD_AP7 = 'up' | PASS | - |
| 377 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet38 - AP3700_ISD_AP6 = 'up' | PASS | - |
| 378 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet39 - AP3700_ISD_AP5 = 'up' | PASS | - |
| 379 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet4 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 380 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet40 - 20/2/226(AP3700_ISD_AP3) = 'up' | PASS | - |
| 381 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet41 - 20/2/226(AP3700_ISD_AP2) = 'up' | PASS | - |
| 382 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet42 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 383 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet43 - AP3700_CCA_AP3 = 'up' | PASS | - |
| 384 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet44 - AP3700_TRAVEL_AP1 = 'up' | PASS | - |
| 385 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet45 - AP3700_CCC_AP2 = 'up' | PASS | - |
| 386 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet46 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 387 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet47 - HRAOTEST-SWITCH = 'up' | PASS | - |
| 388 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet48 - HRAOTEST-SWITCH = 'up' | PASS | - |
| 389 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet49 - HRAOISD1-1-0_Ethernet53/2 = 'up' | PASS | - |
| 390 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet5 - VACANT_SINCE_05-25-2016 = 'up' | PASS | - |
| 391 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet50 - HRAOISD1-1-1_Ethernet53/2 = 'up' | PASS | - |
| 392 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet6 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 393 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet7 - VACANT_SINCE_01-24-2018 = 'up' | PASS | - |
| 394 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet8 - VACANT_SINCE_07-19-2016 = 'up' | PASS | - |
| 395 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet9 - VACANT_SINCE_12-26-2015 = 'up' | PASS | - |
| 396 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel49 - ISD1-SPINES_Po532 = 'up' | PASS | - |
| 397 | HRAOISD1-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan5 - Inband Management = 'up' | PASS | - |
| 398 | HRAOISD1-1-3 | MLAG | VerifyMlagConfigSanity | Verifies there are no MLAG config-sanity inconsistencies. | - | SKIPPED | MLAG is disabled |
| 399 | HRAOISD1-1-3 | MLAG | VerifyMlagInterfaces | Verifies there are no inactive or active-partial MLAG ports. | - | SKIPPED | MLAG is disabled |
| 400 | HRAOISD1-1-3 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | SKIPPED | MLAG is disabled |
| 401 | HRAOISD1-1-3 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | - | PASS | - |
| 402 | HRAOISD1-1-3 | Software | VerifyEOSVersion | Verifies the EOS version of the device. | - | PASS | - |
| 403 | HRAOISD1-1-3 | Software | VerifyTerminAttrVersion | Verifies the TerminAttr version of the device. | - | PASS | - |
| 404 | HRAOISD1-1-3 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | PASS | - |
| 405 | HRAOISD2-1-0 | Configuration | VerifyRunningConfigDiffs | Verifies there is no difference between the running-config and the startup-config | - | PASS | - |
| 406 | HRAOISD2-1-0 | Configuration | VerifyZeroTouch | Verifies ZeroTouch is disabled | - | PASS | - |
| 407 | HRAOISD2-1-0 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet49 - Remote: HRAO-CORE-1 Ethernet5 | PASS | - |
| 408 | HRAOISD2-1-0 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet51 - Remote: HRAOISD2-1-1 Ethernet51 | PASS | - |
| 409 | HRAOISD2-1-0 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet52 - Remote: HRAOISD2-1-1 Ethernet52 | PASS | - |
| 410 | HRAOISD2-1-0 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet53/1 - Remote: HRAOISD2-1-2 Ethernet49 | PASS | - |
| 411 | HRAOISD2-1-0 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet53/2 - Remote: HRAOISD2-1-3 Ethernet49 | PASS | - |
| 412 | HRAOISD2-1-0 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet53/3 - Remote: HRAOISD2-1-4 Ethernet49 | PASS | - |
| 413 | HRAOISD2-1-0 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet53/4 - Remote: HRAOISD2-1-5 Ethernet49 | PASS | - |
| 414 | HRAOISD2-1-0 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet54/1 - Remote: HRAOISD2-1-6 Ethernet49 | PASS | - |
| 415 | HRAOISD2-1-0 | Connectivity | VerifyReachability | Test the network reachability to one or many destination IP(s). | TEST PING TO INTERNET 8.8.8.8 | PASS | - |
| 416 | HRAOISD2-1-0 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on vEOS-lab. |
| 417 | HRAOISD2-1-0 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on vEOS-lab. |
| 418 | HRAOISD2-1-0 | Hardware | VerifyTemperature | Verifies the device temperature. | - | SKIPPED | VerifyTemperature test is not supported on vEOS-lab. |
| 419 | HRAOISD2-1-0 | Hardware | VerifyTransceiversManufacturers | Verifies if all transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on vEOS-lab. |
| 420 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet1 - 20/2-226/001D = 'up' | PASS | - |
| 421 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet10 - 20/2-226/029D = 'up' | PASS | - |
| 422 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet11 - 20/2-226/006D = 'up' | PASS | - |
| 423 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet12 - 20/2-226/030D = 'up' | PASS | - |
| 424 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet13 - 20/2-226/160D = 'up' | PASS | - |
| 425 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet14 - UP_SINCE_06-03-2018 = 'up' | PASS | - |
| 426 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet15 - 20/2-226/APPNETA = 'up' | PASS | - |
| 427 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet16 - 20/2-226/032D = 'up' | PASS | - |
| 428 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet17 - 20/2-228/318D = 'up' | PASS | - |
| 429 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet18 - 20/2-228/319D = 'up' | PASS | - |
| 430 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet19 - 20/2-226/010D = 'up' | PASS | - |
| 431 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet2 - 20/2-226/025D = 'up' | PASS | - |
| 432 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet20 - 20/2-226/034D = 'up' | PASS | - |
| 433 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet21 - 20/2-228/320D = 'up' | PASS | - |
| 434 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet22 - 20/2-228/320D = 'up' | PASS | - |
| 435 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet23 - 20/2-226/012D = 'up' | PASS | - |
| 436 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet24 - 20/2-226/036D = 'up' | PASS | - |
| 437 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet25 - 20/2-226/021D = 'up' | PASS | - |
| 438 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet26 - 20/2-226/138D = 'up' | PASS | - |
| 439 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet27 - 20/2-226/014D = 'up' | PASS | - |
| 440 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet28 - 20/2-226/197D = 'up' | PASS | - |
| 441 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet29 - 20/2-226/015D = 'up' | PASS | - |
| 442 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet3 - 20/2-226/002D = 'up' | PASS | - |
| 443 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet30 - 20/2-226/107D = 'up' | PASS | - |
| 444 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet31 - 20/2-226/016D = 'up' | PASS | - |
| 445 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet32 - 20/2-226/040D = 'up' | PASS | - |
| 446 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet33 - 20/2-226/017D = 'up' | PASS | - |
| 447 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet34 - 20/2-226/Netgear_switch/isd_re-immaging_desk = 'up' | PASS | - |
| 448 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet35 - 20/2-226/019D = 'up' | PASS | - |
| 449 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet36 - 20/2-226/042D = 'up' | PASS | - |
| 450 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet37 - 20/2-226/D-273 = 'up' | PASS | - |
| 451 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet38 - 20/2-226/043D = 'up' | PASS | - |
| 452 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet39 - 20/2-226/DLINK_ROUTER(IOT_WiFi_Router) = 'up' | PASS | - |
| 453 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet4 - 20/2-226/026D = 'up' | PASS | - |
| 454 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet40 - 20/2-226/044D = 'up' | PASS | - |
| 455 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet41 - 20/2-226/023D = 'up' | PASS | - |
| 456 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet42 - 20/2-226/D-274 = 'up' | PASS | - |
| 457 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet43 - 20/2-226/ISD_WAP_3D(AP3700_ISD_AP9) = 'up' | PASS | - |
| 458 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet44 - 20/2-226/D-275 = 'up' | PASS | - |
| 459 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet45 - 20/2-226/018D = 'up' | PASS | - |
| 460 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet46 - 20/2-226/D-278 = 'up' | PASS | - |
| 461 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet47 - 20/2-226/024D = 'up' | PASS | - |
| 462 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet48 - 20/2-226/048D = 'up' | PASS | - |
| 463 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet49 - HRAO-CORE-1_Ethernet5 = 'up' | PASS | - |
| 464 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet5 - 20/2-226/003D = 'up' | PASS | - |
| 465 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet51 - MLAG_PEER_HRAOISD2-1-1_Ethernet51 = 'up' | PASS | - |
| 466 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet52 - MLAG_PEER_HRAOISD2-1-1_Ethernet52 = 'up' | PASS | - |
| 467 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet53/1 - HRAOISD2-1-2_Ethernet49 = 'up' | PASS | - |
| 468 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet53/2 - HRAOISD2-1-3_Ethernet49 = 'up' | PASS | - |
| 469 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet53/3 - HRAOISD2-1-4_Ethernet49 = 'up' | PASS | - |
| 470 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet53/4 - HRAOISD2-1-5_Ethernet49 = 'up' | PASS | - |
| 471 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet54/1 - HRAOISD2-1-6_Ethernet49 = 'up' | PASS | - |
| 472 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet6 - 20/2-226/027D = 'up' | PASS | - |
| 473 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet7 - 20/2-226/004D = 'up' | PASS | - |
| 474 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet8 - 20/2-226/028D = 'up' | PASS | - |
| 475 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet9 - 20/2-226/005D = 'up' | PASS | - |
| 476 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel49 - CORES_Po5 = 'up' | PASS | - |
| 477 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel51 - MLAG_PEER_HRAOISD2-1-1_Po51 = 'up' | PASS | - |
| 478 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel531 - HRAOISD2-1-2_Po49 = 'up' | PASS | - |
| 479 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel532 - HRAOISD2-1-3_Po49 = 'up' | PASS | - |
| 480 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel533 - HRAOISD2-1-4_Po49 = 'up' | PASS | - |
| 481 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel534 - HRAOISD2-1-5_Po49 = 'up' | PASS | - |
| 482 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel541 - HRAOISD2-1-6_Po49 = 'up' | PASS | - |
| 483 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan4094 - MLAG_PEER = 'up' | PASS | - |
| 484 | HRAOISD2-1-0 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan5 - Inband Management = 'up' | PASS | - |
| 485 | HRAOISD2-1-0 | MLAG | VerifyMlagConfigSanity | Verifies there are no MLAG config-sanity inconsistencies. | - | PASS | - |
| 486 | HRAOISD2-1-0 | MLAG | VerifyMlagInterfaces | Verifies there are no inactive or active-partial MLAG ports. | - | PASS | - |
| 487 | HRAOISD2-1-0 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 488 | HRAOISD2-1-0 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | - | PASS | - |
| 489 | HRAOISD2-1-0 | Software | VerifyEOSVersion | Verifies the EOS version of the device. | - | PASS | - |
| 490 | HRAOISD2-1-0 | Software | VerifyTerminAttrVersion | Verifies the TerminAttr version of the device. | - | PASS | - |
| 491 | HRAOISD2-1-0 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | PASS | - |
| 492 | HRAOISD2-1-1 | Configuration | VerifyRunningConfigDiffs | Verifies there is no difference between the running-config and the startup-config | - | PASS | - |
| 493 | HRAOISD2-1-1 | Configuration | VerifyZeroTouch | Verifies ZeroTouch is disabled | - | PASS | - |
| 494 | HRAOISD2-1-1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet49 - Remote: HRAO-CORE-10 Ethernet5 | PASS | - |
| 495 | HRAOISD2-1-1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet51 - Remote: HRAOISD2-1-0 Ethernet51 | PASS | - |
| 496 | HRAOISD2-1-1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet52 - Remote: HRAOISD2-1-0 Ethernet52 | PASS | - |
| 497 | HRAOISD2-1-1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet53/1 - Remote: HRAOISD2-1-2 Ethernet50 | PASS | - |
| 498 | HRAOISD2-1-1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet53/2 - Remote: HRAOISD2-1-3 Ethernet50 | PASS | - |
| 499 | HRAOISD2-1-1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet53/3 - Remote: HRAOISD2-1-4 Ethernet50 | PASS | - |
| 500 | HRAOISD2-1-1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet53/4 - Remote: HRAOISD2-1-5 Ethernet50 | PASS | - |
| 501 | HRAOISD2-1-1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet54/1 - Remote: HRAOISD2-1-6 Ethernet50 | PASS | - |
| 502 | HRAOISD2-1-1 | Connectivity | VerifyReachability | Test the network reachability to one or many destination IP(s). | TEST PING TO INTERNET 8.8.8.8 | PASS | - |
| 503 | HRAOISD2-1-1 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on vEOS-lab. |
| 504 | HRAOISD2-1-1 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on vEOS-lab. |
| 505 | HRAOISD2-1-1 | Hardware | VerifyTemperature | Verifies the device temperature. | - | SKIPPED | VerifyTemperature test is not supported on vEOS-lab. |
| 506 | HRAOISD2-1-1 | Hardware | VerifyTransceiversManufacturers | Verifies if all transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on vEOS-lab. |
| 507 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet1 - UP_SINCE_05-24-2018 = 'up' | PASS | - |
| 508 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet10 - 20/2-226/077D = 'up' | PASS | - |
| 509 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet11 - 20/2-226/054D = 'up' | PASS | - |
| 510 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet12 - 20/2-226/078D = 'up' | PASS | - |
| 511 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet13 - 20/2-226/055D = 'up' | PASS | - |
| 512 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet14 - UP_SINCE_01-26-2018 = 'up' | PASS | - |
| 513 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet15 - 20/2/226-284D = 'up' | PASS | - |
| 514 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet16 - 20/2-226/147D = 'up' | PASS | - |
| 515 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet17 - VACANT_SINCE_07-13-2016 = 'up' | PASS | - |
| 516 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet18 - 20/2-226/081D = 'up' | PASS | - |
| 517 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet19 - 20/2/226-284D = 'up' | PASS | - |
| 518 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet2 - UP_SINCE_01-16-2018 = 'up' | PASS | - |
| 519 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet20 - 20/2-226/082D = 'up' | PASS | - |
| 520 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet21 - VACANT_SINCE_01-13-2017 = 'up' | PASS | - |
| 521 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet22 - 20/2-226/D058 = 'up' | PASS | - |
| 522 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet23 - 20/2-226/TRIPLITE(909705) = 'up' | PASS | - |
| 523 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet24 - Velo-Cloud/312310 = 'up' | PASS | - |
| 524 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet25 - 20/2-226/D-276D = 'up' | PASS | - |
| 525 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet26 - UP_SINCE_05-25-2018 = 'up' | PASS | - |
| 526 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet27 - UP_SINCE_03-08-2018 = 'up' | PASS | - |
| 527 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet28 - 20/2/226-86D = 'up' | PASS | - |
| 528 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet29 - UP_SINCE_01-18-2018 = 'up' | PASS | - |
| 529 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet3 - 20/2-226/326D = 'up' | PASS | - |
| 530 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet30 - 20/2/226-87D = 'up' | PASS | - |
| 531 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet31 - 20/2-226/064D = 'up' | PASS | - |
| 532 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet32 - 20/2/226-88D = 'up' | PASS | - |
| 533 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet33 - 20/2-226/065D = 'up' | PASS | - |
| 534 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet34 - 20/2/226/D-277_Service_Desk_1-G = 'up' | PASS | - |
| 535 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet35 - 20/2-226/BLANK = 'up' | PASS | - |
| 536 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet36 - 20/2-226/09D = 'up' | PASS | - |
| 537 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet37 - 20/2-226/143D = 'up' | PASS | - |
| 538 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet38 - 20/2-226/091D = 'up' | PASS | - |
| 539 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet39 - 20/2/230-346D = 'up' | PASS | - |
| 540 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet4 - 20/2-226/074D = 'up' | PASS | - |
| 541 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet40 - 20/2-230/347D(ISD-PRJ_RM-2-SOLSTICE) = 'up' | PASS | - |
| 542 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet41 - VACANT_SINCE_08-03-2016 = 'up' | PASS | - |
| 543 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet42 - 20/2-226/069D = 'up' | PASS | - |
| 544 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet43 - VACANT_SINCE_06-06-2016 = 'up' | PASS | - |
| 545 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet44 - 20/2/229-349D = 'up' | PASS | - |
| 546 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet45 - UP_SINCE_05-29-2018 = 'up' | PASS | - |
| 547 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet46 - 20/2-226/D039 = 'up' | PASS | - |
| 548 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet47 - 20/2-226/115D = 'up' | PASS | - |
| 549 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet48 - 20/2-226/D041 = 'up' | PASS | - |
| 550 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet49 - HRAO-CORE-10_Ethernet5 = 'up' | PASS | - |
| 551 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet5 - 20/2-226/051D = 'up' | PASS | - |
| 552 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet51 - MLAG_PEER_HRAOISD2-1-0_Ethernet51 = 'up' | PASS | - |
| 553 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet52 - MLAG_PEER_HRAOISD2-1-0_Ethernet52 = 'up' | PASS | - |
| 554 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet53/1 - HRAOISD2-1-2_Ethernet50 = 'up' | PASS | - |
| 555 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet53/2 - HRAOISD2-1-3_Ethernet50 = 'up' | PASS | - |
| 556 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet53/3 - HRAOISD2-1-4_Ethernet50 = 'up' | PASS | - |
| 557 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet53/4 - HRAOISD2-1-5_Ethernet50 = 'up' | PASS | - |
| 558 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet54/1 - HRAOISD2-1-6_Ethernet50 = 'up' | PASS | - |
| 559 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet6 - 20/2-226-D037 = 'up' | PASS | - |
| 560 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet7 - LIBERTPOWER = 'up' | PASS | - |
| 561 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet8 - UP_SINCE_04-16-2018 = 'up' | PASS | - |
| 562 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet9 - VACANT_SINCE_12-21-2017 = 'up' | PASS | - |
| 563 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel49 - CORES_Po5 = 'up' | PASS | - |
| 564 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel51 - MLAG_PEER_HRAOISD2-1-0_Po51 = 'up' | PASS | - |
| 565 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel531 - HRAOISD2-1-2_Po49 = 'up' | PASS | - |
| 566 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel532 - HRAOISD2-1-3_Po49 = 'up' | PASS | - |
| 567 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel533 - HRAOISD2-1-4_Po49 = 'up' | PASS | - |
| 568 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel534 - HRAOISD2-1-5_Po49 = 'up' | PASS | - |
| 569 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel541 - HRAOISD2-1-6_Po49 = 'up' | PASS | - |
| 570 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan4094 - MLAG_PEER = 'up' | PASS | - |
| 571 | HRAOISD2-1-1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan5 - Inband Management = 'up' | PASS | - |
| 572 | HRAOISD2-1-1 | MLAG | VerifyMlagConfigSanity | Verifies there are no MLAG config-sanity inconsistencies. | - | PASS | - |
| 573 | HRAOISD2-1-1 | MLAG | VerifyMlagInterfaces | Verifies there are no inactive or active-partial MLAG ports. | - | PASS | - |
| 574 | HRAOISD2-1-1 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 575 | HRAOISD2-1-1 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | - | PASS | - |
| 576 | HRAOISD2-1-1 | Software | VerifyEOSVersion | Verifies the EOS version of the device. | - | PASS | - |
| 577 | HRAOISD2-1-1 | Software | VerifyTerminAttrVersion | Verifies the TerminAttr version of the device. | - | PASS | - |
| 578 | HRAOISD2-1-1 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | PASS | - |
| 579 | HRAOISD2-1-2 | Configuration | VerifyRunningConfigDiffs | Verifies there is no difference between the running-config and the startup-config | - | PASS | - |
| 580 | HRAOISD2-1-2 | Configuration | VerifyZeroTouch | Verifies ZeroTouch is disabled | - | PASS | - |
| 581 | HRAOISD2-1-2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet49 - Remote: HRAOISD2-1-0 Ethernet53/1 | PASS | - |
| 582 | HRAOISD2-1-2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet50 - Remote: HRAOISD2-1-1 Ethernet53/1 | PASS | - |
| 583 | HRAOISD2-1-2 | Connectivity | VerifyReachability | Test the network reachability to one or many destination IP(s). | TEST PING TO INTERNET 8.8.8.8 | PASS | - |
| 584 | HRAOISD2-1-2 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on vEOS-lab. |
| 585 | HRAOISD2-1-2 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on vEOS-lab. |
| 586 | HRAOISD2-1-2 | Hardware | VerifyTemperature | Verifies the device temperature. | - | SKIPPED | VerifyTemperature test is not supported on vEOS-lab. |
| 587 | HRAOISD2-1-2 | Hardware | VerifyTransceiversManufacturers | Verifies if all transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on vEOS-lab. |
| 588 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet1 - UP_SINCE_06-01-2018 = 'up' | PASS | - |
| 589 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet10 - VACANT_SINCE_07-20-2016 = 'up' | PASS | - |
| 590 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet11 - 20/2-226/126D/ISD-Ravi = 'up' | PASS | - |
| 591 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet12 - 20/2-226/125D = 'up' | PASS | - |
| 592 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet13 - 20/2-226/125D = 'up' | PASS | - |
| 593 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet14 - 20/2/226/127D = 'up' | PASS | - |
| 594 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet15 - VACANT_SINCE_12-18-2017 = 'up' | PASS | - |
| 595 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet16 - VACANT_SINCE_11-09-2017 = 'up' | PASS | - |
| 596 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet17 - VACANT_SINCE_12-08-2017 = 'up' | PASS | - |
| 597 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet18 - 20/2/226/129D = 'up' | PASS | - |
| 598 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet19 - 20/2-226/106D_TONYs_VC_System = 'up' | PASS | - |
| 599 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet2 - 20/2-226/D059 = 'up' | PASS | - |
| 600 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet20 - 20/2/226-130D = 'up' | PASS | - |
| 601 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet21 - 20/2/226-132D = 'up' | PASS | - |
| 602 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet22 - VACANT_SINCE_10-20-2017 = 'up' | PASS | - |
| 603 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet23 - Interworking-Labs = 'up' | PASS | - |
| 604 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet24 - 20/2/226/228D(2M)_ECHAN = 'up' | PASS | - |
| 605 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet25 - 20/2-226/85D() = 'up' | PASS | - |
| 606 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet26 - 20/2-226/D061 = 'up' | PASS | - |
| 607 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet27 - VACANT_SINCE_08-18-2017 = 'up' | PASS | - |
| 608 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet28 - 20/2/226-135D = 'up' | PASS | - |
| 609 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet29 - 20/2-226/D062 = 'up' | PASS | - |
| 610 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet3 - VACANT_SINCE_11-10-2017 = 'up' | PASS | - |
| 611 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet30 - 20/2-226/135D = 'up' | PASS | - |
| 612 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet31 - 20/2-226/112D = 'up' | PASS | - |
| 613 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet32 - UP_SINCE_01-03-2018 = 'up' | PASS | - |
| 614 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet33 - VACANT_SINCE_12-11-2017 = 'up' | PASS | - |
| 615 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet34 - UP_SINCE_01-26-2018 = 'up' | PASS | - |
| 616 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet35 - 20/226/114D = 'up' | PASS | - |
| 617 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet36 - VACANT_SINCE_06-06-2016 = 'up' | PASS | - |
| 618 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet37 - VACANT_SINCE_06-06-2016 = 'up' | PASS | - |
| 619 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet38 - 20/2-226/139D = 'up' | PASS | - |
| 620 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet39 - VACANT_SINCE_06-06-2016 = 'up' | PASS | - |
| 621 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet4 - VACANT_SINCE_06-06-2016 = 'up' | PASS | - |
| 622 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet40 - VACANT_SINCE_11-09-2017 = 'up' | PASS | - |
| 623 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet41 - UP_SINCE_04-26-2018 = 'up' | PASS | - |
| 624 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet42 - 20/2-226/070D = 'up' | PASS | - |
| 625 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet43 - 20/2/228-307D-ISD/PRINTER = 'up' | PASS | - |
| 626 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet44 - VACANT_SINCE_11-28-2017 = 'up' | PASS | - |
| 627 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet45 - VACANT_SINCE_06-06-2016 = 'up' | PASS | - |
| 628 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet46 - VACANT_SINCE_11-01-2017 = 'up' | PASS | - |
| 629 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet47 - VACANT_SINCE_12-11-2017 = 'up' | PASS | - |
| 630 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet48 - VACANT_SINCE_03-06-2017 = 'up' | PASS | - |
| 631 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet49 - HRAOISD2-1-0_Ethernet53/1 = 'up' | PASS | - |
| 632 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet5 - 20/2-226/D060 = 'up' | PASS | - |
| 633 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet50 - HRAOISD2-1-1_Ethernet53/1 = 'up' | PASS | - |
| 634 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet6 - UP_SINCE_05-18-2018 = 'up' | PASS | - |
| 635 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet7 - VACANT_SINCE_12-08-2017 = 'up' | PASS | - |
| 636 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet8 - UP_SINCE_05-15-2018 = 'up' | PASS | - |
| 637 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet9 - 20/2-226/101D = 'up' | PASS | - |
| 638 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel49 - ISD2-SPINES_Po531 = 'up' | PASS | - |
| 639 | HRAOISD2-1-2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan5 - Inband Management = 'up' | PASS | - |
| 640 | HRAOISD2-1-2 | MLAG | VerifyMlagConfigSanity | Verifies there are no MLAG config-sanity inconsistencies. | - | SKIPPED | MLAG is disabled |
| 641 | HRAOISD2-1-2 | MLAG | VerifyMlagInterfaces | Verifies there are no inactive or active-partial MLAG ports. | - | SKIPPED | MLAG is disabled |
| 642 | HRAOISD2-1-2 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | SKIPPED | MLAG is disabled |
| 643 | HRAOISD2-1-2 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | - | PASS | - |
| 644 | HRAOISD2-1-2 | Software | VerifyEOSVersion | Verifies the EOS version of the device. | - | PASS | - |
| 645 | HRAOISD2-1-2 | Software | VerifyTerminAttrVersion | Verifies the TerminAttr version of the device. | - | PASS | - |
| 646 | HRAOISD2-1-2 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | PASS | - |
| 647 | HRAOISD2-1-3 | Configuration | VerifyRunningConfigDiffs | Verifies there is no difference between the running-config and the startup-config | - | PASS | - |
| 648 | HRAOISD2-1-3 | Configuration | VerifyZeroTouch | Verifies ZeroTouch is disabled | - | PASS | - |
| 649 | HRAOISD2-1-3 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet49 - Remote: HRAOISD2-1-0 Ethernet53/2 | PASS | - |
| 650 | HRAOISD2-1-3 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet50 - Remote: HRAOISD2-1-1 Ethernet53/2 | PASS | - |
| 651 | HRAOISD2-1-3 | Connectivity | VerifyReachability | Test the network reachability to one or many destination IP(s). | TEST PING TO INTERNET 8.8.8.8 | PASS | - |
| 652 | HRAOISD2-1-3 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on vEOS-lab. |
| 653 | HRAOISD2-1-3 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on vEOS-lab. |
| 654 | HRAOISD2-1-3 | Hardware | VerifyTemperature | Verifies the device temperature. | - | SKIPPED | VerifyTemperature test is not supported on vEOS-lab. |
| 655 | HRAOISD2-1-3 | Hardware | VerifyTransceiversManufacturers | Verifies if all transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on vEOS-lab. |
| 656 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet1 - VACANT_SINCE_06-06-2016 = 'up' | PASS | - |
| 657 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet10 - VACANT_SINCE_11-09-2017 = 'up' | PASS | - |
| 658 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet11 - VACANT_SINCE_11-09-2017 = 'up' | PASS | - |
| 659 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet12 - VACANT_SINCE_06-06-2016 = 'up' | PASS | - |
| 660 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet13 - VACANT_SINCE_07-11-2016 = 'up' | PASS | - |
| 661 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet14 - VACANT_SINCE_11-10-2017 = 'up' | PASS | - |
| 662 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet15 - UP_SINCE_05-18-2018 = 'up' | PASS | - |
| 663 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet16 - VACANT_SINCE_06-06-2016 = 'up' | PASS | - |
| 664 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet17 - 20/2-226/153D = 'up' | PASS | - |
| 665 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet18 - 20/2-226/177D = 'up' | PASS | - |
| 666 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet19 - 220/2/226-201D = 'up' | PASS | - |
| 667 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet2 - VACANT_SINCE_09-05-2017 = 'up' | PASS | - |
| 668 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet20 - VACANT_SINCE_11-06-2017 = 'up' | PASS | - |
| 669 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet21 - 20/2-226/155D = 'up' | PASS | - |
| 670 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet22 - VACANT_SINCE_06-06-2016 = 'up' | PASS | - |
| 671 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet23 - UP_SINCE_02-22-2018 = 'up' | PASS | - |
| 672 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet24 - VACANT_SINCE_06-06-2016 = 'up' | PASS | - |
| 673 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet25 - ERIC_CHAN_DESKTOP_IN_TESTLAB = 'up' | PASS | - |
| 674 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet26 - 20/2-226/181D = 'up' | PASS | - |
| 675 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet27 - VACANT_SINCE_11-22-2017 = 'up' | PASS | - |
| 676 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet28 - 20/2-226/182D = 'up' | PASS | - |
| 677 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet29 - VACANT_SINCE_07-31-2017 = 'up' | PASS | - |
| 678 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet3 - VACANT_SINCE_06-06-2016 = 'up' | PASS | - |
| 679 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet30 - VACANT_SINCE_03-07-2017 = 'up' | PASS | - |
| 680 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet31 - 20/2-226/013D = 'up' | PASS | - |
| 681 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet32 - 20/2/226-184D(ISD-5-N_Geoff_Gratz_#1_Black) = 'up' | PASS | - |
| 682 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet33 - VACANT_SINCE_12-07-2017 = 'up' | PASS | - |
| 683 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet34 - 20/2-226/185D = 'up' | PASS | - |
| 684 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet35 - UP_SINCE_05-29-2018 = 'up' | PASS | - |
| 685 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet36 - VACANT_SINCE_06-06-2016 = 'up' | PASS | - |
| 686 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet37 - 20/2-226/163D = 'up' | PASS | - |
| 687 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet38 - 20/2/226-187D = 'up' | PASS | - |
| 688 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet39 - 20/2-226/164D = 'up' | PASS | - |
| 689 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet4 - UP_SINCE_02-22-2018 = 'up' | PASS | - |
| 690 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet40 - 20/2/226-188D(ISD-5-O) = 'up' | PASS | - |
| 691 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet41 - 20/2-226/165D = 'up' | PASS | - |
| 692 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet42 - 20/2/226-189D(ISD-5-N_Geoff_Gratz_#2_Green) = 'up' | PASS | - |
| 693 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet43 - VACANT_SINCE_08-17-2017 = 'up' | PASS | - |
| 694 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet44 - 20/2-226/190D,4-N = 'up' | PASS | - |
| 695 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet45 - VACANT_SINCE_11-17-2017 = 'up' | PASS | - |
| 696 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet46 - 20/2/226-191D = 'up' | PASS | - |
| 697 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet47 - DEISHRAOExperienceLaptop#2_ToddRodrick_ISDTestlab/R2/U12(HRARAYL307539P) = 'up' | PASS | - |
| 698 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet48 - 20/2/226-192D = 'up' | PASS | - |
| 699 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet49 - HRAOISD2-1-0_Ethernet53/2 = 'up' | PASS | - |
| 700 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet5 - VACANT_SINCE_11-09-2017 = 'up' | PASS | - |
| 701 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet50 - HRAOISD2-1-1_Ethernet53/2 = 'up' | PASS | - |
| 702 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet6 - VACANT_SINCE_06-06-2016 = 'up' | PASS | - |
| 703 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet7 - 20/2-226/148D = 'up' | PASS | - |
| 704 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet8 - VACANT_SINCE_11-09-2017 = 'up' | PASS | - |
| 705 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet9 - (6L) = 'up' | PASS | - |
| 706 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel49 - ISD2-SPINES_Po532 = 'up' | PASS | - |
| 707 | HRAOISD2-1-3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan5 - Inband Management = 'up' | PASS | - |
| 708 | HRAOISD2-1-3 | MLAG | VerifyMlagConfigSanity | Verifies there are no MLAG config-sanity inconsistencies. | - | SKIPPED | MLAG is disabled |
| 709 | HRAOISD2-1-3 | MLAG | VerifyMlagInterfaces | Verifies there are no inactive or active-partial MLAG ports. | - | SKIPPED | MLAG is disabled |
| 710 | HRAOISD2-1-3 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | SKIPPED | MLAG is disabled |
| 711 | HRAOISD2-1-3 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | - | PASS | - |
| 712 | HRAOISD2-1-3 | Software | VerifyEOSVersion | Verifies the EOS version of the device. | - | PASS | - |
| 713 | HRAOISD2-1-3 | Software | VerifyTerminAttrVersion | Verifies the TerminAttr version of the device. | - | PASS | - |
| 714 | HRAOISD2-1-3 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | PASS | - |
| 715 | HRAOISD2-1-4 | Configuration | VerifyRunningConfigDiffs | Verifies there is no difference between the running-config and the startup-config | - | PASS | - |
| 716 | HRAOISD2-1-4 | Configuration | VerifyZeroTouch | Verifies ZeroTouch is disabled | - | PASS | - |
| 717 | HRAOISD2-1-4 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet49 - Remote: HRAOISD2-1-0 Ethernet53/3 | PASS | - |
| 718 | HRAOISD2-1-4 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet50 - Remote: HRAOISD2-1-1 Ethernet53/3 | PASS | - |
| 719 | HRAOISD2-1-4 | Connectivity | VerifyReachability | Test the network reachability to one or many destination IP(s). | TEST PING TO INTERNET 8.8.8.8 | PASS | - |
| 720 | HRAOISD2-1-4 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on vEOS-lab. |
| 721 | HRAOISD2-1-4 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on vEOS-lab. |
| 722 | HRAOISD2-1-4 | Hardware | VerifyTemperature | Verifies the device temperature. | - | SKIPPED | VerifyTemperature test is not supported on vEOS-lab. |
| 723 | HRAOISD2-1-4 | Hardware | VerifyTransceiversManufacturers | Verifies if all transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on vEOS-lab. |
| 724 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet1 - ISD-4N = 'up' | PASS | - |
| 725 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet10 - 20/2-226/221D = 'up' | PASS | - |
| 726 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet11 - UP_SINCE_05-03-2018 = 'up' | PASS | - |
| 727 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet12 - VACANT_SINCE_11-15-2017 = 'up' | PASS | - |
| 728 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet13 - 20/2-226/199D = 'up' | PASS | - |
| 729 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet14 - VACANT_SINCE_11-17-2017 = 'up' | PASS | - |
| 730 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet15 - VACANT_SINCE_11-27-2017 = 'up' | PASS | - |
| 731 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet16 - 20/2-226/224D = 'up' | PASS | - |
| 732 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet17 - VACANT_SINCE_11-27-2017 = 'up' | PASS | - |
| 733 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet18 - VACANT_SINCE_06-06-2016 = 'up' | PASS | - |
| 734 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet19 - UP_SINCE_02-23-2018 = 'up' | PASS | - |
| 735 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet2 - UP_SINCE_06-01-2018 = 'up' | PASS | - |
| 736 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet20 - VACANT_SINCE_06-06-2016 = 'up' | PASS | - |
| 737 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet21 - VACANT_SINCE_03-22-2017 = 'up' | PASS | - |
| 738 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet22 - UP_SINCE_05-14-2018 = 'up' | PASS | - |
| 739 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet23 - 20/2-226/204D = 'up' | PASS | - |
| 740 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet24 - VACANT_SINCE_11-10-2017 = 'up' | PASS | - |
| 741 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet25 - VACANT_SINCE_01-30-2017 = 'up' | PASS | - |
| 742 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet26 - 20/2-226/229D = 'up' | PASS | - |
| 743 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet27 - UP_SINCE_02-28-2018 = 'up' | PASS | - |
| 744 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet28 - VACANT_SINCE_06-28-2017 = 'up' | PASS | - |
| 745 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet29 - VACANT_SINCE_11-09-2016 = 'up' | PASS | - |
| 746 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet3 - 20/2/226-194D(ISD-5-N_Geoff_Gratz_#3_Red) = 'up' | PASS | - |
| 747 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet30 - VACANT_SINCE_11-08-2017 = 'up' | PASS | - |
| 748 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet31 - VACANT_SINCE_12-11-2017 = 'up' | PASS | - |
| 749 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet32 - COBO-MGMT-port = 'up' | PASS | - |
| 750 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet33 - VACANT_SINCE_06-30-2016 = 'up' | PASS | - |
| 751 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet34 - Courtyard-MGMT-port = 'up' | PASS | - |
| 752 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet35 - VACANT_SINCE_11-21-2017 = 'up' | PASS | - |
| 753 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet36 - VACANT_SINCE_09-07-2016 = 'up' | PASS | - |
| 754 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet37 - 20/2-226/211D = 'up' | PASS | - |
| 755 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet38 - 15A = 'up' | PASS | - |
| 756 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet39 - UP_SINCE_04-10-2018 = 'up' | PASS | - |
| 757 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet4 - 20/2-226/218D = 'up' | PASS | - |
| 758 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet40 - VACANT_SINCE_10-01-2016 = 'up' | PASS | - |
| 759 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet41 - 20/2-226/213D = 'up' | PASS | - |
| 760 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet42 - VACANT_SINCE_10-01-2016 = 'up' | PASS | - |
| 761 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet43 - UP_SINCE_05-18-2018 = 'up' | PASS | - |
| 762 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet44 - VACANT_SINCE_11-01-2017 = 'up' | PASS | - |
| 763 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet45 - UP_SINCE_01-04-2018 = 'up' | PASS | - |
| 764 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet46 - VACANT_SINCE_06-06-2016 = 'up' | PASS | - |
| 765 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet47 - DEISHRAOExperienceLaptop#1_ToddRodrick_ISDTestlab/R2/U12(HRARAYL138837L) = 'up' | PASS | - |
| 766 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet48 - VACANT_SINCE_06-06-2016 = 'up' | PASS | - |
| 767 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet49 - HRAOISD2-1-0_Ethernet53/3 = 'up' | PASS | - |
| 768 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet5 - VACANT_SINCE_11-08-2017 = 'up' | PASS | - |
| 769 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet50 - HRAOISD2-1-1_Ethernet53/3 = 'up' | PASS | - |
| 770 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet6 - VACANT_SINCE_10-20-2016 = 'up' | PASS | - |
| 771 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet7 - 20/2/226-196D(ISD-5-O) = 'up' | PASS | - |
| 772 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet8 - VACANT_SINCE_06-30-2016 = 'up' | PASS | - |
| 773 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet9 - VACANT_SINCE_12-07-2017 = 'up' | PASS | - |
| 774 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel49 - ISD2-SPINES_Po533 = 'up' | PASS | - |
| 775 | HRAOISD2-1-4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan5 - Inband Management = 'up' | PASS | - |
| 776 | HRAOISD2-1-4 | MLAG | VerifyMlagConfigSanity | Verifies there are no MLAG config-sanity inconsistencies. | - | SKIPPED | MLAG is disabled |
| 777 | HRAOISD2-1-4 | MLAG | VerifyMlagInterfaces | Verifies there are no inactive or active-partial MLAG ports. | - | SKIPPED | MLAG is disabled |
| 778 | HRAOISD2-1-4 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | SKIPPED | MLAG is disabled |
| 779 | HRAOISD2-1-4 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | - | PASS | - |
| 780 | HRAOISD2-1-4 | Software | VerifyEOSVersion | Verifies the EOS version of the device. | - | PASS | - |
| 781 | HRAOISD2-1-4 | Software | VerifyTerminAttrVersion | Verifies the TerminAttr version of the device. | - | PASS | - |
| 782 | HRAOISD2-1-4 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | PASS | - |
| 783 | HRAOISD2-1-5 | Configuration | VerifyRunningConfigDiffs | Verifies there is no difference between the running-config and the startup-config | - | PASS | - |
| 784 | HRAOISD2-1-5 | Configuration | VerifyZeroTouch | Verifies ZeroTouch is disabled | - | PASS | - |
| 785 | HRAOISD2-1-5 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet49 - Remote: HRAOISD2-1-0 Ethernet53/4 | PASS | - |
| 786 | HRAOISD2-1-5 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet50 - Remote: HRAOISD2-1-1 Ethernet53/4 | PASS | - |
| 787 | HRAOISD2-1-5 | Connectivity | VerifyReachability | Test the network reachability to one or many destination IP(s). | TEST PING TO INTERNET 8.8.8.8 | PASS | - |
| 788 | HRAOISD2-1-5 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on vEOS-lab. |
| 789 | HRAOISD2-1-5 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on vEOS-lab. |
| 790 | HRAOISD2-1-5 | Hardware | VerifyTemperature | Verifies the device temperature. | - | SKIPPED | VerifyTemperature test is not supported on vEOS-lab. |
| 791 | HRAOISD2-1-5 | Hardware | VerifyTransceiversManufacturers | Verifies if all transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on vEOS-lab. |
| 792 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet1 - VACANT_SINCE_07-01-2016 = 'up' | PASS | - |
| 793 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet10 - 20/2-226/265D = 'up' | PASS | - |
| 794 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet11 - 20/2-226/246D = 'up' | PASS | - |
| 795 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet12 - UP_SINCE_06-01-2018 = 'up' | PASS | - |
| 796 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet13 - 20/2-226/199D = 'up' | PASS | - |
| 797 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet14 - 20/2-226/267D = 'up' | PASS | - |
| 798 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet15 - UP_SINCE_03-27-2018 = 'up' | PASS | - |
| 799 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet16 - UP_SINCE_06-01-2018 = 'up' | PASS | - |
| 800 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet17 - 20/2-226/249D = 'up' | PASS | - |
| 801 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet18 - VACANT_SINCE_12-01-2017 = 'up' | PASS | - |
| 802 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet19 - UP_SINCE_01-24-2018 = 'up' | PASS | - |
| 803 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet2 - (AP3700_ISD_AP4) = 'up' | PASS | - |
| 804 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet20 - UP_SINCE_06-04-2018 = 'up' | PASS | - |
| 805 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet21 - 20/2-226/251D = 'up' | PASS | - |
| 806 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet22 - 20/2-231/003D = 'up' | PASS | - |
| 807 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet23 - VACANT_SINCE_01-11-2017 = 'up' | PASS | - |
| 808 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet24 - UP_SINCE_05-22-2018 = 'up' | PASS | - |
| 809 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet25 - UP_SINCE_05-05-2018 = 'up' | PASS | - |
| 810 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet26 - UP_SINCE_05-09-2018 = 'up' | PASS | - |
| 811 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet27 - VACANT_SINCE_06-06-2016 = 'up' | PASS | - |
| 812 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet28 - 20/2-231/006D(ISD_MTG_RM_VeloCloud) = 'up' | PASS | - |
| 813 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet29 - VACANT_SINCE_11-09-2017 = 'up' | PASS | - |
| 814 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet3 - 20/2/226/242D(2M)_ECHAN = 'up' | PASS | - |
| 815 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet30 - VACANT_SINCE_11-13-2017 = 'up' | PASS | - |
| 816 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet31 - VACANT_SINCE_06-06-2016 = 'up' | PASS | - |
| 817 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet32 - VACANT_SINCE_12-02-2016 = 'up' | PASS | - |
| 818 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet33 - VACANT_SINCE_11-10-2017 = 'up' | PASS | - |
| 819 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet34 - VACANT_SINCE_10-24-2017 = 'up' | PASS | - |
| 820 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet35 - VACANT_SINCE_06-06-2016 = 'up' | PASS | - |
| 821 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet36 - VACANT_SINCE_05-04-2017 = 'up' | PASS | - |
| 822 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet37 - VACANT_SINCE_11-14-2017 = 'up' | PASS | - |
| 823 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet38 - UP_SINCE_05-03-2018 = 'up' | PASS | - |
| 824 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet39 - VACANT_SINCE_06-06-2016 = 'up' | PASS | - |
| 825 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet4 - VACANT_SINCE_06-06-2016 = 'up' | PASS | - |
| 826 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet40 - UP_SINCE_04-16-2018 = 'up' | PASS | - |
| 827 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet41 - 20/2-226/261D = 'up' | PASS | - |
| 828 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet42 - 20/2-226/D-286 = 'up' | PASS | - |
| 829 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet43 - UP_SINCE_01-24-2018 = 'up' | PASS | - |
| 830 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet44 - UP_SINCE_06-01-2018 = 'up' | PASS | - |
| 831 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet45 - 20/2-226/263D = 'up' | PASS | - |
| 832 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet46 - 20/2-226/D-287 = 'up' | PASS | - |
| 833 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet47 - UP_SINCE_05-25-2018 = 'up' | PASS | - |
| 834 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet48 - UP_SINCE_01-17-2018 = 'up' | PASS | - |
| 835 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet49 - HRAOISD2-1-0_Ethernet53/4 = 'up' | PASS | - |
| 836 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet5 - 20/2/226/243D = 'up' | PASS | - |
| 837 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet50 - HRAOISD2-1-1_Ethernet53/4 = 'up' | PASS | - |
| 838 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet6 - (AP3700_ISD_AP9) = 'up' | PASS | - |
| 839 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet7 - 20/2-226/244D = 'up' | PASS | - |
| 840 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet8 - VACANT_SINCE_06-06-2016 = 'up' | PASS | - |
| 841 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet9 - VACANT_SINCE_04-20-2017 = 'up' | PASS | - |
| 842 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel49 - ISD2-SPINES_Po534 = 'up' | PASS | - |
| 843 | HRAOISD2-1-5 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan5 - Inband Management = 'up' | PASS | - |
| 844 | HRAOISD2-1-5 | MLAG | VerifyMlagConfigSanity | Verifies there are no MLAG config-sanity inconsistencies. | - | SKIPPED | MLAG is disabled |
| 845 | HRAOISD2-1-5 | MLAG | VerifyMlagInterfaces | Verifies there are no inactive or active-partial MLAG ports. | - | SKIPPED | MLAG is disabled |
| 846 | HRAOISD2-1-5 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | SKIPPED | MLAG is disabled |
| 847 | HRAOISD2-1-5 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | - | PASS | - |
| 848 | HRAOISD2-1-5 | Software | VerifyEOSVersion | Verifies the EOS version of the device. | - | PASS | - |
| 849 | HRAOISD2-1-5 | Software | VerifyTerminAttrVersion | Verifies the TerminAttr version of the device. | - | PASS | - |
| 850 | HRAOISD2-1-5 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | PASS | - |
| 851 | HRAOISD2-1-6 | Configuration | VerifyRunningConfigDiffs | Verifies there is no difference between the running-config and the startup-config | - | PASS | - |
| 852 | HRAOISD2-1-6 | Configuration | VerifyZeroTouch | Verifies ZeroTouch is disabled | - | PASS | - |
| 853 | HRAOISD2-1-6 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet49 - Remote: HRAOISD2-1-0 Ethernet54/1 | PASS | - |
| 854 | HRAOISD2-1-6 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet50 - Remote: HRAOISD2-1-1 Ethernet54/1 | PASS | - |
| 855 | HRAOISD2-1-6 | Connectivity | VerifyReachability | Test the network reachability to one or many destination IP(s). | TEST PING TO INTERNET 8.8.8.8 | PASS | - |
| 856 | HRAOISD2-1-6 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on vEOS-lab. |
| 857 | HRAOISD2-1-6 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on vEOS-lab. |
| 858 | HRAOISD2-1-6 | Hardware | VerifyTemperature | Verifies the device temperature. | - | SKIPPED | VerifyTemperature test is not supported on vEOS-lab. |
| 859 | HRAOISD2-1-6 | Hardware | VerifyTransceiversManufacturers | Verifies if all transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on vEOS-lab. |
| 860 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet1 - UP_SINCE_05-23-2018 = 'up' | PASS | - |
| 861 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet10 - 20/2-226/297D = 'up' | PASS | - |
| 862 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet11 - 20/2-228/274D = 'up' | PASS | - |
| 863 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet12 - UP_SINCE_01-09-2018 = 'up' | PASS | - |
| 864 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet13 - UP_SINCE_01-24-2018 = 'up' | PASS | - |
| 865 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet14 - UP_SINCE_05-18-2018 = 'up' | PASS | - |
| 866 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet15 - VACANT_SINCE_06-06-2016 = 'up' | PASS | - |
| 867 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet16 - UP_SINCE_03-19-2018 = 'up' | PASS | - |
| 868 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet17 - 20/2-226/277D = 'up' | PASS | - |
| 869 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet18 - UP_SINCE_06-01-2018 = 'up' | PASS | - |
| 870 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet19 - 20/2-226/278D/CHARLES-A-DESK = 'up' | PASS | - |
| 871 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet2 - VACANT_SINCE_06-06-2016 = 'up' | PASS | - |
| 872 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet20 - 20/2-228/298D = 'up' | PASS | - |
| 873 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet21 - 20/2-228/279D = 'up' | PASS | - |
| 874 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet22 - UP_SINCE_01-05-2018 = 'up' | PASS | - |
| 875 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet23 - 20/2-228/280D = 'up' | PASS | - |
| 876 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet24 - 20/2-228/299D = 'up' | PASS | - |
| 877 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet25 - TIE-LINE/09 = 'up' | PASS | - |
| 878 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet26 - VACANT_SINCE_10-11-2016 = 'up' | PASS | - |
| 879 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet27 - TIELINE-10 = 'up' | PASS | - |
| 880 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet28 - VACANT_SINCE_11-03-2017 = 'up' | PASS | - |
| 881 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet29 - VACANT_SINCE_06-23-2016 = 'up' | PASS | - |
| 882 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet3 - 20/2-226/270D = 'up' | PASS | - |
| 883 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet30 - VACANT_SINCE_11-03-2017 = 'up' | PASS | - |
| 884 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet31 - VACANT_SINCE_12-22-2017 = 'up' | PASS | - |
| 885 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet32 - VACANT_SINCE_12-20-2017 = 'up' | PASS | - |
| 886 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet33 - VACANT_SINCE_12-13-2017 = 'up' | PASS | - |
| 887 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet34 - VACANT_SINCE_12-20-2017 = 'up' | PASS | - |
| 888 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet35 - VACANT_SINCE_12-01-2017 = 'up' | PASS | - |
| 889 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet36 - VACANT_SINCE_06-06-2016 = 'up' | PASS | - |
| 890 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet37 - 20/2-228/286D = 'up' | PASS | - |
| 891 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet38 - 20/2-228/287D = 'up' | PASS | - |
| 892 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet39 - 20/2-228/288D = 'up' | PASS | - |
| 893 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet4 - Help_Desk_Test_Bench_Switch(HRAO_Helpdesk_Bench) = 'up' | PASS | - |
| 894 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet40 - VACANT_SINCE_11-27-2017 = 'up' | PASS | - |
| 895 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet41 - 20/2-228/289D = 'up' | PASS | - |
| 896 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet42 - VACANT_SINCE_11-22-2017 = 'up' | PASS | - |
| 897 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet43 - 20/2-226/290D = 'up' | PASS | - |
| 898 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet44 - ISD-CONFERENCE-CLOCK = 'up' | PASS | - |
| 899 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet45 - VACANT_SINCE_06-06-2016 = 'up' | PASS | - |
| 900 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet46 - laptop-asset/914327 = 'up' | PASS | - |
| 901 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet47 - Laptop-asset-311234 = 'up' | PASS | - |
| 902 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet48 - VACANT_SINCE_06-06-2016 = 'up' | PASS | - |
| 903 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet49 - HRAOISD2-1-0_Ethernet54/1 = 'up' | PASS | - |
| 904 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet5 - 20/2-228/271D = 'up' | PASS | - |
| 905 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet50 - HRAOISD2-1-1_Ethernet54/1 = 'up' | PASS | - |
| 906 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet6 - 20/2-226/295D = 'up' | PASS | - |
| 907 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet7 - 20/2-228/272D = 'up' | PASS | - |
| 908 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet8 - 20/2-226/296D = 'up' | PASS | - |
| 909 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet9 - 20/2/226/273D(3C_BCoy) = 'up' | PASS | - |
| 910 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel49 - ISD2-SPINES_Po541 = 'up' | PASS | - |
| 911 | HRAOISD2-1-6 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan5 - Inband Management = 'up' | PASS | - |
| 912 | HRAOISD2-1-6 | MLAG | VerifyMlagConfigSanity | Verifies there are no MLAG config-sanity inconsistencies. | - | SKIPPED | MLAG is disabled |
| 913 | HRAOISD2-1-6 | MLAG | VerifyMlagInterfaces | Verifies there are no inactive or active-partial MLAG ports. | - | SKIPPED | MLAG is disabled |
| 914 | HRAOISD2-1-6 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | SKIPPED | MLAG is disabled |
| 915 | HRAOISD2-1-6 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | - | PASS | - |
| 916 | HRAOISD2-1-6 | Software | VerifyEOSVersion | Verifies the EOS version of the device. | - | PASS | - |
| 917 | HRAOISD2-1-6 | Software | VerifyTerminAttrVersion | Verifies the TerminAttr version of the device. | - | PASS | - |
| 918 | HRAOISD2-1-6 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | PASS | - |
