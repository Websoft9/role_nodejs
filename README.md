Ansible Role: node.js
=========

Theis role is used for installing NVM, [Node](https://nodejs.org/en/) and YARN, it include some useful tool of Node, e.g  NPM, PM2

## Requirements

Make sure these requirements need before the installation:

| **Items**      | **Details** |
| ------------------| ------------------|
| Operating system | CentOS7.x Ubuntu18.04 AmazonLinux |
| Python version	 | Python2, Python3 |
| Python components |    |
| Runtime |  |


## Related roles

This Role does not depend on other role variables in syntax, but it depend on other role before:

```
roles:
    - {role: role_common, tags: "role_common"}
    - {role: role_nodejs , tags: "role_nodejs  "}
```

## Variables

The main variables of this Role and how to use them are as follows:

| **Items**      | **Details** | **Format**  | **Need to assignment** |
| ------------------| ------------------|-----|-----|
| nodejs_version | e.g "10" | String | No |
| nodejs_applications | - Express | List | No |

Note: 

1. docker_applications is used to install more than two applications


## Example

```
nodejs_version: "14"
nodejs_applications
  - express
```

## FAQ

#### Could this role support muti-version of Node?
Their only one version for default installation, but you can use `nvm` to install more version of Node
