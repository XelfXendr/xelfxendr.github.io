---
layout: page
title: Pesterfox
description: A client/server chat app written in Java using JavaFX and PostgreSQL
img: assets/img/pesterfox_background.jpg
importance: 1
category: work
---

In this project, I created a simple chat application called Pesterfox. 
The project is split into two parts: the client application and the server.
Both parts are written in Java. 

To create the GUI of the client application, I used JavaFX.
The server uses a PostgreSQL database to store the user data and the messages.
The communication between the client and the server is done using the [KryoNet](https://github.com/EsotericSoftware/kryonet) library.

Upon starting the client application, the user first connects to a server by its IP address and port.
They may then log in or register a new account. The passwords are stored in the database as salted hashes.

<div class="row justify-content-sm-center">
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/pesterfox1.png" title="Pesterfox login screen" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The login screen of Pesterfox.
</div>

Upon successful login, the user can select a chat room they are a member of, join a chat room or create a new one.
All rooms are inherently treated as group chats, but the user can also create a private room with another user.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/pesterfox2.png" title="Pesterfox chat window" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    A chat room.
</div>

The code for this project is available on our university's [GitLab](https://gitlab.mff.cuni.cz/bronecja/pesterfox).
