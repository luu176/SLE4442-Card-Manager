# SLE4442-Card-Manager

With SLE4442 Card Manager you can perform all basic operations on you memory cards, including: inizialization, reading memory, presenting security PIN, changing PIN, writing to memory, permanently protecting the first 32 bytes from writing.

## Getting Started

> [!WARNING]
> SLE4442 allows 3 attempts when entering the pin, if you fail authentication three times, you'll be permanently locked out of accessing the chip. 

[SLE4442 Datasheet ](https://www.digikey.com.au/htmldatasheets/production/433077/0/0/1/sle-4442-m3-2.html)

In order to write to the card you must first enter the 3 bytes security PIN (usually set by manufacturers to FF,FF,FF).

once authenticated, you can change the pin & write to the memory, the first 32 bytes of which can be permanently locked to prevent further writing.


### Requirements

You must have a PCSC smartcard reader capable of interfacing with SLE4442 chips (synchronous)

>[!NOTE]
> This works with HID omnikey smartcard readers

[Python 3](https://www.python.org/downloads/) 

[Pyscard](https://github.com/LudovicRousseau/pyscard) python lib


### Installing

Clone the repo and run `sle4442.py` to run the tool. 


## Acknowledgments

This is an updated version (with UI Stripped) of the [SLE4442-Card-Manager](https://github.com/hvfrancesco/SLE4442-card-manager) by [hvfrancesco](https://github.com/hvfrancesco)
With thanks to the [pyscard](https://github.com/LudovicRousseau/pyscard) devs 

## License 
This tool is protected under the [MIT](https://en.wikipedia.org/wiki/MIT_License) License, see LICENSE file for more information. 

## Support
For any support you may need, file a github issue. 

