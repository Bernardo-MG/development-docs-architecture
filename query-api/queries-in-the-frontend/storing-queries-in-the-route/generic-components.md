# Generic Components

We are keeping two separate flows. One for writing the arguments, another for reading them.

![Using the URL to store parameters](../../../.gitbook/assets/datasource\_url\_flow.drawio.png)

## Writing Parameters

![Updating a URL with pagination parameters](<../../../.gitbook/assets/actuator\_url\_flow.drawio (2).png>)

The user can change parameters through the controllers. These are mapped to components, such as a pagination navigation, which will do the actual call to the controller. Afterwards the new parameter is sent to the URL actuator, which will add or update any required parameter to the URL.

This change implies reloading the view.

## Reading Parameters

![Making a request with URL parameters](<../../../.gitbook/assets/datasource\_endpoint\_flow.drawio (1).png>)

When the view is loaded the datasource reads any parameter it requires from the URL. Then makes the initial data request from it, updating the view. Any additional request will keep those parameters

The only way to change the query parameters is by updating the URL.

