# Reading 38

## Location

What are the benefits and downfalls of using the ‘getLastLocation()’ method to get your device’s location?

it's quick as it has already fetched this data before and it helps save battery, the downfalls here is that you're working with old/stale data that might not be representable if you need real time location. Sometimes you may get a null location if the location is turned off on the device.

What about the ‘getCurrentLocation()’ method?

- Fresh and Accurate - as close sd real time we can get.

- It does cost more batteries and time as the device will ping multiple times.

## Things I want to know more about

## References

[Location](https://developer.android.com/training/location/retrieve-current)
