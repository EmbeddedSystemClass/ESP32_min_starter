# ESP32 Starter template

## prerequisites

1. setup your toolchain and ESP-IDF as described in the [official documentation](https://docs.espressif.com/projects/esp-idf/en/latest/get-started/#step-1-set-up-the-toolchain)

2. add an environment variable called `IDF_TOOLS` that points to the tools directory in the extensia  installation (C:\Program Files\Espressif\ESP-IDF Tools\tools)
   
3. ensure tour ESP32 is plugged in and that a COM PORT is established (You may need a driver for your ESP32 dev board)

## vs code intellisense

intellisense should just work so long as you have set up the IDF_PATH environment variable as described in the [official documentation] [official documentation](https://docs.espressif.com/projects/esp-idf/en/latest/get-started/#step-1-set-up-the-toolchain) and the IDF_TOOLS as described above.

>NB. you may meed to do an initial build and restart vscode before it can resolve all variables.

## flashing the esp32

1. in vs code, open a new terminal by pressing ctrl + `(or pressing F1 and typing `open new terminal`)
2. type the following command

```bash
idf.py -p [your com port] flash monitor
