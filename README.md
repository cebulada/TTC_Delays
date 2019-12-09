## TTC_Delays

## Authors

- [Daniel Adam Cebula](https://github.com/cebulada)
- [William Lim](https://github.com/naga456)
- [Rohan Chaudhari](https://github.com/focusrohan)
- [Sofiat Ishola](https://github.com/sishola)
- [Tom Callegari](https://github.com/TomCallegari)

___

## Version 2.0.0 (Adapted from [ttc-delays](https://github.com/sishola/ttc-delays))

___

## Getting Started / Installation

View this [PRESENTATION.md](PRESENTATION.md) for a summary of findings or the [PowerPoint](TTC_Delays_PowerPoint.pptx)

Or

Download the compressed [GitHub Repository](https://github.com/cebulada/TTC_Delays.git)

Then view the [PRESENTATION.md](PRESENTATION.md) file or the [PowerPoint](TTC_Delays_PowerPoint.pptx)

Or

```
$ git clone https://github.com/cebulada/TTC_Delays.git
```

Then view the [PRESENTATION.md](PRESENTATION.md) file or the [PowerPoint](TTC_Delays_PowerPoint.pptx)

___

## Prerequisites

### Optional - [Detailed Instructions](ftp://client_climate@ftp.tor.ec.gc.ca/Pub/Get_More_Data_Plus_de_donnees/)

### 1. Install [cygwin64](https://www.cygwin.com/) (setup-x86_64.exe - Executable)

### 2. Install [wget](https://cygwin.com/packages/summary/wget.html) package on cygwin64

### 3. Obtain [Historical Weather Data](http://www.climate.weather.gc.ca) by cygwin64 command line entries (Optional - .csv Files already Included)
```
$ for year in `seq 1998 2008`;do for month in `seq 1 12`;do wget --content-disposition "http://climate.weather.gc.ca/climate_data/bulk_data_e.html?format=csv&stationID=1706&Year=${year}&Month=${month}&Day=14&timeframe=1&submit= Download+Data" ;done;done

WHERE; 
• year = change values in command line (`seq 1998 2008)
• month = change values in command line (`seq 1 12)
• format= [csv|xml]: the format output
• timeframe = 1: for hourly data 
• timeframe = 2: for daily data 
• timeframe = 3 for monthly data 
• Day: the value of the "day" variable is not used and can be an arbitrary value 
• For another station, change the value of the variable stationID
• For the data in XML format, change the value of the variable format to xml in the URL. 
```
### List of [wgets](./Jupyter-Notebooks/Toronto_Weather/How_to_obtain_Raw_Data/Cygwin_wgets.txt)

### 4. Obtain [TTC Subway Delay Data](https://open.toronto.ca/dataset/ttc-subway-delay-data/), [TTC Bus Delay Data](https://open.toronto.ca/dataset/ttc-bus-delay-data/) and [TTC Streetcar Delay Data](https://open.toronto.ca/dataset/ttc-streetcar-delay-data/) data (Optional - .xlsx files already included)

### 5. Obtain a list of [Holidays](https://github.com/uWaterloo/Datasets/blob/master/Holidays/holidays.csv) from 2012 - 2020 (Optional - .csv file already included)

### Required

### 5. Installation of Python 3.7.5 ([Instructions](https://www.python.org/downloads/release/python-375/))

### 6. Installation of Jupyter Notebook/Lab ([Instructions](https://jupyter.org/install))

### 7. Install Scientific Python Distribution ([Instructions](https://www.scipy.org/install.html))
#### Specifically pandas, NumPy, Matplotlib and SciPy
___

## Versioning

[SemVer](http://semver.org/) for versioning.

___

## License

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE.md](LICENSE.md) file for details

___