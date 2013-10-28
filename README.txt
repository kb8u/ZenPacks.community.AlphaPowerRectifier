This Zenpack is for monitoring Alpha Power Systems, Inc. AC-DC power
converters that are managed by CXC controllers.  It has been tested against
a CXPS 48-1T.  It may work with other models, but it has not been tested.

Device and component modelding is not done by this Zenpack, it merely has
some SNMP OIDs that it gathers data for:

AC mains voltage
Battery Capacity
Battery temperature
Battery Charge amps
Battery Charge volts
Load volts
Load amps
Number of major alarms
Number of minor alarms

There are graphs for the first seven, and events will be generated if there
are more than zero alarms.  Major alarms are at error level, minor alarms at
warn level.  An event class /HW/Power/Rectifier has been added for these.
Traps are not mapped nor is the MIB included.

There is also a device class /Power/Rectifiers/Alpha Technologies to contain
devices and which has a localy defined monitoring template for the above bound
to it.
