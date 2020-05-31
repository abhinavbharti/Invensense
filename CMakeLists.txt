
set(COMP_SRCS   Invn/Devices/DeviceIcm20649.c
                Invn/Devices/DeviceIcm20948.c
                Invn/Devices/HostSerif.c
                Invn/Devices/Sensor.c
                Invn/Devices/VSensorId.c
                Invn/Devices/Drivers/Icm20649/Icm20649DataBaseControl.c
                Invn/Devices/Drivers/Icm20649/Icm20649DataBaseDriver.c
                Invn/Devices/Drivers/Icm20649/Icm20649DataConverter.c
                Invn/Devices/Drivers/Icm20649/Icm20649Dmp3Driver.c
                Invn/Devices/Drivers/Icm20649/Icm20649LoadFirmware.c
                Invn/Devices/Drivers/Icm20649/Icm20649MPUFifoControl.c
                Invn/Devices/Drivers/Icm20649/Icm20649SelfTest.c
                Invn/Devices/Drivers/Icm20649/Icm20649Setup.c
                Invn/Devices/Drivers/Icm20649/Icm20649Transport.c
                Invn/Devices/Drivers/Icm20948/Icm20948Augmented.c
                Invn/Devices/Drivers/Icm20948/Icm20948AuxCompassAkm.c
                Invn/Devices/Drivers/Icm20948/Icm20948AuxTransport.c
                Invn/Devices/Drivers/Icm20948/Icm20948DataBaseControl.c
                Invn/Devices/Drivers/Icm20948/Icm20948DataBaseDriver.c
                Invn/Devices/Drivers/Icm20948/Icm20948DataConverter.c
                Invn/Devices/Drivers/Icm20948/Icm20948Dmp3Driver.c
                Invn/Devices/Drivers/Icm20948/Icm20948LoadFirmware.c
                Invn/Devices/Drivers/Icm20948/Icm20948MPUFifoControl.c
                Invn/Devices/Drivers/Icm20948/Icm20948SelfTest.c
                Invn/Devices/Drivers/Icm20948/Icm20948Setup.c
                Invn/Devices/Drivers/Icm20948/Icm20948Transport.c
                Invn/DynamicProtocol/DynProtocol.c
                Invn/DynamicProtocol/DynProtocolTransportUart.c
                Invn/EmbUtils/DataConverter.c
                Invn/EmbUtils/ErrorHelper.c
                Invn/EmbUtils/InvBasicMath.c
                Invn/EmbUtils/InvCksum.c
                Invn/EmbUtils/InvFormat.c
                Invn/EmbUtils/InvList.c
                Invn/EmbUtils/InvPrintf.c
                Invn/EmbUtils/InvProtocol.c
                Invn/EmbUtils/InvQueue.c
                Invn/EmbUtils/InvScheduler.c
                Invn/EmbUtils/Logger.c
                Invn/EmbUtils/Message.c
                Invn/EmbUtils/RingByteBuffer.c
                Invn/EmbUtils/UartTxEmulator.c
                Invn/VSensor/VSensor.c)
#add_definitions(-DSPIBUS_COMPONENT_TRUE=1)


idf_component_register(SRCS ${COMP_SRCS}
                       INCLUDE_DIRS "."
                       REQUIRES driver)
