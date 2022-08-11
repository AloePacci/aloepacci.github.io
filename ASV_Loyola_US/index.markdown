---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
#This project is divided in 2 machines:

# [Rapberry Pi](./Raspberry/Raspi.html)
# [Jetson Xavier NX](./src/Xavier.html)
# [Server](./src/Server.html)

#You may also want to see

# [Quickstart](./quickstart.html)
# [Principle of operation](./funcionamiento.html)

layout: page
---
Welcome to ASV_Loyola_US project! 

I have worked in this project from 16-Dec-2021 to 31-jul-2022 last commit done by me [here](https://github.com/derpberk/ASV_Loyola_US/tree/83a195d2237af34dc4d31a91853105b321b2a84f)

Autonomous Surface Vehicles - Proyecto Universidad de Sevilla - Universidad Loyola

this package includes a ROS2 strategy transcode from a python based original aproach made by [Fede Peralta](https://github.com/FedePeralta)

The goal is to implement and deploy a float of Autonomous Surface Vehicles to monitorize enviromental areas.

You can find the original code in [ASV_Loyola_US](https://github.com/FedePeralta/ASV_Loyola_US)

And the ROS2 Code [ASV_Loyola_US](https://github.com/AloePacci/ASV_Loyola_US)

To have a first approach to the code check [First Steps in understanding the code](./src/Xavier.html)

![drone](./assets/ASV.jpeg)

You can also cheok our [Posts](./post.html) to check what was our test progression!

{% for post in paginator.posts %}
  <div class="post">
    <h1>{{ post.title }}</h1>
    {{ post.content }}
  </div>
{% endfor %}

<nav class="pagination">
  {% if paginator.previous_page %}
    <a href="{{ paginator.previous_page_path }}">Más nuevo</a>
  {% endif %}

  {% if paginator.next_page %}
    <a href="{{ paginator.next_page_path }}">Más antiguo</a>
  {% endif %}
</nav>