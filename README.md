# Hackintosh Ventura - Surface Laptop Go
![D09E3D7F-F58E-4740-A655-EA892D806229_1_201_a](https://user-images.githubusercontent.com/81677769/232604708-fa58a97c-e912-446c-8cca-060ff9e421c8.jpeg)

	Surface Laptop Go Hardware
	
	Specs:
		CPU: Intel i5-1035G1 (Icelake)
		GPU: Intel UHD Graphics (Iris Plus Graphics G1)
		RAM: 8GB Soldered to motherboard
		Wifi: Intel Killer Wifi 6 AX1650i (201NGW)
		Audio: Intel Ice Lake-LP Smart Sound Technology (Realtek ALC274 codec)
		Touchpad: ELAN
		SSD: 128GB NVME M.2

	Working:
		WiFi
		Suspend/Sleep (standby works, hibernate will not)
		Touchpad
		Graphics Accel.
		Sound
		Touchscreen
		Screen brightness
		Power Management
		Bluetooth 4.X and lower devices
		
	Not Working:
		Bluetooth 5.X devices
		AirDrop
 		Secure Boot

	Working On:
		Hibernate
			--> possible problems: $ pmset -g log
			2023-04-22 23:53:12 +0200 Notification        	Display is turned off 
			2023-04-22 23:53:12 +0200 Assertions          	PID 149(WindowServer) Summary UserIsActive "com.apple.iohideventsystem.queue.tickle serviceID:100000446 service:AppleUserHIDEventService product:ELAN Touchpad and Keyboard eventType:3" 00:00:14  id:0x0x900008085 [System: DeclUser kDisp]
			2023-04-22 23:53:12 +0200 Assertions          	PID 149(WindowServer) TurnedOn UserIsActive "com.apple.iohideventsystem.queue.tickle serviceID:10000044f service:AppleMultitouchDevice product:Magic Trackpad 2 eventType:11" 00:00:00  id:0x0x900008085 [System: DeclUser kDisp]          
			2023-04-22 23:53:12 +0200 Assertions          	Kernel Idle sleep preventers: -None-          
			2023-04-22 23:53:12 +0200 Assertions          	PID 0(kernel_task) Released Idle Sleep Preventer "IODisplayWrangler"  id:0x0x0 [System: DeclUser kDisp]          
			2023-04-22 23:53:12 +0200 Assertions          	PID 95(powerd) Created InternalPreventSleep "com.apple.powermanagement.darkwakelinger" 00:00:00  id:0x0xd00008266 [System: DeclUser SRPrevSleep kCPU kDisp]          
			2023-04-22 23:53:27 +0200 Assertions          	PID 95(powerd) TimedOut InternalPreventSleep "com.apple.powermanagement.darkwakelinger" 00:00:14  id:0x0xd00008266 [System: DeclUser SRPrevSleep kCPU kDisp]          
			2023-04-22 23:53:27 +0200 Assertions          	Summary- [System: DeclUser kDisp] Using Batt(Charge: 84)          
			2023-04-22 23:55:12 +0200 Assertions          	PID 149(WindowServer) TimedOut UserIsActive "com.apple.iohideventsystem.queue.tickle serviceID:10000044f service:AppleMultitouchDevice product:Magic Trackpad 2 eventType:11" 00:01:59  id:0x0x900008085 [System: DeclUser kDisp]          
			2023-04-22 23:55:12 +0200 Assertions          	Summary- [System: No Assertions] Using Batt(Charge: 83)          
			2023-04-22 23:59:41 +0200 Assertions          	PID 149(WindowServer) Created UserIsActive "com.apple.iohideventsystem.queue.tickle serviceID:100000280 service:AppleACPILid product:(null) eventType:3" 00:00:00  id:0x0x9000082fc [System: DeclUser kDisp]          

