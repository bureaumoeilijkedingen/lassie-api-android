# Lassie Android API
An Android library to connect with the Lassie API.

## Getting started
To use this library, add the LassieAPI.java file to your Android project. LassieAPI makes use of some references in the api_settings.xml file, these should be implemented somewhere in your resources.

### Initiate the LassieAPI
```
RequestQueue queue = Volley.newRequestQueue(this);
LassieAPI lassieApi = new LassieAPI(this, queue);
```

## Implementation of callbacks
```
lassieApi.getPersonalInfo(new LassieAPI.LassieObjectCallback() {
  @Override
  public void result(JSONObject result) {
    Log.d(TAG, result);
  }
});
```
