---
content_title: Nodtlk Options
---

`nodtlk` is a command line interface (CLI) application. As such, it can be started manually from the command line or through an automated script. The behavior of `nodtlk` is determined mainly by which plugins are loaded and which plugin options are used. The `nodtlk` application features two main option categories: *nodtlk-specific* options and *plugin-specific* options.

## Nodtlk-specific Options

Nodtlk-specific options are used mainly for housekeeping purposes, such as setting the directory where the blockchain data resides, specifying the name of the `nodtlk` configuraton file, setting the name and path of the logging configuration file, etc. A sample output from running  `nodtlk --help` is displayed below, showing the nodtlk-specific options (Note: the plugin-specific options have been excluded for clarity):

```console
Application Config Options:
  --plugin arg                          Plugin(s) to enable, may be specified 
                                        multiple times

Application Command Line Options:
  -h [ --help ]                         Print this help message and exit.
  -v [ --version ]                      Print version information.
  --full-version                        Print full version information.
  --print-default-config                Print default configuration template
  -d [ --data-dir ] arg                 Directory containing program runtime 
                                        data
  --config-dir arg                      Directory containing configuration 
                                        files such as config.ini
  -c [ --config ] arg (=config.ini)     Configuration file name relative to 
                                        config-dir
  -l [ --logconf ] arg (=logging.json)  Logging configuration file name/path 
                                        for library users
```

## Plugin-specific Options

Plugin-specific options control the behavior of the nodtlk plugins. Every plugin-specific option has a unique name, so it can be specified in any order within the command line or `config.ini` file. When specifying one or more plugin-specific option(s), the applicable plugin(s) must also be enabled using the `--plugin` option or else the corresponding option(s) will be ignored.
