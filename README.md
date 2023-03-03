# AWS-EC2-Deployment
Deploying in a web back application in AWS EC2 Instance

# Illustration in a Django App
<img src="https://user-images.githubusercontent.com/50916200/222664035-2a1669ac-3409-4c2c-afe8-bc5e486d6add.png" width="90%" />


### Setup
Update the System
```bash
sudo apt-get update
```
To get this repository, run the following command inside your git enabled terminal
```bash
git clone https://github.com/repositorynamehere.git
```

Install the latest version of python3

```bash
sudo apt install python3-pip -y
```
You will need django to be installed in you computer to run this app. Head over to https://www.djangoproject.com/download/ for the download guide

Download django using pip
```bash
pip install django
```
Once you have downloaded django, go to the cloned repo directory and run the following command

```bash
python3 manage.py makemigrations
```

This will create all the migrations file (database migrations) required to run this App.

Now, to apply this migrations run the following command
```bash
python3 manage.py migrate
```

One last step and then our todo App will be live. We need to create an admin user to run this App. On the terminal, type the following command and provide username, password and email for the admin user
```bash
python3 manage.py createsuperuser
```

That was pretty simple, right? Now let's make the App live. We just need to start the server now and then we can start using our simple todo App. Start the server by following command

```bash
python3 manage.py runserver 0.0.0.0:8000
```

Once the server is hosted, head over to http://127.0.0.1:8000/portal for the App.

Cheers and Happy Coding :)
