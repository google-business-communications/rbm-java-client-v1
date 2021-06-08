# RCS BUSINESS MESSAGING: First agent

This sample demonstrates how to use the [RCS Business Messaging Java client library](https://github.com/google-business-communications/java-rcsbusinessmessaging) for performing operations
with the [RCS Business Messaging API](https://developers.google.com/business-communications/rcs-business-messaging/reference/rest)
to send and receive messages to an RCS-enabled device.

This application assumes that you're signed up with
[RCS Business Messaging](https://developers.google.com/business-communications/rcs-business-messaging/guides/get-started/register-partner).

## Documentation

The documentation for the RCS Business Messaging API can be found [here](https://developers.google.com/business-communications/rcs-business-messaging/reference/rest).

## Prerequisite

You must have the following software installed on your machine:

    * [Apache Maven](http://maven.apache.org) 3.3.9 or greater
    * [Java 8](http://www.oracle.com/technetwork/java/javase/downloads/index.html)

## Before you begin

1.  [Register with RCS Business Messaging](https://developers.google.com/business-communications/rcs-business-messaging/guides/get-started/register-partner).
1. Open the Business Communications Developer Console (https://business-communications.cloud.google.com/console/) with your registered
    Google account and create a new RBM agent.
1. When the agent is available, click the agent's card.
1. In the left navigation, click **Service account**.
1. Click **Create key**, then click **Create**. Your browser downloads a service account key for
    your agent. You need this key to make RBM API calls as your agent.
1. Rename the service account key "rbm-agent-service-account-credentials.json" and move it
    into the "rbm-java-client-v1/src/main/resources" directory.

## Execute the sample

### Setup your test device

1. In a terminal, navigate to this sample's root directory.

1. Run the following commands:

    mvn compile
    mvn exec:java -Dexec.args="TEST_DEVICE_PHONE_NUMBER invite"

    Where the TEST_DEVICE_PHONE_NUMBER is replaced by the phone number of your RCS-enabled device in E.164 format.
    
    For example, with the US phone number +1-222-333-4444, the value would be +12223334444.

### Run the sample

1. In a terminal, navigate to this sample's root directory.

1. Run the following commands:

    mvn compile
    mvn exec:java -Dexec.args="TEST_DEVICE_PHONE_NUMBER chat"

    Where the TEST_DEVICE_PHONE_NUMBER is replaced by the phone number of your RCS-enabled device in E.164 format.

    For example, with the US phone number +1-222-333-4444, the value would be +12223334444.

## Learn more

To learn more about setting up RCS Business Messaging see the
[documentation](https://developers.google.com/business-communications/rcs-business-messaging/guides/get-started/how-it-works).
