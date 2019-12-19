# Item Catalog

## About

This is a project for the Udacity Full Stack Nanodegree. The Item Catalog project involves developing an application that lists items within categories and that provides user registration and authentication systems. This is a RESTful web application that allows users to perform Create, Read, Update, and Delete operations.

This program uses third-party auth via Google. 

## Tech

- Python
- CSS
- Bootstrap
- Google Login
- Flask
- SQLAchemy
- OAuth
- Jinja2

## Requirements

- [Vagrant](https://www.vagrantup.com/)
- [Udacity Vagrantfile](https://github.com/udacity/fullstack-nanodegree-vm)
- [VirtualBox](https://www.virtualbox.org/wiki/Downloads)

## Getting Started

- Install Vagrant and VirtualBox
- Download Vagrantfile from the Udacity
- Download this repo into the `catlog/item-catalog` directory found in the Vagrant directory
- Run `vagrant up` to run the virtual machine, then `vagrant ssh` to login
- In the main directory run `sudo pip install -r requirements`
- Type `python application.py` from within its directory to run the app
- In the browser go to `http://localhost/categories` to access the application

## JSON Endpoints

`/api/v1/catalog.json` - Returns JSON of every item

`/api/v1/categories/<int:category_id>/item/<int:catalog_item_id>/JSON` - Returns JSON of a selected item in catalog

`/api/v1/categories/JSON` - Returns JSON of all categories

## REST Endpoints

### CRUD for categories

`/` or `/categories` - Returns catalog page with all categories and recently added items

`/categories/new` - Allows user to create new category

`/categories/<int:category_id>/edit/` - Allows user to edit an existing category

`/categories/<int:category_id>/delete/` - Allows user to delete an existing category
