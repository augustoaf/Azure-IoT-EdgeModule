all projects were created from template ".Net Core Console - C#", but running on .Net Framework 4.7.2.

Projects:

Counter/Calculation - EdgeModule which received a downstream device message, process the content and create a new message (with the data processed) to send to the IoT Hub. It also adds a property to the message.

Counter/Device1 - Simulated Downstream device wich connects to the Edge Device Gateway.
Counter/Device2 - Simulated Device using DPS to provision.

Note: Device1 and Device2 has the same code, the difference is how the variables are set inside, meaning how they will connect to the IoT Hub. Also the code has a handler for a direct method.

OperatorApp - app which reads messages from an Event Hub instance.

