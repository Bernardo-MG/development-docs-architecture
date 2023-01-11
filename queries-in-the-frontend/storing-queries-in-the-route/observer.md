# Observer

![Reacting to URL changes](../../.gitbook/assets/observer\_url\_flow.drawio.png)

Reacts to these events:

* When the URL route changes

Does:

* Sends change event

This means that an initial request may be needed, to set the default values.

## Flow

<figure><img src="../../.gitbook/assets/business_route_observer_changed_params.drawio.png" alt=""><figcaption><p>Parameter observer flow</p></figcaption></figure>

## Model

<figure><img src="../../.gitbook/assets/route_observer.drawio.png" alt=""><figcaption><p>Route parameters observer</p></figcaption></figure>
