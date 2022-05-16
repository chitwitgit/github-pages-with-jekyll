# Introduction
In this project, our team will create and manage a repository on Github, starting with setting up a workflow and organizing the project flow. Then, we declare ourselves as contributors and add some personal information to this file. After making sure every team member has added their own .md file and input the respective information, we add some C code to our repository, get a status badge and finally adding our page link to the course public repository for TA checking.

# Code

# Contributors

{% for students in site.student %}
    <p> >> <img src="{{student.image}}" width="100" height="100">
        @<a href="https://github.com/{{student.user}}">{{student.user}}</a> 
        ({{student.name}}) </p>
    <p> &emsp; >> {{student.content | markdownify}}
{% endfor %}
