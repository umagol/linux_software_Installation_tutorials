# MySQL

<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#how-to-install-mysql-on-ubuntu-1804">Install On ubuntu 18.04</a>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>


## - Prerequisites
  - One Ubuntu 18.04 server set up by following this initial server setup guide, including a non-root user with sudo privileges and a firewall.
  

### How To Install MySQL on Ubuntu 18.04
<br />

#### - Installing MySQL
On Ubuntu 18.04, only the latest version of MySQL is included in the APT package repository by default. At the time of writing, that’s MySQL 5.7

    sudo apt update

Then install the default package:

    sudo apt install mysql-server

#### - Configuring MySQL
<br />

Run the security script:

MySQL server package comes with a script called mysql_secure_installation that can perform several security-related operations.

Run the script by typing:

    sudo mysql_secure_installation

You will be asked to configure the VALIDATE PASSWORD PLUGIN which is used to test the strength of the MySQL users' passwords and improve the security. There are three levels of password validation policy, low, medium and strong. Press ENTER if you don’t want to set up the validate password plugin.

On the next prompt, you will be asked to set a password for the MySQL root user. Once you do that the script will also ask you to remove the anonymous user, restrict root user access to the local machine and remove the test database. You should answer “Y” (yes) to all questions.

