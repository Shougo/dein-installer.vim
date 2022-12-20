# Dein-installer.vim


**Dein.vim** installer script from command line.

## Getting started


### Prerequisites

- **Git** must be installed (v2.4.11 or higher)


### Basic installation

To install dein.vim on **UNIX** systems, you should run the install script. To
do that, you may either download and run the script manually, or use the
following **wget** or **curl** command:


#### Wget

```sh
sh -c "$(wget -O- https://raw.githubusercontent.com/Shougo/dein-installer.vim/master/installer.sh)"
```


#### Curl

```sh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/Shougo/dein-installer.vim/master/installer.sh)"
```


#### Manual inspection

> **Note:** _"It's a good idea to inspect the install script from projects you
> don't know."_

You can do that by downloading the install script, then looking through it to
check if the code is safe:

```sh
$ wget https://raw.githubusercontent.com/Shougo/dein-installer.vim/master/installer.sh
$ less installer.sh
$ sh installer.sh
```

The script code is well formatted, so you can better understand all the code.
The script can take some arguments that are listed in **Additional Notes**
section below.


#### Additional Notes

- If you want to overwrite an existent `.vimrc` or `init.vim` config, pass the
  `--overwrite-config` (or in short `-oWC`) argument to the installation
  script. By default, if there's one config already, the new config is
  generated inside the base path.

- The `installer` script has prompt menus that helps you setup everything.
  However, if you want install **Dein.vim** into an different path location,
  pass the location to the end of the script like `sh installer.sh
  ~/.vim/bundle`.

- If you want to complete the setup without the `installer` script prompting,
  Select your editor config location and pass the `--use-vim-config` (or in
  short `-uVC`) or `--use-neovim-config` (or in short `-uNC`) argument to the
  installation script.


### Powershell (Windows)

> The support for Windows requires Powershell.

Open your Powershell and download the script:

```powershell
Invoke-WebRequest https://raw.githubusercontent.com/Shougo/dein-installer.vim/master/installer.ps1 -OutFile installer.ps1
```

After checking the code, allow it to be executed properly:

```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

Lastly, for an installation at the `~/.cache/dein` directory execute:

```powershell
./installer.ps1 ~/.cache/dein
```

## License

Licensed under the [MIT](LICENSE) license.
