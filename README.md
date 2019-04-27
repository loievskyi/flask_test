# flask_test
## Flask-based application with two endpoints. It's work in a Linux and use Redis as temporary storage.
Flask-based application with two endpoints that will work in a Linux environment using Redis as temporary storage.
1. /add_new_list - for adding new list from post data into db (redis for now),
2. /show_lists - for show all lists


## How to install:
1. Install python, pip, virtualenv
2. Create virtualenv and activate it
3. Clone repository (git clone https://github.com/bakutake/flask_test.git)
4. Open it's folder in console (cd path/to/project/flask_test)
4. Install packages from requirements (pip3 install -r requirements.txt)
5. Run application (python3 items_list.py)


## How to use it:
### example requert using curl:
- for add list: curl --header "Content-Type: application/json" --request POST --data '{"new_item":["xxx", "xxx", "xxx"]}' http://localhost:8080/add_new_list/
- for get lists: curl --header "Content-Type: application/json" --request GET http://localhost:8080/show_lists/


## Note
#### You can send json data only using double quotes (not single quotes).
