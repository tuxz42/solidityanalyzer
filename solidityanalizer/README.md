# Installation
First, make sure that you have [Rust installed](https://www.rust-lang.org/tools/install). Then you can choose either of the installation methods by entering the corresponding command in your terminal below.

&nbsp;
### Install from crates.io
```
cargo install solstat
```


```

&nbsp;
# Usage
Now that you have solstat involved, you can use the `solstat` command from anywhere in your terminal. By default, solstat looks for a `./contracts` directory and analyzes every file within the folder. If you would like to specify the directory solstat should use, you can pass the `--path` flag (ex. `solstat --path <path_to_dir>`). 

In the default configuration, solstat runs analysis for every [currently included Optimization, Vulnerability and QA] however if you would like to run analysis for select patterns, you can create a `.toml` file for your custom configuration.  Check out the [default solstat.toml configuration] for reference. After creating a custom `.toml` file, make sure to pass the `--toml` flag when running solstat (ex. `solstat --toml <path_to_toml_file>`).

Once solstat runs its analysis, a report will be generated and output as `solstat_report.md`.

At any point you can use `solstat --help` to see a list of all commands and options.

```
Usage: solstat [OPTIONS]

Options:
  -p, --path <PATH>  Path to the directory containing the files solstat will analyze. The default directory is `./contracts`
  -t, --toml <TOML>  Path to the toml file containing the solstat configuration when not using the default settings.
  -h, --help         Print help information
```

&nbsp;
# Contributing
First off, thanks for taking the time to contribute! Contributions are welcomed and greatly appreciated.

