# Welcome to the Query

<img align="right" src="./ferry.png" height="150px" alt="the rust mascot">

The **Query** is a command-line tool developed in Rust that empowers users to
seamlessly interact with RESTful APIs from their terminal. Whether you're
fetching data, posting information, or managing API resources, this CLI tool
simplifies the process by offering a straightforward and intuitive interface.

> [!NOTE]
> This project is for practice Rust 

## Key Features

- **Easy Configuration:** Configure the base URL, authentication, and custom
  headers for your API requests.
- **HTTP Methods:** Supports various HTTP methods, including GET, POST, PUT,
  DELETE, and more.
- **Testing and Documentation:** Write tests to ensure functionality and provide
  detailed documentation for users.

## Example CLI

Init configuration for query cli:

```sh
query --config init

Created file successfuly! # Generate file `query.json`
```

command:

```sh
query --method get --url languagues
```

response:

```log
[
  {
    "name": "Java",
    "publish_date": "1995",
    "description": "Java is a widely used programming language that is designed to be platform-independent."
  },
  {
    "name": "C++",
    "publish_date": "1985",
    "description": "C++ is a general-purpose programming language that supports object-oriented programming."
  },
  {
    "name": "Python",
    "publish_date": "1991",
    "description": "Python is a high-level programming language known for its simplicity and readability."
  },
  {
    "name": "C#",
    "publish_date": "2000",
    "description": "C# is a modern programming language developed by Microsoft for building a variety of applications."
  }
]
```

### unzip is required

The program [`unzip`](https://linux.die.net/man/1/unzip) is a requirement for
the Shell installer.

```sh
$ curl -fsSL https://query.dev/install.sh | sh
Error: unzip is required to install Query (see: https://github.com/castrogarciajs/query#unzip-is-required).
```

> [!IMPORTANT]
> These steps are when installing _query_

**When does this issue occur?**

During the `install.sh` process, `unzip` is used to extract the zip archive.

**How can this issue be fixed?**

You can install unzip via `brew install unzip` on MacOS or
`apt-get install unzip -y` on Linux.

## License

This project is LICENSE **MIT**.
