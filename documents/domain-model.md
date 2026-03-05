# Domain Model

## Entities

- `Customer`
- `Restaurant`
- `RestaurantCategory`
- `ShoppingCart`
- `RestaurantOrder`
- `FoodItem`
- `Discount`
- `PaymentMethods`

## Attributes and Operations

### `Customer`

- ID: string
- Name: string
- Email: string
- `addToFavorites(Restaurant.ID)`

### `Restaurant`

- ID: string
- Name: string
- Description: string
- Logo URL: string
- Address: string
- `searchMenuItems(string)`

### `RestaurantCategory`

- ID: string
- Name: string
- Description: string
- RestaurantID: string

### `RestaurantOrder`

- ID: string
- Name: string
- Description: string
- ShoppingCartID: string
- Status: string
- Review: string
- Rate: string

### `ShoppingCart`

- ID: string
- RestaurantID: string
- CustomerID: string
- Itens: FoodItem[] 
- Price: number

### `FoodItem`

- ID: string
- Name: string
- Description: string
- RestaurantID: string
- Extras: string[]
- Price: number
- Review: string
- Rate: string
