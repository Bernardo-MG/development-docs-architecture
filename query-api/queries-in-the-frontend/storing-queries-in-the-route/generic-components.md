# Generic Components

We are keeping two separate flows. One for writing the arguments, another for reading them.

![Using the URL to store parameters](<../../../.gitbook/assets/datasource\_url\_flow.drawio (1).png>)

## Writing Parameters

![Updating URL parameters](../../../.gitbook/assets/actuator\_url\_flow.drawio.png)

Reacts to these events:

* User activates UI

Does:

* Updates route with parameters

The actuator is called by the user, through buttons or any other UI component, such as pagination navigation. The new parameter is added to the URL.

This change implies reloading the view.

## Reading Parameters

![Reacting to URL changes](../../../.gitbook/assets/observer\_url\_flow.drawio.png)

Reacts to these events:

* When the URL route changes

Does:

* Throws change event

This means that an initial request may be needed, to set the default values.
