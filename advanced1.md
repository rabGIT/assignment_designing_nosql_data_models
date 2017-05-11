Your eCommerce business needs to keep track of products and their prices. The products each belong to a department. The business needs to keep track of revenue as product prices change over time. The business also needs to keep track of receipts of transactions and the number of units each product has in stock.

product collection
{
  id: number
  name: string
  department
    {
      name: string
      manager: string
    }
  price: array
    {
      price: currency
      effectiveDate: datetime
    }
  quantity: number
}

receipts collection
{
  transaction id: number
  transaction date: datetime
  customer id: number
  items: array
    {
      product id: number
      quantity: number
    }
}

customer collection
{
  customer id: number
  address, etc. 
}
