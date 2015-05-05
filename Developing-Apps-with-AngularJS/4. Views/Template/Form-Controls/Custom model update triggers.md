* By default, any change to the content will trigger a model update and form validation
* We can override this behavior using the ngModelOptions directive to bind only to specified list of events. E.g. ng-model-options="{ updateOn: 'blur' }"
* We can set several events using a space delimited list. E.g. ng-model-options="{ updateOn: 'mousedown blur' }"
* We can use the default behaviour by using default as one of the events in the list
