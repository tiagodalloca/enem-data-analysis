# Setting up

## Requirements

- `sqlite3`
- `python3`
	- `pandas`
	- `numpy`
	- `seaborn`
- `jupyter`
	
Make sure you have everything installed before proceding.

## Downloading and configuring the dataset

1. Run the script `setup-dataset`
2. Wait a while
3. You're done :)

Oh, it'll probably **work only on Linux** (maybe OSX, definitely not on Windows)

## Dataset dictionary

It can be found in portuguese at `./microdados_enem2017/DICIONÁRIO/Dicionário_Microdados_Enem_2017.xlsx`

If everything was configured correctly, you should be able to use the dataset located in a sqlite3 database at the table enem from `./microdados_enem2017/database.db`.

All letter-encoded categorical variables were transformed to integers, as 

``` 
A -> 0
B -> 1
C -> 2
...
```

UFs were encoded from 0 to 26 in alphabetical order.

Values already encoded as integers were left the same. Some columns I judged unnecessary were kept out of the dataset.
