Ember Tutorial Services and Utilities
https://guides.emberjs.com/v3.0.0/tutorial/service/

Making Google Maps available
- ember install ember-simple-google-maps

generate google api keY

- GOOGLE_MAPS_API_KEY=<your key here> ember s
https://console.developers.google.com/apis/credentials

Accessing the Google API with a Utility

- ember g util google-maps

Fetching Maps with a Service

- ember g service maps

Display maps with a component

- ember g component location-map

Unit testing a Service

instantiate the service with factoryFor

Integration Testing with Map component

Stubbing Services in Application Tests
