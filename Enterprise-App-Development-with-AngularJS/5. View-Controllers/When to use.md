* Use controllers to:
  - Set up the initial state of the $scope object
  - Add behavior to the $scope object
  - watch other parts of the model for changes and take action
  
  
* Do not use controllers to:
  - Manipulate DOM - use data binding and directives
  - Format input - use form controls
  - Filter output - use filter
  - Share code or state across controllers  - use services
  - Manage the life-cycle of other components (for example, to create service instances)
