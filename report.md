using kit 107.3.0 (e8b660c96183f4a35f12f5ff75e37756ae6aee3b) with Isaac Sim 5.1

ISAACSIM --enable uosm.isaac.px4_bridge


Recordings and screenshots are available in the following Google Drive folder:
https://drive.google.com/drive/folders/1dDV8QXW2VMLbV2tpHYmBT32S8ixZ61ms?usp=sharing

Logs below:

```bash

|---------------------------------------------------------------------------------------------|
| Driver Version: 580.95.05     | Graphics API: Vulkan
|=============================================================================================|
| GPU | Name                             | Active | LDA | GPU Memory | Vendor-ID | LUID       |
|     |                                  |        |     |            | Device-ID | UUID       |
|     |                                  |        |     |            | Bus-ID    |            |
|---------------------------------------------------------------------------------------------|
| 0   | NVIDIA GeForce RTX 5070 Ti       | Yes: 0 |     | 16303   MB | 10de      | 0          |
|     |                                  |        |     |            | 2c05      | 3290c917.. |
|     |                                  |        |     |            | 1         |            |
|---------------------------------------------------------------------------------------------|
| 1   | AMD Radeon Graphics (RADV RAPH.. |        |     | 42988   MB | 1002      | 0          |
|     |                                  |        |     |            | 164e      | 00000000.. |
|     |                                  |        |     |            | d         |            |
|=============================================================================================|
| OS: 24.04.3 LTS (Noble Numbat) ubuntu, Version: 24.04.3, Kernel: 6.14.0-36-generic
| XServer Vendor: The X.Org Foundation, XServer Version: 12101011 (1.21.1.11)
| Processor: AMD Ryzen 9 7900X 12-Core Processor
| Cores: 12 | Logical Cores: 24
|---------------------------------------------------------------------------------------------|
| Total Memory (MB): 127940 | Free Memory: 122515
| Total Page/Swap (MB): 8191 | Free Page/Swap: 8191
|---------------------------------------------------------------------------------------------|



[1764156448.309636] info     | UDPv4AgentLinux.cpp | init                     | running...             | port: 8888
[1764156448.309803] info     | Root.cpp           | set_verbose_level        | logger setup           | verbose_level: 4
INFO  [px4] instance: 0

______  __   __    ___ 
| ___ \ \ \ / /   /   |
| |_/ /  \ V /   / /| |
|  __/   /   \  / /_| |
| |     / /^\ \ \___  |
\_|     \/   \/     |_/

px4 starting.

INFO  [px4] startup script: /bin/sh /home/ava/kit-extension-template-cpp/_build/linux-x86_64/release/exts/uosINFO  [init] found model autostart file as SYS_AUTOSTART=22000
INFO  [param] selected parameter default file parameters.bson
INFO  [param] importing from 'parameters.bson'
INFO  [parameters] BSON document size 393 bytes, decoded 393 bytes (INT32:17, FLOAT:3)
INFO  [param] selected parameter backup file parameters_backup.bson
  SYS_AUTOCONFIG: curr: 0 -> new: 1
  SYS_AUTOSTART: curr: 0 -> new: 22000
  SENS_BOARD_X_OFF: curr: 0.0000 -> new: 0.0000
2025-11-26T11:27:28Z [301,261ms] [Warning] [rtx.postprocessing.plugin] DLSS increasing input dimensions: Render resolution of (320, 240) is below minimal input resolution of 300.
  SENS_DPRES_OFF: curr: 0.0000 -> new: 0.0010
INFO  [dataman] data manager file './dataman' size is 7872608 bytes
INFO  [init] PX4_SIM_HOSTNAME: localhost
INFO  [simulator_mavlink] Waiting for simulator to accept connection on TCP port 4560
INFO  [simulator_mavlink] Simulator connected on TCP port 4560.
2025-11-26T11:27:29Z [301,808ms] [Warning] [uosm.isaac.px4.plugin] Client connected on port 4560
COMMAND_LONG - Command: 511, Confirmation: 0, Target system: 0, Target component: 0, Params: 115.000000, 5000.000000, 0.000000, 0.000000, 0.000000, 0.000000, 0.000000
HEARTBEAT - System type: 0, Autopilot: 12
INFO  [lockstep_scheduler] setting initial absolute time to 125000 us
INFO  [commander] LED: open /dev/led0 failed (22)
  UXRCE_DDS_DOM_ID: curr: 0 -> new: 10
INFO  [uxrce_dds_client] init UDP agent IP:127.0.0.1, port:8888
[1764156449.327021] info     | Root.cpp           | create_client            | create                 | client_key: 0x00000001, session_id: 0x81
[1764156449.327052] info     | SessionManager.hpp | establish_session        | session established    | client_key: 0x00000001, address: 127.0.0.1:32668
[1764156449.329812] info     | ProxyClient.cpp    | create_participant       | participant created    | client_key: 0x00000001, participant_id: 0x001(1)
INFO  [mavlink] mode: Normal, data rate: 4000000 B/s on udp port 18570 remote port 14550
INFO  [mavlink] partner IP: 127.0.0.1
INFO  [mavlink] mode: Onboard, data rate: 4000000 B/s on udp port 14580 remote port 14540
INFO  [mavlink] mode: Onboard, data rate: 4000 B/s on udp port 14280 remote port 14030
INFO  [mavlink] mode: Gimbal, data rate: 400000 B/s on udp port 13030 remote port 13280
INFO  [logger] logger started (mode=all)
INFO  [logger] Start file log (type: full)
INFO  [logger] [logger] ./log/2025-11-26/11_27_29.ulg
INFO  [logger] Opened full log file: ./log/2025-11-26/11_27_29.ulg
INFO  [mavlink] MAVLink only on localhost (set param MAV_{i}_BROADCAST = 1 to enable network)
INFO  [mavlink] MAVLink only on localhost (set param MAV_{i}_BROADCAST = 1 to enable network)
INFO  [px4] Startup script returned successfully
INFO  [tone_alarm] home set
INFO  [commander] Ready for takeoff!


INFO  [uxrce_dds_client] synchronized with time offset 1764156464475914us
[1764156474.583980] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x800(2), participant_id: 0x001(1)
[1764156474.584050] info     | ProxyClient.cpp    | create_subscriber        | subscriber created     | client_key: 0x00000001, subscriber_id: 0x800(4), participant_id: 0x001(1)
[1764156474.584417] info     | ProxyClient.cpp    | create_datareader        | datareader created     | client_key: 0x00000001, datareader_id: 0x800(6), subscriber_id: 0x800(4)
[1764156474.584540] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x801(2), participant_id: 0x001(1)
[1764156474.584559] info     | ProxyClient.cpp    | create_subscriber        | subscriber created     | client_key: 0x00000001, subscriber_id: 0x801(4), participant_id: 0x001(1)
[1764156474.584733] info     | ProxyClient.cpp    | create_datareader        | datareader created     | client_key: 0x00000001, datareader_id: 0x801(6), subscriber_id: 0x801(4)
[1764156474.584811] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x802(2), participant_id: 0x001(1)
[1764156474.584826] info     | ProxyClient.cpp    | create_subscriber        | subscriber created     | client_key: 0x00000001, subscriber_id: 0x802(4), participant_id: 0x001(1)
[1764156474.584991] info     | ProxyClient.cpp    | create_datareader        | datareader created     | client_key: 0x00000001, datareader_id: 0x802(6), subscriber_id: 0x802(4)
[1764156474.585073] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x803(2), participant_id: 0x001(1)
[1764156474.585088] info     | ProxyClient.cpp    | create_subscriber        | subscriber created     | client_key: 0x00000001, subscriber_id: 0x803(4), participant_id: 0x001(1)
[1764156474.585266] info     | ProxyClient.cpp    | create_datareader        | datareader created     | client_key: 0x00000001, datareader_id: 0x803(6), subscriber_id: 0x803(4)
[1764156474.585361] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x804(2), participant_id: 0x001(1)
[1764156474.585380] info     | ProxyClient.cpp    | create_subscriber        | subscriber created     | client_key: 0x00000001, subscriber_id: 0x804(4), participant_id: 0x001(1)
[1764156474.585549] info     | ProxyClient.cpp    | create_datareader        | datareader created     | client_key: 0x00000001, datareader_id: 0x804(6), subscriber_id: 0x804(4)
[1764156474.585628] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x805(2), participant_id: 0x001(1)
[1764156474.585656] info     | ProxyClient.cpp    | create_subscriber        | subscriber created     | client_key: 0x00000001, subscriber_id: 0x805(4), participant_id: 0x001(1)
[1764156474.585905] info     | ProxyClient.cpp    | create_datareader        | datareader created     | client_key: 0x00000001, datareader_id: 0x805(6), subscriber_id: 0x805(4)
[1764156474.585978] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x806(2), participant_id: 0x001(1)
[1764156474.585993] info     | ProxyClient.cpp    | create_subscriber        | subscriber created     | client_key: 0x00000001, subscriber_id: 0x806(4), participant_id: 0x001(1)
[1764156474.586147] info     | ProxyClient.cpp    | create_datareader        | datareader created     | client_key: 0x00000001, datareader_id: 0x806(6), subscriber_id: 0x806(4)
[1764156474.586213] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x807(2), participant_id: 0x001(1)
[1764156474.586230] info     | ProxyClient.cpp    | create_subscriber        | subscriber created     | client_key: 0x00000001, subscriber_id: 0x807(4), participant_id: 0x001(1)
[1764156474.586377] info     | ProxyClient.cpp    | create_datareader        | datareader created     | client_key: 0x00000001, datareader_id: 0x807(6), subscriber_id: 0x807(4)
[1764156474.586438] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x808(2), participant_id: 0x001(1)
[1764156474.586458] info     | ProxyClient.cpp    | create_subscriber        | subscriber created     | client_key: 0x00000001, subscriber_id: 0x808(4), participant_id: 0x001(1)
[1764156474.586608] info     | ProxyClient.cpp    | create_datareader        | datareader created     | client_key: 0x00000001, datareader_id: 0x808(6), subscriber_id: 0x808(4)
[1764156474.586677] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x809(2), participant_id: 0x001(1)
[1764156474.586693] info     | ProxyClient.cpp    | create_subscriber        | subscriber created     | client_key: 0x00000001, subscriber_id: 0x809(4), participant_id: 0x001(1)
[1764156474.586838] info     | ProxyClient.cpp    | create_datareader        | datareader created     | client_key: 0x00000001, datareader_id: 0x809(6), subscriber_id: 0x809(4)
[1764156474.586900] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x80A(2), participant_id: 0x001(1)
[1764156474.586915] info     | ProxyClient.cpp    | create_subscriber        | subscriber created     | client_key: 0x00000001, subscriber_id: 0x80A(4), participant_id: 0x001(1)
[1764156474.587064] info     | ProxyClient.cpp    | create_datareader        | datareader created     | client_key: 0x00000001, datareader_id: 0x80A(6), subscriber_id: 0x80A(4)
[1764156474.587127] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x80B(2), participant_id: 0x001(1)
[1764156474.587141] info     | ProxyClient.cpp    | create_subscriber        | subscriber created     | client_key: 0x00000001, subscriber_id: 0x80B(4), participant_id: 0x001(1)
[1764156474.587285] info     | ProxyClient.cpp    | create_datareader        | datareader created     | client_key: 0x00000001, datareader_id: 0x80B(6), subscriber_id: 0x80B(4)
[1764156474.587347] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x80C(2), participant_id: 0x001(1)
[1764156474.587357] info     | ProxyClient.cpp    | create_subscriber        | subscriber created     | client_key: 0x00000001, subscriber_id: 0x80C(4), participant_id: 0x001(1)
[1764156474.587532] info     | ProxyClient.cpp    | create_datareader        | datareader created     | client_key: 0x00000001, datareader_id: 0x80C(6), subscriber_id: 0x80C(4)
[1764156474.587619] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x80D(2), participant_id: 0x001(1)
[1764156474.587631] info     | ProxyClient.cpp    | create_subscriber        | subscriber created     | client_key: 0x00000001, subscriber_id: 0x80D(4), participant_id: 0x001(1)
[1764156474.587774] info     | ProxyClient.cpp    | create_datareader        | datareader created     | client_key: 0x00000001, datareader_id: 0x80D(6), subscriber_id: 0x80D(4)
[1764156474.587840] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x80E(2), participant_id: 0x001(1)
[1764156474.587849] info     | ProxyClient.cpp    | create_subscriber        | subscriber created     | client_key: 0x00000001, subscriber_id: 0x80E(4), participant_id: 0x001(1)
[1764156474.587992] info     | ProxyClient.cpp    | create_datareader        | datareader created     | client_key: 0x00000001, datareader_id: 0x80E(6), subscriber_id: 0x80E(4)
[1764156474.588074] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x80F(2), participant_id: 0x001(1)
[1764156474.588087] info     | ProxyClient.cpp    | create_subscriber        | subscriber created     | client_key: 0x00000001, subscriber_id: 0x80F(4), participant_id: 0x001(1)
[1764156474.588264] info     | ProxyClient.cpp    | create_datareader        | datareader created     | client_key: 0x00000001, datareader_id: 0x80F(6), subscriber_id: 0x80F(4)
[1764156474.588447] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x810(2), participant_id: 0x001(1)
[1764156474.588488] info     | ProxyClient.cpp    | create_subscriber        | subscriber created     | client_key: 0x00000001, subscriber_id: 0x810(4), participant_id: 0x001(1)
[1764156474.588703] info     | ProxyClient.cpp    | create_datareader        | datareader created     | client_key: 0x00000001, datareader_id: 0x810(6), subscriber_id: 0x810(4)
[1764156474.588792] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x811(2), participant_id: 0x001(1)
[1764156474.588805] info     | ProxyClient.cpp    | create_subscriber        | subscriber created     | client_key: 0x00000001, subscriber_id: 0x811(4), participant_id: 0x001(1)
[1764156474.588969] info     | ProxyClient.cpp    | create_datareader        | datareader created     | client_key: 0x00000001, datareader_id: 0x811(6), subscriber_id: 0x811(4)
[1764156474.589044] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x812(2), participant_id: 0x001(1)
[1764156474.589059] info     | ProxyClient.cpp    | create_subscriber        | subscriber created     | client_key: 0x00000001, subscriber_id: 0x812(4), participant_id: 0x001(1)
[1764156474.589238] info     | ProxyClient.cpp    | create_datareader        | datareader created     | client_key: 0x00000001, datareader_id: 0x812(6), subscriber_id: 0x812(4)
[1764156474.589388] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x813(2), participant_id: 0x001(1)
[1764156474.589407] info     | ProxyClient.cpp    | create_subscriber        | subscriber created     | client_key: 0x00000001, subscriber_id: 0x813(4), participant_id: 0x001(1)
[1764156474.589676] info     | ProxyClient.cpp    | create_datareader        | datareader created     | client_key: 0x00000001, datareader_id: 0x813(6), subscriber_id: 0x813(4)
[1764156474.589839] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x814(2), participant_id: 0x001(1)
[1764156474.589860] info     | ProxyClient.cpp    | create_subscriber        | subscriber created     | client_key: 0x00000001, subscriber_id: 0x814(4), participant_id: 0x001(1)
[1764156474.590070] info     | ProxyClient.cpp    | create_datareader        | datareader created     | client_key: 0x00000001, datareader_id: 0x814(6), subscriber_id: 0x814(4)
[1764156474.590183] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x815(2), participant_id: 0x001(1)
[1764156474.590198] info     | ProxyClient.cpp    | create_subscriber        | subscriber created     | client_key: 0x00000001, subscriber_id: 0x815(4), participant_id: 0x001(1)
[1764156474.590364] info     | ProxyClient.cpp    | create_datareader        | datareader created     | client_key: 0x00000001, datareader_id: 0x815(6), subscriber_id: 0x815(4)
[1764156474.590438] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x816(2), participant_id: 0x001(1)
[1764156474.590454] info     | ProxyClient.cpp    | create_subscriber        | subscriber created     | client_key: 0x00000001, subscriber_id: 0x816(4), participant_id: 0x001(1)
[1764156474.590610] info     | ProxyClient.cpp    | create_datareader        | datareader created     | client_key: 0x00000001, datareader_id: 0x816(6), subscriber_id: 0x816(4)
[1764156474.590677] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x817(2), participant_id: 0x001(1)
[1764156474.590693] info     | ProxyClient.cpp    | create_subscriber        | subscriber created     | client_key: 0x00000001, subscriber_id: 0x817(4), participant_id: 0x001(1)
[1764156474.590845] info     | ProxyClient.cpp    | create_datareader        | datareader created     | client_key: 0x00000001, datareader_id: 0x817(6), subscriber_id: 0x817(4)
[1764156474.590910] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x818(2), participant_id: 0x001(1)
[1764156474.590924] info     | ProxyClient.cpp    | create_subscriber        | subscriber created     | client_key: 0x00000001, subscriber_id: 0x818(4), participant_id: 0x001(1)
[1764156474.591081] info     | ProxyClient.cpp    | create_datareader        | datareader created     | client_key: 0x00000001, datareader_id: 0x818(6), subscriber_id: 0x818(4)
[1764156474.591143] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x819(2), participant_id: 0x001(1)
[1764156474.591153] info     | ProxyClient.cpp    | create_subscriber        | subscriber created     | client_key: 0x00000001, subscriber_id: 0x819(4), participant_id: 0x001(1)
[1764156474.591306] info     | ProxyClient.cpp    | create_datareader        | datareader created     | client_key: 0x00000001, datareader_id: 0x819(6), subscriber_id: 0x819(4)
[1764156474.591372] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x81A(2), participant_id: 0x001(1)
[1764156474.591381] info     | ProxyClient.cpp    | create_subscriber        | subscriber created     | client_key: 0x00000001, subscriber_id: 0x81A(4), participant_id: 0x001(1)
[1764156474.591539] info     | ProxyClient.cpp    | create_datareader        | datareader created     | client_key: 0x00000001, datareader_id: 0x81A(6), subscriber_id: 0x81A(4)
[1764156474.591604] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x81B(2), participant_id: 0x001(1)
[1764156474.591614] info     | ProxyClient.cpp    | create_subscriber        | subscriber created     | client_key: 0x00000001, subscriber_id: 0x81B(4), participant_id: 0x001(1)
[1764156474.591764] info     | ProxyClient.cpp    | create_datareader        | datareader created     | client_key: 0x00000001, datareader_id: 0x81B(6), subscriber_id: 0x81B(4)
[1764156474.591829] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x81C(2), participant_id: 0x001(1)
[1764156474.591842] info     | ProxyClient.cpp    | create_subscriber        | subscriber created     | client_key: 0x00000001, subscriber_id: 0x81C(4), participant_id: 0x001(1)
[1764156474.591989] info     | ProxyClient.cpp    | create_datareader        | datareader created     | client_key: 0x00000001, datareader_id: 0x81C(6), subscriber_id: 0x81C(4)
[1764156474.592489] info     | ProxyClient.cpp    | create_replier           | replier created        | client_key: 0x00000001, requester_id: 0x800(7), participant_id: 0x001(1)
[1764156474.592617] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x013(2), participant_id: 0x001(1)
[1764156474.592640] info     | ProxyClient.cpp    | create_publisher         | publisher created      | client_key: 0x00000001, publisher_id: 0x013(3), participant_id: 0x001(1)
[1764156474.592738] info     | ProxyClient.cpp    | create_datawriter        | datawriter created     | client_key: 0x00000001, datawriter_id: 0x013(5), publisher_id: 0x013(3)
INFO  [uxrce_dds_client] successfully created rt/fmu/out/battery_status data writer, topic id: 19
[1764156474.592804] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x052(2), participant_id: 0x001(1)
[1764156474.592817] info     | ProxyClient.cpp    | create_publisher         | publisher created      | client_key: 0x00000001, publisher_id: 0x052(3), participant_id: 0x001(1)
[1764156474.592875] info     | ProxyClient.cpp    | create_datawriter        | datawriter created     | client_key: 0x00000001, datawriter_id: 0x052(5), publisher_id: 0x052(3)
INFO  [uxrce_dds_client] successfully created rt/fmu/out/estimator_status_flags data writer, topic id: 82
[1764156474.592924] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x058(2), participant_id: 0x001(1)
[1764156474.592932] info     | ProxyClient.cpp    | create_publisher         | publisher created      | client_key: 0x00000001, publisher_id: 0x058(3), participant_id: 0x001(1)
[1764156474.592992] info     | ProxyClient.cpp    | create_datawriter        | datawriter created     | client_key: 0x00000001, datawriter_id: 0x058(5), publisher_id: 0x058(3)
INFO  [uxrce_dds_client] successfully created rt/fmu/out/failsafe_flags data writer, topic id: 88
[1764156474.593039] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x089(2), participant_id: 0x001(1)
[1764156474.593047] info     | ProxyClient.cpp    | create_publisher         | publisher created      | client_key: 0x00000001, publisher_id: 0x089(3), participant_id: 0x001(1)
[1764156474.593110] info     | ProxyClient.cpp    | create_datawriter        | datawriter created     | client_key: 0x00000001, datawriter_id: 0x089(5), publisher_id: 0x089(3)
INFO  [uxrce_dds_client] successfully created rt/fmu/out/manual_control_setpoint data writer, topic id: 137
[1764156474.593153] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x0B5(2), participant_id: 0x001(1)
[1764156474.593160] info     | ProxyClient.cpp    | create_publisher         | publisher created      | client_key: 0x00000001, publisher_id: 0x0B5(3), participant_id: 0x001(1)
[1764156474.593220] info     | ProxyClient.cpp    | create_datawriter        | datawriter created     | client_key: 0x00000001, datawriter_id: 0x0B5(5), publisher_id: 0x0B5(3)
INFO  [uxrce_dds_client] successfully created rt/fmu/out/position_setpoint_triplet data writer, topic id: 181[1764156474.593270] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x0D5(2), participant_id: 0x001(1)
[1764156474.593278] info     | ProxyClient.cpp    | create_publisher         | publisher created      | client_key: 0x00000001, publisher_id: 0x0D5(3), participant_id: 0x001(1)
[1764156474.593345] info     | ProxyClient.cpp    | create_datawriter        | datawriter created     | client_key: 0x00000001, datawriter_id: 0x0D5(5), publisher_id: 0x0D5(3)
INFO  [uxrce_dds_client] successfully created rt/fmu/out/sensor_combined data writer, topic id: 213
[1764156474.593431] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x0EC(2), participant_id: 0x001(1)
[1764156474.593456] info     | ProxyClient.cpp    | create_publisher         | publisher created      | client_key: 0x00000001, publisher_id: 0x0EC(3), participant_id: 0x001(1)
[1764156474.593537] info     | ProxyClient.cpp    | create_datawriter        | datawriter created     | client_key: 0x00000001, datawriter_id: 0x0EC(5), publisher_id: 0x0EC(3)
INFO  [uxrce_dds_client] successfully created rt/fmu/out/timesync_status data writer, topic id: 236
[1764156474.593628] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x109(2), participant_id: 0x001(1)
[1764156474.593666] info     | ProxyClient.cpp    | create_publisher         | publisher created      | client_key: 0x00000001, publisher_id: 0x109(3), participant_id: 0x001(1)
[1764156474.593754] info     | ProxyClient.cpp    | create_datawriter        | datawriter created     | client_key: 0x00000001, datawriter_id: 0x109(5), publisher_id: 0x109(3)
INFO  [uxrce_dds_client] successfully created rt/fmu/out/vehicle_land_detected data writer, topic id: 265
[1764156474.593873] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x0FC(2), participant_id: 0x001(1)
[1764156474.593884] info     | ProxyClient.cpp    | create_publisher         | publisher created      | client_key: 0x00000001, publisher_id: 0x0FC(3), participant_id: 0x001(1)
[1764156474.593953] info     | ProxyClient.cpp    | create_datawriter        | datawriter created     | client_key: 0x00000001, datawriter_id: 0x0FC(5), publisher_id: 0x0FC(3)
INFO  [uxrce_dds_client] successfully created rt/fmu/out/vehicle_attitude data writer, topic id: 252
[1764156474.593995] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x103(2), participant_id: 0x001(1)
[1764156474.594005] info     | ProxyClient.cpp    | create_publisher         | publisher created      | client_key: 0x00000001, publisher_id: 0x103(3), participant_id: 0x001(1)
[1764156474.594067] info     | ProxyClient.cpp    | create_datawriter        | datawriter created     | client_key: 0x00000001, datawriter_id: 0x103(5), publisher_id: 0x103(3)
INFO  [uxrce_dds_client] successfully created rt/fmu/out/vehicle_control_mode data writer, topic id: 259
[1764156474.594115] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x100(2), participant_id: 0x001(1)
[1764156474.594134] info     | ProxyClient.cpp    | create_publisher         | publisher created      | client_key: 0x00000001, publisher_id: 0x100(3), participant_id: 0x001(1)
[1764156474.594271] info     | ProxyClient.cpp    | create_datawriter        | datawriter created     | client_key: 0x00000001, datawriter_id: 0x100(5), publisher_id: 0x100(3)
INFO  [uxrce_dds_client] successfully created rt/fmu/out/vehicle_command_ack data writer, topic id: 256
[1764156474.594377] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x104(2), participant_id: 0x001(1)
[1764156474.594389] info     | ProxyClient.cpp    | create_publisher         | publisher created      | client_key: 0x00000001, publisher_id: 0x104(3), participant_id: 0x001(1)
[1764156474.594459] info     | ProxyClient.cpp    | create_datawriter        | datawriter created     | client_key: 0x00000001, datawriter_id: 0x104(5), publisher_id: 0x104(3)
INFO  [uxrce_dds_client] successfully created rt/fmu/out/vehicle_global_position data writer, topic id: 260
[1764156474.594513] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x106(2), participant_id: 0x001(1)
[1764156474.594526] info     | ProxyClient.cpp    | create_publisher         | publisher created      | client_key: 0x00000001, publisher_id: 0x106(3), participant_id: 0x001(1)
[1764156474.594598] info     | ProxyClient.cpp    | create_datawriter        | datawriter created     | client_key: 0x00000001, datawriter_id: 0x106(5), publisher_id: 0x106(3)
INFO  [uxrce_dds_client] successfully created rt/fmu/out/vehicle_gps_position data writer, topic id: 262
[1764156474.594642] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x10A(2), participant_id: 0x001(1)
[1764156474.594651] info     | ProxyClient.cpp    | create_publisher         | publisher created      | client_key: 0x00000001, publisher_id: 0x10A(3), participant_id: 0x001(1)
[1764156474.594710] info     | ProxyClient.cpp    | create_datawriter        | datawriter created     | client_key: 0x00000001, datawriter_id: 0x10A(5), publisher_id: 0x10A(3)
INFO  [uxrce_dds_client] successfully created rt/fmu/out/vehicle_local_position data writer, topic id: 266
[1764156474.594753] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x10F(2), participant_id: 0x001(1)
[1764156474.594761] info     | ProxyClient.cpp    | create_publisher         | publisher created      | client_key: 0x00000001, publisher_id: 0x10F(3), participant_id: 0x001(1)
[1764156474.594823] info     | ProxyClient.cpp    | create_datawriter        | datawriter created     | client_key: 0x00000001, datawriter_id: 0x10F(5), publisher_id: 0x10F(3)
INFO  [uxrce_dds_client] successfully created rt/fmu/out/vehicle_odometry data writer, topic id: 271
[1764156474.594861] info     | ProxyClient.cpp    | create_topic             | topic created          | client_key: 0x00000001, topic_id: 0x114(2), participant_id: 0x001(1)
[1764156474.594869] info     | ProxyClient.cpp    | create_publisher         | publisher created      | client_key: 0x00000001, publisher_id: 0x114(3), participant_id: 0x001(1)
[1764156474.594931] info     | ProxyClient.cpp    | create_datawriter        | datawriter created     | client_key: 0x00000001, datawriter_id: 0x114(5), publisher_id: 0x114(3)
INFO  [uxrce_dds_client] successfully created rt/fmu/out/vehicle_status data writer, topic id: 276
INFO  [uxrce_dds_client] time sync converged
WARN  [timesync] time jump detected. Resetting time synchroniser.
WARN  [uxrce_dds_client] time sync no longer converged
INFO  [uxrce_dds_client] time sync converged


ava@ava:~/kit-extension-template-cpp/source/extensions/uosm.isaac.px4_bridge$ ros2 topic hz /fmu/out/sensor_combined --window 100
average rate: 39.217
        min: 0.000s max: 0.079s std dev: 0.02164s window: 40
average rate: 38.184
        min: 0.000s max: 0.091s std dev: 0.02338s window: 78
average rate: 37.494
        min: 0.000s max: 0.091s std dev: 0.02378s window: 100

INFO  [uxrce_dds_client] successfully created rt/fmu/out/vehicle_status data writer, topic id: 276
INFO  [uxrce_dds_client] time sync converged
WARN  [timesync] time jump detected. Resetting time synchroniser.
WARN  [uxrce_dds_client] time sync no longer converged
INFO  [uxrce_dds_client] time sync converged
INFO  [commander] Armed by external command
INFO  [tone_alarm] arming warning
INFO  [commander] Takeoff detected
WARN  [timesync] time jump detected. Resetting time synchroniser.
WARN  [uxrce_dds_client] time sync no longer converged
INFO  [uxrce_dds_client] time sync converged
WARN  [health_and_arming_checks] Preflight Fail: Attitude failure (roll)
WARN  [failsafe] Failsafe activated
WARN  [failsafe] Failsafe activated
WARN  [failsafe] Failsafe activated
INFO  [tone_alarm] battery warning (fast)
WARN  [timesync] time jump detected. Resetting time synchroniser.
WARN  [uxrce_dds_client] time sync no longer converged
WARN  [failsafe] Failsafe activated
INFO  [uxrce_dds_client] time sync converged
WARN  [failsafe] Failsafe activated
WARN  [failsafe] Failsafe activated
INFO  [commander] Disarmed by external command
INFO  [tone_alarm] notify neutral
INFO  [vehicle_imu] GYRO 0 (1310988) offset committed: [0.000 0.000 0.000]->[0.007 0.007 -0.007])
INFO  [logger] closed logfile, bytes written: 7840704
WARN  [health_and_arming_checks] Preflight Fail: vertical velocity unstable
WARN  [health_and_arming_checks] Preflight Fail: Attitude failure (roll)
WARN  [health_and_arming_checks] Preflight Fail: vertical velocity unstable
WARN  [health_and_arming_checks] Preflight Fail: Attitude failure (roll)
WARN  [health_and_arming_checks] Preflight Fail: vertical velocity unstable
WARN  [health_and_arming_checks] Preflight Fail: Attitude failure (roll)
WARN  [health_and_arming_checks] Preflight Fail: vertical velocity unstable
WARN  [health_and_arming_checks] Preflight Fail: Attitude failure (roll)
WARN  [timesync] time jump detected. Resetting time synchroniser.
WARN  [uxrce_dds_client] time sync no longer converged
WARN  [health_and_arming_checks] Preflight Fail: vertical velocity unstable
WARN  [health_and_arming_checks] Preflight Fail: Attitude failure (roll)
INFO  [uxrce_dds_client] time sync converged
WARN  [health_and_arming_checks] Preflight Fail: Attitude failure (roll)
WARN  [health_and_arming_checks] Preflight Fail: vertical velocity unstable
WARN  [health_and_arming_checks] Preflight Fail: Attitude failure (roll)
```

