# ecommerce-app

# results
uploaded in json file
./ecom_app/apis.json

Initialize app

# unpack folder
tar -zxvf ecommerce-app.zip
cd ecommerce-app.zip

# create environment
virtualenv env
source env/bin/activate

# migrate to sqlite db
python manage.py migrate

# populate data
python manage.py populate_data

# run local server 
python manage.py runserver
