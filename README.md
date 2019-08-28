# Test-Driven Development with Python

Provisioning
1. Assume we have a user account and home folder
2. add-apt-repository ppa:fkrull/deadsnakes
3. apt-get install nginx git python3.6 python3.6-venv
4. Add Nginx config for virtual host
5. Add Systemd job for Gunicorn
Deployment
1. Create directory structure in ~/sites
2. Pull down source code into folder named source
3. Start virtualenv in ../virtualenv
4. pip install -r requirements.txt
5. manage.py migrate for database
6. collectstatic for static files
7. Set DEBUG = False and ALLOWED_HOSTS in settings.py
8. Restart Gunicorn job
9. Run FTs to check everything works
