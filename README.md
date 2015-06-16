# Create-Django-project

If you use fish in fish config add function.

    function start-django-app
        git clone https://github.com/we3x/Create-Django-Project $argv
        cd $argv
        echo $argv > provision/roles/common/nameOfProject.txt
        vagrant up --provision 
    end
