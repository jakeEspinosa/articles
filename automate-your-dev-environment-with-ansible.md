After weeks of research, you finally unbox your new computer and start setting it up. It boots, you install your OS, and then the magic happens! Except, it doesn't. You still need to install all of your software. As fast as your new SSD, your excitement is replaced with dread...

This article will not teach you how to use Ansible or write playbooks. Rather, I aim to inspire you to automate your environment setup and think about other ways to increase productivity and decrease brain cycles spent on insignificant things.

## What Is Ansible?
Ansible is an open-source tool for configuration management commonly used in cloud environments. It uses yaml to specify the desired end state of a system declaratively. 

## The Problem Ansible Solves
If you're like me, you program in multiple languages and thus need numerous environments. You also need the environments to be consistent across machines. Manually installing everything can be an error-prone slog and cuts into precious time you could use for anything else. Instead, consider writing an Ansible playbook to do it for you.

### Playbook Ideas
- Install and configure node/npm
- Install python
- Configure git with your username, email, and SSH keys
- Clone your personal project repos from Github

## Takeaway
Consider spending a few hours now to save countless hours on installing and configuring software. Automating your environment with Ansible isn't something flashy and exciting, but it will free up precious time and allow you to focus on the code.
