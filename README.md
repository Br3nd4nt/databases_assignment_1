## Пользователи 
### User - покупатель
#### Поля
- email
- passwordHash
- preferedpaymentType
- address
#### Методы
- CreateOrder (List[Dish]) => Order
- ViewAllOrders() => List[Order]

### Restaurant - ресторан
#### Поля
- email
- passwordHash
- allAvailableDishes - List[Dish]
- allDeliveryManHired - List[Delivery]
#### Методы
- addNewDish (Dish)
### Delivery - доставщик
#### Поля
- email
- passwordHash
- currentOrder
#### Методы
- MarkOrderasdelivered()
- GetCurrentOrder() => Order

## Dish
- price
- listofIngredientsAndNutritions

## Order
- customer - User
- allDishes - List[Dish]
- orderStatus - {Accepted, Cooking, Delivering, Delivered, Canceled}

