# Wzpaper
This script is a background manager that can allow you to :
- Changes your wallpaper randomly.
- Change your wallpaper randomly at any given time in hours.
- Choise your wallpaper.

# How to run Wzpaper ?
first of all you have to give the right of execution to wzpaper.
```
$ chmod +x ./wzpaper
```

Then it is necessary to indicate to the script where is the folder which contains your background.
```
$ wzpaper -i
```

# How to use Wzpaper ?
To know how to use Wzpaper made :
```
$ wzpaper --help
USAGE
	wzpaper [options]
DESCRIPTION
	-h	Print the different information of this programme.
	-i	Initialize information to use the program (mandatory first time).
	-r	Changes your wallpaper randomly.
	-p	<time> Change your wallpaper randomly at any given <time> in hours.
	-c	Choise your wallpaper.
```

# How to use the program background change ?
The "-c" option allows you to program the change of the background according to the time you have given.

for exemple I would like my background to change randomly every 15 minutes.
I should do :
```
$ wzpaper -c 0.25
```
Here 0.25 hour is equal to 15 minutes.
You can check this with the following formula:
hour * 60

# How to autostart with i3 ?
In your i3 config file add these lines :
```
exec wzpaper -c 0.25
```

# To stop it
```
$ killall wzpaper
```