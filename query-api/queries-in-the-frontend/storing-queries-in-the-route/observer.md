# Observer

<figure><img src="../../../.gitbook/assets/observer_url_flow.drawio.png" alt=""><figcaption><p>Reacting to URL changes</p></figcaption></figure>

Reacts to these events:

* When the URL route changes

Does:

* Sends change event

This means that an initial request may be needed, to set the default values.

## Flow

<figure><img src="../../../.gitbook/assets/business_route_observer_changed_params.drawio.png" alt=""><figcaption><p>Parameter observer flow</p></figcaption></figure>

The observer subscribes to changes on the route parameters, and catches them to be parsed and stored. As the observer is observable any change on the stored data is notified to any listener.

## Model

<figure><img src="../../../.gitbook/assets/route_observer.drawio.png" alt=""><figcaption><p>Route parameters observer</p></figcaption></figure>
