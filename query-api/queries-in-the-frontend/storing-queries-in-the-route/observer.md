# Observer

![Reacting to URL changes](../../../.gitbook/assets/observer\_url\_flow.drawio.png)

Reacts to these events:

* When the URL route changes

Does:

* Sends change event

This means that an initial request may be needed, to set the default values.

## Model

<figure><img src="../../../.gitbook/assets/route_observer.drawio.png" alt=""><figcaption><p>Route parameters observer</p></figcaption></figure>

## Flow

On component build:

* Add listener to route. When the parameters change:
  * Send parameters to parse
  * Set parse result into subject
