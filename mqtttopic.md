## How do you design MQTT topics and payloads for smart washing machine

1. สถานะเครื่องซักผ้า
    - topic:v1cdti/app/get/1212312121/model-01/sn-001/
    - payload
        - {"STATUS": "POWER ON|START|STOP|FINISHED|POWERED OFF"}
1. เซนเซอร์ภายในเครื่องซักผ้า
    - topic:v1cdti/app/get/1212312121/model-01/sn-001
    - payload
        - {"temperature": "25.2"}
        - {"weight_cloth": "2"}
        - {"inbalance": "9.5"}
        - {"rotation": "20"}
        - {"้huminity": "60"}
        - {"load": "5"}
        - {"water_level": "3"}
        - {"detergent": "2"}
        - {"noise_anomaly": "2.5"}
        

 1. เซนเซอร์ภายนอกเครื่องซักผ้า
    - topic:v1cdti/app/get/1212312121/model-01/sn-001
    - payload
        - {"temperature": "30.7"}
        - {"huminity": "20"}
        - {"vibration": "0.2"}
        - {"radar": "1"}
        - {"current": "121"}
        - {"air_pressure": "210"}
        - {"touch_open/close": "0"}