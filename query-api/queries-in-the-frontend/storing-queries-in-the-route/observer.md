# Observer

<figure><img src="../../../.gitbook/assets/route_observer.drawio.png" alt=""><figcaption><p>Route parameters observer</p></figcaption></figure>

## Flow

On build:

* Add listener to route. When the parameters change:
  * Send parameters to parse
  * Set parse result into subject
