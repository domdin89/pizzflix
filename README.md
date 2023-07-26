### Create a virtual evironment

`python3 -m venv project_env`

### Check with ls that is created the folder

`ls`

### Activate virtual environment

`source project_env/bin/activate`

### Install requirements

`pip install -r requirements.txt`

### Start the project

`python3 manage.py runserver`


## All in one

```bash
python3 -m venv project_env && source project_env/bin/activate &&  pip install -r requirements.txt && python3 manage.py makemigrations && python3 manage.py migrate && python3 manage.py runserver
```

## ENV variables

### Db connection
| Parameter                 | Description                
| :--------------------     | :------------------------- 
| `DEBUG`                   | **Required** `True` -o- `False` 
| `SECRET_KEY`              | **Required** Your API key 
| `DB_ENGINE`               | **Required** `django.db.backends.mysql` 
| `DB_NAME`                 | **Required** `investivino` 
| `DB_USER`                 | **Required** `root` 
| `DB_PASSWORD`             | **Required** `password` 
| `DB_HOST`                 | **Required** `srv-captain--investivino2-db-db` 
| `DB_PORT`                 | **Required** `3306` 


### Django Secret Key
| Parameter                 | Description                
| :--------------------     | :------------------------- 
| `DJANGO_SECRET`                   | **Required** `YOUR DJANGO SECRET KEY` 


### S3 parameters
| Parameter                 | Description                
| :--------------------     | :------------------------- 
| `USE_S3`                  | **Required** `True` -o- `False`
| `AWS_ACCESS_KEY_ID`       | **Required** `SCW6M8PNVKP4SEZQYGS3` 
| `AWS_SECRET_ACCESS_KEY`   | **Required** `50d914ce-6805-4d83-91d3-ebc6fd4ad261` 

### Stripe parameters
| Parameter                 | Description                
| :--------------------     | :------------------------- 
| `STRIPE_PUBLIC_KEY`       | **Required** `pk_test_51MbnuwLNSi3DSbwly9BTmYlpbIBLPjHk005EHcOKlXEiUuyoH13QEOdfgZEFd0c5NnzMJlkYsEUikkPdFqujlqI5003rMeneyl`
| `STRIPE_SECRET_KEY`       | **Required** `sk_test_51MbnuwLNSi3DSbwlO7GihbG9PYpDy1PHn0CL7nxiCYxW7JUyoarCM5DzdMDGdTUuNy8ch7j59BKB0n0fUMWPDS0o00j5MVpce2`
| `STRIPE_WEBHOOK_SECRET`   | **Required** `whsec_a2p7yURYZ8lBsYEAld96M94Z9ZcN18LZ`
| `STRIPE_DEFAULT_CURRENCY` | `eur`

### Paypal parameters
| Parameter                         | Description                
| :--------------------             | :------------------------- 
| `PAYPAL_CLIENT_ID`                | **Required** `AdvH9io4569_jQt-c4wBxJD85SM4ujhSS1uvkrSgzIdhiO69SlTAZmcVIBlJXUzYQ3apJJ28WBFMCBmq`
| `PAYPAL_SECRET`                   | **Required** `ENwDJF-kn34uO8yg_V-MxQFr4gbKCYgrd_iCY6fmzR_KKnooB2JlDTIBwrZ4bYsoh7Nyh0-GTEgbbHAq`
| `PAYPAL_ACCESS_TOKEN`             | **Required** `A21AAKwFzvBhx4uG4CnQyn34iea3bVSLAzda4-4WMwKLhQw1hq9JlMqhX1VqydwjeFZK_aXZrMUFdSM8OJtxruL0eyLcVZZnw`
| `PAYPAL_CURRENCY`                 | `eur`

### Sendgrid parameters
| Parameter                         | Description                
| :--------------------             | :------------------------- 
| `EMAIL_BACKEND`                   | **Required** `sendgrid_backend.SendgridBackend`
| `SENDGRID_API_KEY`                | **Required** `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`
| `SENDGRID_SANDBOX_MODE_IN_DEBUG`  | **Required** `True` -o- `False`
| `EMAIL_SENDGRID`                  | **Required** `test@gmail.com`

## Authors

- [@domdin89](https://www.github.com/domdin89)
- [@cocco12892](https://www.github.com/cocco12892)