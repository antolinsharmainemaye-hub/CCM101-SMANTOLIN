# Security Audit Report

## 1. Principle of Least Privilege (PoLP)

The Principle of Least Privilege means giving users and applications only the permissions they need to perform their assigned tasks. It is important in cloud environments because it helps prevent unauthorized access and reduces the damage that could happen if an account is compromised.

## 2. Attack Surface

The attack surface refers to all the points where an attacker could try to access or compromise a virtual machine. These include open network ports, running services, applications, and user accounts. Reducing unnecessary services and closing unused ports helps minimize security risks.

## 3. Default Deny Policy

A Default Deny Policy blocks incoming network traffic unless it is explicitly allowed by a firewall rule. This is safer than trying to block individual attackers because unknown or unauthorized connections are automatically denied, while only approved services can receive traffic.