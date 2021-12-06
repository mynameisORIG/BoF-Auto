#BoF-Auto

The purpose of this script is to make Buffer Overflows easier.

## Notes from Creator

This assumes you are running a Kali OS system.

This has only been tested on Try Hack Me's
1. Buffer Overflow Prep
	1.1 OVERFLOW1

## Commands

### creating a fuzzer in python3
You will still need to provide an IP.

``` bash
sudo ./BoF -f
```

### Using pattern-create
This uses /usr/share/metasploit-framework/tools/exploit/pattern_create.rb to help start create the first payload.

In this example, lets assume the offset is around 400 bytes and the program range is between 1900 to 2000 bytes.

``` bash
./BoF -pc 2400
```
### netcat listener
This allows an attacker to listen to a certain port if the desired program is running on a certain port you can listen too.

``` bash
./BoF -nc -RH <RemoteIP> -RP <RemotePort>
```

