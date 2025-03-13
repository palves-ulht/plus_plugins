A fork of sensor_plus, resetted to version 2.0.2, with a change in the sampling rate of the accelerometer (for Android):

StreamHandlerImpl:

    sensorManager.registerListener(sensorEventListener, sensor, 50 * 1000)

instead of

    sensorManager.registerListener(sensorEventListener, sensor, SensorManager.SENSOR_DELAY_NORMAL)
