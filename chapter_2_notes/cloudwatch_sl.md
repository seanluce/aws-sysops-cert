* Compute
	* EC2 
		* CPU
		* Network
		* Disk
		* Status Checks
			* System (checks host)
				* Loss of network connectivity
				* Loss of system power
				* Software issues on physical host
				* Hardware issues on the physical host
				* Stop the VM and start it again will cause it to restart on a new host
			* Instance (checks VM)
				* Exhausted memory
				* Corrupted file system
				* Reboot or fix at OS level
		* RAM Utilization is a custom metric!
		* By default 5 minute intervals, 1 minute detailed monitoring can be enabled
	
* Storage


* Metrics stored for 2 weeks.  Granularity varies based on service.

* Alarms
	* Alarms can be created, triggered on some thresholds.
