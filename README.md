# MouseTools

A Python wrapper for the Disney API. Data is pulled directly from Disney. This package supports Walt Disney World and Disneyland.


### Installation
You can install using pip:
```bash
pip install MouseTools
```
or because version 2.0.0 is in beta right now and might be updated frequently:
```bash
pip install git+https://github.com/scaratozzolo/MouseTools
```

Installation will take some time as the initial database is set up and created. There is a lot of data to load and parse so just be patient.



### Example usage:
```python
import MouseTools

wdw_dest = MouseTools.Destination(80007798)
print(wdw_dest.get_park_ids())

dlr_dest = MouseTools.Destination(80008297)
print(dlr_dest.get_attraction_ids())

mk = MouseTools.Park(80007944)
print(mk.get_wait_times())

pirates = MouseTools.Attraction(80010177)
print(pirates.get_wait_time())
print(pirates.get_possible_ids())

```


I created this project to help with another project found [here](https://github.com/scaratozzolo/WDWWaits). Some parts of the wrapper were created with that in mind.
