# Project Name: Hotel Integrate Technologies API - [HITA]

### 1. Core Features:
--------------------
	##### Key functionalities  support:
	
		* Hotel Data Management (CRUD operations for hotels, rooms, amenities, pricing).
		* Data Standardization (normalize hotel names, addresses, amenities).
		* ID Mapping (map internal hotel IDs to external systems like Expedia, Booking.com).
		* Search & Filtering (search hotels by location, amenities, price range).
		* Data Export/Distribution (export data in formats like JSON/XML for partners).
		* Authentication & Rate Limiting (secure API access).


### 2. Set Up Django Project & Database
-----------------------------------------------------------------------------------------------------------------------------------
	Step 1.1: Create and Activate Pipenv Environment
		```sh
			1. mkdir hita
			2. cd hita
			3. pipenv install django mysqlclient django-rest-framework django-filter drf-yasg
			4. pipenv shell 
		```

	Step 1.2: Verify Installed Packages
		Ensure Pipfile includes:
		```sh
			[packages]
			django = "*"
			mysqlclient = "*"
			djangorestframework = "*"
			django-filter = "*"
			drf-yasg = "*"
		```
	
	Step 2.1: Start Django Project:

		```sh
			django-admin startproject hita .
		```

	Step 2.2: Update 'hita/settings.py' file:
		```sh
				DATABASES = {
			'default': {
				'ENGINE': 'django.db.backends.mysql',
				'NAME': 'ittster_contents',
				'USER': 'itt_coents',
				'PASSWORD': 'baa98569745',
				'HOST': 'ls-2606205faee891e.c1m8so4gsag3.ap-southeast-1.rds.amazonaws.com',
				'PORT': '3306',
			}
		}
		
				INSTALLED_APPS = [
			...
			'rest_framework',
			'drf_yasg',
			'hotels',  
		]
		```














