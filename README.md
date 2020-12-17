Ansible Role: node.js
=========

Theis role is used for installing NVM, [Node](https://nodejs.org/en/) and YARN, it include some useful tool of Node, e.g  NPM, PM2

## Requirements

运行本 Role，请确认符合如下的必要条件：

| **Items**      | **Details** |
| ------------------| ------------------|
| Operating system | CentOS7.x Ubuntu18.04 AmazonLinux |
| Python 版本 | Python2  |
| Python 组件 |    |
| Runtime |  |


## Related roles

本 Role 在运行时需要确保已经运行：common。以下为例：

```
roles:
    - {role: role_common, tags: "role_common"}
    - {role: role_nodejs , tags: "role_nodejs  "}
```


## Variables

本 Role 主要变量以及使用方法如下：

| **Items**      | **Details** | **Format**  | **是否初始化** |
| ------------------| ------------------|-----|-----|
| nodejs_ver | [ 10 ] | 字符串 | 否 |



## Example

```
- name: Node.js
  hosts: all
  become: yes
  become_method: sudo 
  vars_files:
    - vars/main.yml 

  roles:
    - { role: role_common }
    - { role: role_node.js   }
    ...
```

## FAQ


