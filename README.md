[![CircleCI](https://circleci.com/gh/sirjmkitavi/cp2-bucketlist/tree/develop.svg?style=svg)](https://circleci.com/gh/sirjmkitavi/cp2-bucketlist/tree/develop)
[![Coverage Status](https://coveralls.io/repos/github/sirjmkitavi/cp2-bucketlist/badge.svg?branch=develop&update=1)](https://coveralls.io/github/sirjmkitavi/cp2-bucketlist?branch=develop)
[![Issue Count](https://codeclimate.com/github/sirjmkitavi/cp2-bucketlist/badges/issue_count.svg)](https://codeclimate.com/github/sirjmkitavi/cp2-bucketlist)

#BucketList Application API

## Introduction

> This application is a Flask API for a bucket list service that allows users to create, update and delete bucket lists. It also provides programmatic access to the items added to the items created. This API is a REST API and the return format for all endpoints is JSON.

## Endpoints

1. `POST /auth/login`
2. `POST /auth/register`
3. `GET /bucketlists/`: returns a listing of all buckets
4. `GET /bucketlists/<bucketlist_id>`: returns the bucket list with the specified ID
5. `PUT /bucketlist/<bucketlist_id>`: updates the specified bucket list
6. `DELETE /bucketlist/<bucketlist_id>`: deletes a bucket list based on the specified ID
7. `POST /bucketlists/<bucketlist_id>/items/`: adds a new item to the specified bucket list
8. `PUT /bucketlists/<bucketlist_id>/items/<item_id>`: updates an item in the specified bucket list
9. `DELETE /bucketlists/<bucketlist_id>/items/<item_id>`: deletes an item from the specified bucket list

## Installation & Setup
1. Ensure your python enviroment is setup properly
2. clone the repository
3. Install the requiremnts ```pip install -r requirements.txt```

## Perform migrations
```sh
python server.py db init
python server.py db migrate
python server.py db upgrade
```

## Testing
To run the tests for the app, and see the coverage, run
```
nosetests --with-coverage
```
