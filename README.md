# School Register
> A Java Swing desktop app for an electronic school register — separate logins and views for pupils, teachers and educators, backed by a MySQL database. Built for a university course.

## Table of contents
* [General info](#general-info)
* [Screenshots](#screenshots)
* [Setup](#setup)
* [Status](#status)
* [Contact](#contact)

## General info
Models a school's day-to-day records — classes, subjects, grades, notes and absences — with role-based logins for pupils, teachers, and educators.

* `Users` – a `Person` base class with `Pupil`, `Teacher`, `Educator` and `Administrator` subclasses
* `System` – domain entities: `Class`, `Subject`, `Grade`, `Note`, `Absence`
* `GUI` – Swing panels for each role (login screens, grading, notes, teacher search, and more)
* `Register` – the app entry point and the MySQL connection layer
* `database/school_register.sql` – the MySQL schema

## Screenshots
![Example screenshot](./img/screenshot1.png)
![Example screenshot](./img/screenshot2.png)
![Example screenshot](./img/screenshot3.png)
![Example screenshot](./img/screenshot4.png)
![Example screenshot](./img/screenshot5.png)

## Setup
1. Import `database/school_register.sql` into a local MySQL/MariaDB instance named `SchoolRegister`.
2. Add the two jars in `/resources` to the project: `mysql-connector-java-8.0.13` (DB driver) and `rs2xml` (renders query results in the app's tables).
3. `SQLConnection.java` connects to `jdbc:mysql://localhost/SchoolRegister` as `root` with no password — update this for your own environment.

## Status
**Archived** — not actively maintained.

Written in early 2019 for a university course. Development stopped with the pupil, teacher and educator roles working; the planned administrator role and a few smaller features were never implemented.
