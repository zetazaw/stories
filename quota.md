## Quota Card

### Stories

[-] Card Reader in central
### Components
1. ESP32 or ESP8266
2. RF Reader

or RF Card Reader with USB (CR100)

### Story
1. Read card data first. [count, date/timestamp, station_number, licence_plate, expire_date]
2. Check card data [ expire_date, timestamp, count, UID ] but all are new
3. Write card data [ card_key, licence_plate, expire_date, timestamp, count, UID, device_serial ]
4. LED output and Buzzer output and LCD output for success or fail


[-] Card Reader in stations
### Components
1. ESP32 or ESP8266
2. RF Reader
3. LCD
4. RTC
5. Buzzer

### Story
1. Read card data first. [count, date/timestamp, station_number, licence_plate, expire_date]
2. Check card data [ expire_date, timestamp, count, UID]
3. Write card data [ timestamp, count, station_number ]
4. Response on decision parameters [ UID, count ]
5. LED output and Buzzer output and LCD output

[-] Cards
### Story
1. Accept [ new_card_key, licence_plate, expire_date, timestamp, count, UID, device_serial ] on central
2. Accept [ timestamp, count, station_numbers ] 

