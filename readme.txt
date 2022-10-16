au démarrage
1. pip install -r requirements.txt 
2. python3 manage.py init_local_dev 
3. python3 manage.py migrate
4. python3 manage.py runserver

#création d'un user

python3 manage.py shell
from django.contrib.auth import get_user_model
UserModel = get_user_model()
user = UserModel.objects.create_user('user-oc', password='password-oc')