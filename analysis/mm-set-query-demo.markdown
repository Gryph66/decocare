## query or set suspend/resume status
hi ` Namespace(commands=['query', 'suspend', 'query', 'resume', 'query', 'suspend', 'query', 'resume', 'query'], dryrun=False, init=False, port='/dev/ttyUSB.Carelink0', serial='208850', verbose=None) `
```
```
```
```
```
```
```
```
```javascript
{'radio': {'errors.crc': 0,
           'errors.naks': 0,
           'errors.sequence': 0,
           'errors.timeouts': 18,
           'packets.received': 183L,
           'packets.transmit': 203L},
 'usb': {'errors.crc': 0,
         'errors.naks': 0,
         'errors.sequence': 0,
         'errors.timeouts': 0,
         'packets.received': 3096L,
         'packets.transmit': 3096L}}
```
```
```
### PUMP MODEL: `ReadPumpModel:size[64]:data:'515'`
###  query
response: ReadPumpStatus:size[64]:data:{'status': 'normal', 'bolusing': False, 'suspended': False}
hexdump:
```
0000   0x03 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0008   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0010   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0018   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0020   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0028   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0030   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0038   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
```
##### decoded:
```python
{'status': 'normal', 'bolusing': False, 'suspended': False} 
```
###  suspend
ERROR:decocare.stick:size is less than 64, which will cause an error. trying 64 instead
WARNING:decocare.stick:bad zero CRC?
ERROR:decocare.stick:size is less than 64, which will cause an error. trying 64 instead
WARNING:decocare.stick:bad zero CRC?
CRITICAL:decocare.session:this seems like a problem
response: PumpSuspend:size[64]:data:bytearray(b'\x00')
hexdump:
```
0000   0x00                                       .
```
##### decoded:
```python
bytearray(b'\x00') 
```
###  query
response: ReadPumpStatus:size[64]:data:{'status': 'normal', 'bolusing': False, 'suspended': True}
hexdump:
```
0000   0x03 0x00 0x01 0x00 0x00 0x00 0x00 0x00    ........
0008   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0010   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0018   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0020   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0028   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0030   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0038   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
```
##### decoded:
```python
{'status': 'normal', 'bolusing': False, 'suspended': True} 
```
###  resume
ERROR:decocare.stick:size is less than 64, which will cause an error. trying 64 instead
WARNING:decocare.stick:bad zero CRC?
ERROR:decocare.stick:size is less than 64, which will cause an error. trying 64 instead
WARNING:decocare.stick:bad zero CRC?
CRITICAL:decocare.session:this seems like a problem
response: PumpResume:size[64]:data:bytearray(b'\x00')
hexdump:
```
0000   0x00                                       .
```
##### decoded:
```python
bytearray(b'\x00') 
```
###  query
response: ReadPumpStatus:size[64]:data:{'status': 'normal', 'bolusing': False, 'suspended': False}
hexdump:
```
0000   0x03 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0008   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0010   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0018   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0020   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0028   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0030   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0038   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
```
##### decoded:
```python
{'status': 'normal', 'bolusing': False, 'suspended': False} 
```
###  suspend
ERROR:decocare.stick:size is less than 64, which will cause an error. trying 64 instead
WARNING:decocare.stick:bad zero CRC?
ERROR:decocare.stick:size is less than 64, which will cause an error. trying 64 instead
WARNING:decocare.stick:bad zero CRC?
CRITICAL:decocare.session:this seems like a problem
response: PumpSuspend:size[64]:data:bytearray(b'\x00')
hexdump:
```
0000   0x00                                       .
```
##### decoded:
```python
bytearray(b'\x00') 
```
###  query
response: ReadPumpStatus:size[64]:data:{'status': 'normal', 'bolusing': False, 'suspended': True}
hexdump:
```
0000   0x03 0x00 0x01 0x00 0x00 0x00 0x00 0x00    ........
0008   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0010   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0018   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0020   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0028   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0030   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0038   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
```
##### decoded:
```python
{'status': 'normal', 'bolusing': False, 'suspended': True} 
```
###  resume
ERROR:decocare.stick:size is less than 64, which will cause an error. trying 64 instead
WARNING:decocare.stick:bad zero CRC?
ERROR:decocare.stick:size is less than 64, which will cause an error. trying 64 instead
WARNING:decocare.stick:bad zero CRC?
CRITICAL:decocare.session:this seems like a problem
response: PumpResume:size[64]:data:bytearray(b'\x00')
hexdump:
```
0000   0x00                                       .
```
##### decoded:
```python
bytearray(b'\x00') 
```
###  query
response: ReadPumpStatus:size[64]:data:{'status': 'normal', 'bolusing': False, 'suspended': False}
hexdump:
```
0000   0x03 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0008   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0010   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0018   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0020   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0028   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0030   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
0038   0x00 0x00 0x00 0x00 0x00 0x00 0x00 0x00    ........
```
##### decoded:
```python
{'status': 'normal', 'bolusing': False, 'suspended': False} 
```
### end stats
```
```
```javascript
{'radio': {'errors.crc': 0,
           'errors.naks': 0,
           'errors.sequence': 0,
           'errors.timeouts': 18,
           'packets.received': 205L,
           'packets.transmit': 225L},
 'usb': {'errors.crc': 0,
         'errors.naks': 0,
         'errors.sequence': 0,
         'errors.timeouts': 0,
         'packets.received': 3140L,
         'packets.transmit': 3140L}}
```
