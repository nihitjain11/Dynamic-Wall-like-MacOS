# Dynamic-Wall-like-MacOS
MacOS like dynamic wallpaper for Linux Ubuntu


# Setup Instructions:
1. download and extract the zip(containing 16 images) from this repo
2. paste the code given below at the end in your ubuntu crontab file 
3. To edit crontab, Open your terminal and enter
`$ crontab -e`
# And then paste the following 
```
0 0-23/3 * * * gsettings set org.gnome.desktop.background picture-uri "file://~/Downloads/mojave_dynamic/$(($(date +%H)*2/3)).jpeg"

30 1-23/3 * * * gsettings set org.gnome.desktop.background picture-uri "file://~/Downloads/mojave_dynamic/$((($(date +%H)*2/3)+1)).jpeg"
```
