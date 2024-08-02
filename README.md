# **E-Sales web**

| Name and Lastname | Email | GitHub account |
| --- | --- | --- |
| Maria Amparo Alami Mochi | ma.alami.2020@alumnos.urjc.es | MaAlami2020 |

#### Team coordination zone: [Jira](https://webapp1.atlassian.net/jira/software/projects/SCRUM/boards/1)

# Main aspects of the web application

## **1. Entities**
- user: attribute -> name, email, password, image
- producto: attribute -> name, price
- shopping cart: attribute -> item
- order: attribute -> paying (accepted/denied, debit/credit)

**RELATION ->** an user purchases a product that is added to a shopping cart; and after confirming and paying for it, the user can track the generated order.

## **2. User permissions**

#### Permissions framework: [Miró](https://miro.com/app/board/uXjVKum1Mlo=/)

Anonymous user permissions

1. register in the application
2. access the app without registering
3. be shown the available products loaded by the manager
4. be shown a graphic with the most popular products
5. search products

![anonymous_perm](/images/anonymous_user.PNG)

Registered user permissions

1. delete the account and all its information from the app
2. log in the application
3. edit personal info
4. access the app without registering
5. be shown the available products loaded by the manager
6. search for products
7. view a graph with product recommendations based on purchase history
8. view purchase history
9. modify registration data
10. add products to cart
11. modify the quantity of an item
12. remove the item from the cart
13. save an item for later
14. view the available quantity of an item product when there are 5 or less
15. View the status of an order among 3 available -> confirmed, on the way, delivered
16. confirm the products in the car
17. be redirected to the payment screen where credit card data will be entered
18. pay with one of the credit card saved in the app
19. save a credit card for future payments

![registered_perm](/images/registered_user.PNG)

Administrator user permissions

1. register/unsubscribe a product in the app
2. manage product stock (number of units of an item visible to users)
3. display a graph with the best-selling products according to type (skirt, t-shirt,...), color, size (large, medium, small)
4. register as an manager with a specific password in a configuration file (encrypted)
5. validate an order
6. view the quantity of a product in time real

![administrator_perm](/images/administrator_user.PNG)

## **3. Images**
| Entity | Image |
| --- | --- |
| User | profile photo |
| Product | product image |
| Shopping cart | product image |

## **4. Graphics**
| Type of graphic | Info |
| --- | --- |
| bars | the most popular products |
| bars | product recommendations |
| bars | sales by product type |
| bars | sales by size |

## **5. Complementary technology**
- generate PDF of an order

## **6. Algorithm or advanced query**
- random products
- recommendate products
- see the amount of a product in real time
- sales by an attribute (type of product, size) of a product