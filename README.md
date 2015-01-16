# OneWire2Graphite
Spark core code to poll 1-wire temperature sensors and send to [graphite](https://github.com/graphite-project/graphite-web) server. It works well enough for me but there seem to be some bugs. 

# Requires

* [SparkCoreDallasTemperature](http://github.com/tomdeboer/SparkCoreDallasTemperature)

* [OneWireSpark](http://github.com/Hotaman/OneWireSpark)

# Bugs
* Seems to fail sending data too often
* Temperature reading are occasionally set to 85/185 which I read could be caused by 

> if it has not had a chance to do a complete convert_t by the time you read_t on it
[this forum post](http://comments.gmane.org/gmane.comp.file-systems.owfs.devel/7810)
