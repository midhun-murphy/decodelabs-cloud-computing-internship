# Week 3 - AWS RDS MySQL Integration

## Project Overview

This project demonstrates how to securely connect an Amazon EC2 instance to an Amazon RDS MySQL database using VPC Security Groups.

## Architecture

Local Machine
      |
      v
Amazon EC2 (Ubuntu)
      |
      v
Amazon RDS MySQL

## Services Used

- Amazon EC2
- Amazon RDS MySQL
- VPC
- Security Groups
- SSH
- MySQL Client

## Steps Performed

1. Created Amazon RDS MySQL Instance
2. Created Amazon EC2 Ubuntu Instance
3. Configured Security Groups
4. Connected EC2 to RDS
5. Installed MySQL Client
6. Logged into RDS Database
7. Created Database and Tables
8. Inserted Sample Records
9. Queried Data Successfully

## SQL Commands

### Create Database

```sql
CREATE DATABASE internship_db;
```

### Use Database

```sql
USE internship_db;
```

### Create Table

```sql
CREATE TABLE interns (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    department VARCHAR(100),
    email VARCHAR(100),
    joining_date DATE
);
```

### Insert Records

```sql
INSERT INTO interns
(name, department, email, joining_date)
VALUES
('Midhun Kumar', 'Cloud Computing', 'midhun@gmail.com', '2026-06-20'),
('Rahul', 'DevOps', 'rahul@gmail.com', '2026-06-20'),
('Priya', 'AWS', 'priya@gmail.com', '2026-06-20');
```

### View Records

```sql
SELECT * FROM interns;
```

## Screenshots

Add all screenshots in the screenshots folder.

## Learning Outcomes

- AWS RDS Setup
- EC2 to RDS Connectivity
- Security Group Configuration
- MySQL Administration
- Cloud Database Management

## Author

Midhun Kumar
DecodeLabs Cloud Computing Internship
