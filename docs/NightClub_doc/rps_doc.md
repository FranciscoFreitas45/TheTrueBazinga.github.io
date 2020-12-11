## Public Relations

List of all routes:
* [List all Public Relations](#List-All-Public-Relations)
* [Update Public Relation](#Update-Public-Relation)
* [Create new Public Relation](#Create-new-Public-Relation)
* [Delete Public Relation](#Delete-Public-Relation)

___

### List All Public Relations

* **GET https://nite-apigateway.herokuapp.com/nightClub/public-relations/** - List all Public Relations from one night club

Requires token in header (*Bearer token*) from employee or manager.


___


### Update Public Relation

* **PUT https://nite-apigateway.herokuapp.com/nightClub/public-relations/{id}** - Update a Public Relation

Requires token from manager.

```js
req.body = {
    pr_fullname: String,
    pr_shortcode: String,
    pr_phone: String,
    pr_email: String
}
```

___

### Create new Public Relation
* **POST https://nite-apigateway.herokuapp.com/nightClub/public-relations/** - Create new Public Relation

Requires token from manager.

```js
req.body = {
    pr_fullname: String,
    pr_shortcode: String,
    pr_phone: String,
    pr_email: String
}
```

___

### Delete Public Relation
* **DELETE https://nite-apigateway.herokuapp.com/nightClub/public-relations/{id}** - Deletes Public Relation

Requires token from manager