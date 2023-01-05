# Actuator

![Updating URL parameters](../../../.gitbook/assets/actuator\_url\_flow.drawio.png)

Reacts to these events:

* User activates UI

Does:

* Updates route with parameters

The actuator is called by the user, through buttons or any other UI component, such as pagination navigation. The new parameter is added to the URL.

This change implies reloading the view.

## Model

<figure><img src="../../../.gitbook/assets/route_actuator.drawio.png" alt=""><figcaption><p>Route parameters actuator</p></figcaption></figure>

## Flow

When adding parameters:

* Get the current parameters
* Add the new ones
* Set the parameters

When setting the parameters:

* Remove the route parameters
* Navigate to the route with the new parameters
