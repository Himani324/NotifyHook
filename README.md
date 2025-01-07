# NotifyHook
Custom Notify hook to show notifications when a user submits any form.

It is a common scenario in React applications to show notifications to the user when a certain action is successfully completed or when there is any error while processing the user’s request.

# Shape of Notify state
{
  isActive: true,
  message: 'success message',
  isError: false
}

# Application flow
![image](https://github.com/user-attachments/assets/6dea9b92-d6af-41da-b88d-15df13e088c1)

When the user clicks the Save button on a form, send an API request to the back-end to save the details. Upon receiving a response, dispatch an action to update the Notify state. Depending upon this state, the Notify view will show a modal with a success or error message in it. The modal should disappear automatically after 3 seconds.

![image](https://github.com/user-attachments/assets/0570edd9-bd5e-4a9a-9545-349bd35efc18)

