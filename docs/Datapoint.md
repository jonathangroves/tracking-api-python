# Datapoint

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**location** | [**GeoPoint**](GeoPoint.md) |  | [optional] 
**timestamp** | **datetime** | Timestamp for the datapoint. NB this is not necessarily the same as &#39;created&#39; | 
**speed** | **float** | Ground velocity in kmh, as determined by the GPS | [optional] 
**altitude** | **float** | Altitude in m, as determined by the GPS | [optional] 
**course** | **float** | Course in degrees, as determined by the GPS | [optional] 
**num_value** | **str** | Internal use only | [optional] 
**string_value** | **str** | Internal use only | [optional] 
**send_reason** | **float** | Bitfield indicating reason for datapoint transmission and status of the device at the time.   Bit1(1): Wake mode active,    Bit2(2): Sleep mode active,    Bit3(4): Bluetooth disconnected,    Bit4(8): Outside of Safe-zone,    Bit5(16): Motion detected,    Bit6(32): Device started moving,    Bit7(64): Device stopped moving,    Bit8(128): Position is stale: last known location was used   Special case 255/0xFF: device was checking in with server. Ignore all data | [optional] 
**sats** | **float** | Number of visible satellites, as determined by the GPS | [optional] 
**hdop** | **float** | Deprecated | [optional] 
**accuracy** | **float** | Accuracy of the location in meters | [optional] 
**location_type** | **str** | Type of position. Can be &#39;gps&#39;, &#39;wifi&#39;, &#39;gsm&#39; or &#39;invalid&#39; | [default to 'gps']
**battery_voltage** | **float** | Battery charge level in volts. | [optional] 
**average_charge** | **float** | Internal Use. 255 indicates plugged in and charging. | [optional] 
**created** | **datetime** | Timestamp for when the datapoint was received and processed by the server | 
**address** | **str** | A reverse geocode result for the point | [optional] 
**alert_type** | **float** | Bitfield indicating what alerts where active at transmission time   Bit1(1): Freefall / Drop detected,    Bit2(2): Rotation detected,    Bit3(4): GSM jamming detected,    Bit4(8): Button was pressed,    Bit5(16): Generic Alert    Bit6(32): Ignition input high| [optional] 
**current_used** | **float** | Current Used to send this location in microAmp Hours | [optional] 
**gsm_signal** | **float** | GSM CSQ value | [optional] 
**correlation_id** | **str** | Internal use - correlation identifier | [optional] 
**id** | **float** |  | [optional] 
**device_id** | **float** |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


