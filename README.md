# 1090mhz-data
SFO ADS-B data captures

The CSV data is consolidated (a combination of several successive ADS-B messages for a given callsign) to give a full reference frame for the aircraft at a given (local, machine) time.  The header and an example row look like this:

```
machine-time,callsign,altitude,ground-speed,track,lat,lon,vertical-rate
1432328723,vrd0714,2950,263,53,37.68599,-122.27094,2496
```

The JSON data has more fields than the CSV, but is not consolidated (these are raw ADS-B messages augmented with corresponding ICAO data).  JSON entries look like this:

```
{
  "type": "msg",
  "subtype": "Air To Air Message",
  "subtype-note": "Triggered from TCAS.",
  "session-id": "111",
  "aircraft-id": "11111",
  "icao-hex-ident": "a695ef",
  "plane-n-number": "523VA",
  "plane-serial-number": "3181",
  "plane-mfr-mdl-code": "3940009",
  "plane-eng-mfr-mdl": "13011",
  "plane-year-mfr": "2007",
  "plane-type-registrant": "3",
  "plane-name": "WELLS FARGO BANK NORTHWEST NA TRUSTEE",
  "plane-street": "MAC U1228-51",
  "plane-street2": "299 S MAIN ST FL 5",
  "plane-city": "SALT LAKE CITY",
  "plane-state": "UT",
  "plane-zip-code": "841112689",
  "plane-region": "S",
  "plane-county": "035",
  "plane-country": "US",
  "plane-last-action-date": "20150129",
  "plane-cert-issue-date": "20070709",
  "plane-certification": "1T",
  "plane-type-aircraft": "5",
  "plane-type-engine": "5",
  "plane-status-code": "V",
  "plane-mode-s-code": "51512757",
  "plane-fract-owner": "",
  "plane-air-worth-date": "20070710",
  "plane-other-names(1)": "",
  "plane-other-names(2)": "",
  "plane-other-names(3)": "",
  "plane-other-names(4)": "",
  "plane-other-names(5)": "",
  "plane-expiration-date": "20171130",
  "plane-unique-id": "00374929",
  "plane-kit-mfr": "",
  "plane-kit-model": "",
  "plane-mode-s-code-hex": "A695EF",
  "plane-": "",
  "flight-id": "111111",
  "callsign": "",
  "altitude": "2900",
  "ground-speed": "",
  "track": "",
  "lat": "",
  "lon": "",
  "latlon": ",",
  "vertical-rate": "",
  "squawk": "",
  "alert-squawk-change": "",
  "emergency-squawk": "",
  "spi-ident": "",
  "is-on-ground": "0",
  "machine-time": 1432328722
}
```
