# Directus API - (Postman)

## 🧐 About

This repository will be aiming to explain the steps required to check/fetch data from the Directus API using Postman.

## 🏁 Getting Started

These instructions will get you ready for the Directus API testing using Postman

### Prerequisites

Do install the following applications

- [Postman](https://www.postman.com/) - API Platform

### Installing

A step by step guide that tell you how to get Postman Installed .

- [Postman](https://learning.postman.com/docs/getting-started/installation-and-updates/#:~:text=and%20updating%20Postman-,Postman%20is%20available%20on%20the%20web%20at%20go.postman.co,select%20Download%20for%20your%20platform.) - Installation Guide

## API testing

### Step 1: Directus API Token

Login to Directus and open the User Management module. If you haven't created an API user, create a new user now. At the bottom of the API user, there is a field labelled Token. By default this is always blank. If empty, type a token now and save the user. There are some great token generators on Google. Copy the token from the field.

<p align="center">
  <a href="" rel="noopener">
 <img  src="https://cdn.discordapp.com/attachments/907964824372252674/1100349158990295112/image.png" alt="Project logo"></a>
</p>

### Step 2: Permissions

Permissions are a very important part of APIs. It keeps you data safe from accidental or deliberate changes that cause havoc on your system. It's very tempting to use the Administrator privilages, but it's definately worth having a dedicated API Role.

<p align="center">
  <a href="" rel="noopener">
 <img  src="https://cdn.discordapp.com/attachments/907964824372252674/1100349556429963295/image.png" alt="Project logo"></a>
</p>
Create a new role in Directus and assign it to the API user. On the role, you'll see a list of all the collections in Directus and the permissions for Create, View, Edit, Delete and Share. Simply grant access to the required actions for each collection. Bare in mind, relational tables need to be visible to return the data and editable to write relational data.

### Step 3: Create a Postman Collection

In Postman it's important to create a collection for each service. In this cas you can call it Directus, or something relative to the project. To create a new collection, click the + (plus) symbol next to the Collection menu button then name your collection.

Next, change the Authorization type to Bearer Token.

<p align="center">
  <a href="" rel="noopener">
 <img  src="https://learndirectus.com/content/images/size/w1000/2022/03/image.png" alt="Project logo"></a>
</p>

A Token field will appear. Paste the token from the Directus API and click Save. If the save button is not showing you need to close the right-side panel. pic
You can add as many collections as you need and you can add multiple Directus projects with ease.

### Step 4: Create API Requests

Now that you have a collection, you can create some requests. Right click on the collection in you left navigation or click the ellipsis menu icon when you hover the mouse on the collection. Choose Add Request.

Enter the API URL and click on get Request.

<p align="center">
  <a href="" rel="noopener">
 <img  src="https://learndirectus.com/content/images/size/w1000/2022/03/image-4.png" alt="Project logo"></a>
</p>

### Step 5: Results

<p align="center">
  <a href="" rel="noopener">
 <img  src="https://cdn.discordapp.com/attachments/907964824372252674/1100350281855799327/image.png" alt="Project logo"></a>
</p>
