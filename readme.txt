How to build
-------------
run: mvn clean install

How to add the handler to the GW
--------------------------------
Once it is build, copy the
target/logging-handler-1.0.0.jar to GW_HOME/osgi/dropins/

restart the Gateway,
You will be able to see a log as follows
"A new handler named logging handler is added to the Handler Executor"


Once the request is send it will log the transport headers available in the message coming to camel engine and sending
out from camel engine

for more information on the invocation points please refer:
https://github.com/wso2/carbon-messaging/blob/master/components/src/main/java/org/wso2/carbon/messaging/handler/MessagingHandler.java

fixing issue1 incorrectly. Now fixing correctly :)
