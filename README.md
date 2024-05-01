# Bike-Sharing-Dataset-Analysis

## About This Dataset

City of Washington, D.C. which is the capital of the United States, there is a bicycle rental business called Capital Bikeshare DC. The bicycle rental system is the latest generation of traditional bicycle rental where all membership, rental and return are automated.

Currently, there are more than 500 bicycle rental programs worldwide covering up to 500 thousand bicycles. Seeing the large interest and business potential of bicycle rental, the characteristics of the data produced by this program are interesting for research. This dataset focuses on the correlation between environmental conditions and seasons in the hourly, daily and monthly ranges on rental behavior. Data was recorded from 2011 to 2012.

The results of this bicycle rental data analysis can produce new insights for development or improvement in the bicycle rental business.

## Dataset Dictionary

- instant: record index
- dteday : date
- season : season (1:springer, 2:summer, 3:fall, 4:winter)
- yr : year (0: 2011, 1:2012)
- mnth : month ( 1 to 12)
- hr : hour (0 to 23)
- holiday : weather day is holiday or not (extracted from http://www.freemeteo.com)
- weekday : day of the week
- workingday : if day is neither weekend nor holiday is 1, otherwise is 0.
- weathersit :
  - 1: Clear, Few clouds, Partly cloudy, Partly cloudy
  - 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
  - 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
  - 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
- temp : Normalized temperature in Celsius. The values are derived via (t-t_min)/(t_max-t_min), t_min=-8, t_max=+39 (only in hourly scale)
- atemp: Normalized feeling temperature in Celsius. The values are derived via (t-t_min)/(t_max-t_min), t_min=-16, t_max=+50 (only in hourly scale)
- hum: Normalized humidity. The values are divided to 100 (max)
- windspeed: Normalized wind speed. The values are divided to 67 (max)
- casual: count of casual users
- registered: count of registered users
- cnt: count of total rental bikes including both casual and registered

## How to Run Dashboard file

1. Download dashboard.py in Dashboard Folder
2. Go to Google Colab in your browser
```
https://colab.google/
```
3. Add dashboard.py to Files
   - Click **Files** in the left navbar
   - New menu will show up, click **Upload to session storage** button at the top of the menu. button position on the far left
   - Choose dashboard.py then upload it
4. Streamlit Installation
```
!pip install streamlit
```
5. Get Tunnel Password
```
! wget -q -O - ipv4.icanhazip.com
```
6. Run dashboard.py file
```
! streamlit run dashboard.py & npx localtunnel --port 8501
```
Wait a little bit... then it will give you a link. This is the link you're looking for
```
Collecting usage statistics. To deactivate, set browser.gatherUsageStats to false.
You can now view your Streamlit app in your browser.
Network URL: http://172.28.0.12:8501
External URL: http://35.245.128.170:8501

npx: installed 22 in 3.078s
your url is: https://stupid-adults-melt.loca.lt ----------------> this is the link, click this link
```
7. Paste the Tunnel Password to **Tunnel Password:**
8. Click **Click to Submit**, there you go
