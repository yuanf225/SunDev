# SunDev
SunDev is developed with the micro-framework Silex.

# Requirements
-  HTTP server handling php
-  [Composer](https://getcomposer.org/)

# Installation
- Clone this repository into a folder of your choice.
- Run `composer update` at the root of the SunDev folder.
- Install the following databases, included in repository (TODOOO):
    - dbc
    - suntools
    - world: your live world
    - test_world: your ptr world (can be the same as world)
- Create et edit `app/config.php` from `app/config.sample.php`
- Edit your host file so that `dev.sunstrider.com` points to your server. For example:   
        `127.0.0.1  dev.sunstrider.com`
- Create a virtual host in your web server config.
    Example of Apache config:

        <VirtualHost dev.sunstrider.com:80>
            DocumentRoot "D:/htdocs/SunDev/web"
            ServerName dev.sunstrider.com
        </VirtualHost>

# Usage

- Access:  
Just go into the address you put into your host file, such as `dev.sunstrider.com`  
The following dummy users are already created in the database included (user:password):
    - admin:admin
    - full:full
    - dev:dev
    - tester:tester

- Creating a user  
    `dev.sunstrider.com/admin/user/add`

# Development
* SmartAI:
  SmartAI Web Editor inspired by SmartAI Editor by Discover- using a custom jQuery library(smartai.js), [dataTables.js](http://www.datatables.net/), [chosen.js](http://harvesthq.github.io/chosen/) and [jQuery.xcolor.js](https://github.com/infusion/jQuery-xcolor).

* SunDungeon:
  Checklist of points to check for every NPCs in Outland Dungeons.

# Testing
* SunQuests:
  Checklist of points to check for every quests in Outland including zones, dungeons, raids and cities.

# Roles
| Role  		| Access      							|
|---------------|---------------------------------------|
| ROLE_ADMIN    | Validate the code in review           |
| ROLE_FULL     | Access Development and Testing parts  |
| ROLE_DEV      | Access Development part               |
| ROLE_TESTER   | Access Testing part                   |

# To Do
Implement:
* SunClasses
* SunEquip
* SunGossip
* SunWaypoints
* SunWorld