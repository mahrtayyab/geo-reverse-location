# GEO REVERSE LOCATION
## Description 
This Free API can be used to reverse the Longitude and Latitude to a Location Name
## Authentication
```diff
**No Authentication Required for this API**
```
## Limits
```diff
**This API isn't limited in any term**
```
## Using API
### Required Parameters
* Latitude (lat)
* Longitude (long)

### API Endpoint

```
https://factory-apis.herokuapp.com/api/geo_reverse?lat=31.402696&long=73.0287094
```
* Replace number against "lat" with latitude of your queried location
* Replace number against "long" with longitude of your queried location

## Output
* Type -> json
* Structure 
```bash
{
    AdministrativeArea: {
        CountryID: "PK",
        EnglishName: "Punjab",
        EnglishType: "Province",
        ID: "PB",
        Level: 1,
        LocalizedName: "Punjab",
        LocalizedType: "Province"
    },
    Country: {
        EnglishName: "Pakistan",
        ID: "PK",
        LocalizedName: "Pakistan"
    },
    LocalizedName: "Faisalabad",
    geoLocation: {
        Elevation: {
            Imperial: {
                Unit: "ft",
                UnitType: 0,
                Value: 570
            },
            Metric: {
                Unit: "m",
                UnitType: 5,
                Value: 174
            }
        },
        Latitude: 31.409,
        Longitude: 73.083
    },
    region: {
        EnglishName: "Asia",
        ID: "ASI",
        LocalizedName: "Asia"
    },
    status: 200,
    timeZone: {
        Code: "PKT",
        GmtOffset: 5,
        IsDaylightSaving: false,
        Name: "Asia/Karachi",
        NextOffsetChange: null
    },
    type: "City"
} 
```

## Status
### Status 200
The Request was successful and the Location has been fetched
### Status 404
The Request was successful but the Location wasn't found for provided Latitude and Longitude
### Status 422
The Request wasn't successful because one or both parameters were not fulfilled  