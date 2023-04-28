# Mavick

Mavick is an Ansible-based tool written in Go for configuring operating systems to a predefined configuration. With Mavick, you can automate the setup and configuration of your favorite operating system and the applications you use on a daily basis.

## Installation

To install Mavick, you can download the latest binary release from the [releases](https://github.com/yourusername/mavick/releases) page. Alternatively, you can also build Mavick from source by following these steps:

1. Clone the Mavick repository:

   ```shell
   git clone https://github.com/legitShivam/mavick.git
   cd mavick
   ```

2. Build Mavick:

   ```shell
   go build
   ```

## Usage

To use Mavick, you first need to create a configuration file. The configuration file is a YAML file that specifies the operating system and the applications you want to configure. Here is an example configuration file:

```yaml
---
os: ubuntu
packages:
  - vim
  - git
  - curl
  - htop
  - neofetch
```

To run the configuration, simply pass the configuration file to the `mavick` binary:

```shell
./mavick --config /path/to/config.yaml
```

Mavick will then use Ansible to configure your operating system to the specified configuration.

## Contributing

We welcome contributions to Mavick! If you find a bug or have a feature request, please [open an issue](https://github.com/legitShivam/mavick/issues) to let us know.

If you would like to contribute code, please follow these steps:

1. Fork the Mavick repository and clone it to your local machine.
2. Create a new branch for your changes: `git checkout -b my-feature-branch`.
3. Make your changes and write tests for them. Ensure that all tests pass by running `go test ./...`.
4. Commit your changes and push them to your forked repository.
5. Submit a pull request to the main Mavick repository.

> Please ensure that your code adheres to the project's code style and follows best practices for Go development.

## License

Mavick is licensed under the [MIT License](./LICENSE).
