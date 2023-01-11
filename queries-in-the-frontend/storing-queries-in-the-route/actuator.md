# Actuator

![Updating URL parameters](../../.gitbook/assets/actuator\_url\_flow.drawio.png)

Reacts to these events:

* User activates UI

Does:

* Updates route with parameters

The actuator is called by the user, through buttons or any other UI component, such as pagination navigation. The new parameter is added to the URL.

This change implies reloading the view.

## Flow

### Setting parameters

<figure><img src="../../.gitbook/assets/business_route_actuator_set_params.drawio.png" alt=""><figcaption></figcaption></figure>

### Adding parameters

<figure><img src="../../.gitbook/assets/business_route_actuator_add_params.drawio.png" alt=""><figcaption></figcaption></figure>

## Model

<figure><img src="../../.gitbook/assets/route_actuator.drawio.png" alt=""><figcaption><p>Route parameters actuator</p></figcaption></figure>
