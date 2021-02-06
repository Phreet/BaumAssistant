# Mold indicator

### Indicator to inform about necessary air vent when value rises above approx. 70%
* Resource: https://www.home-assistant.io/integrations/mold_indicator/
* Based on each room specific Aqara multisensor and external weather input
* calibration_factor = (temp_indoor - temp_outdoor) / (temp_criticalpoint - temp_outdoor)

The Mold Indicator sensor integration consumes information of two temperature sensors and a humidity sensor to give an indication for possible mold growth in your home. In case of bad ventilation and insulation, the indoor humidity may lead to condensation on cold surfaces as the windows or even walls. Condensation or a high relative humidity near those cold surfaces leads to a higher risk for mold growth. This sensor integration estimates the temperature at a pre-calibrated critical point in the room (the coldest surface) and calculates the relative humidity of the air at that point. If the sensor value rises above approximately 70 percent, mold growth might occur and the room should be ventilated. At 100%, the air humidity condensates at the critical point.

The sensor data may be used e.g., to signal bad air quality (too high air humidity) or to automate operation of indoor air humidifiers to keep the indoor humidity at an optimum.