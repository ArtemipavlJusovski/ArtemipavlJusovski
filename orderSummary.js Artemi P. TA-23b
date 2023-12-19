var tellimus = {
  "id": 2113,
  "orderNumber": "E210126001",
  "createdAt": "2021-01-26 16:04:24",
  "clientName": "Kalle Tali",
  "deliveryType": "Omniva smartpost",
  "deliveryValue": 178,
  "rows": [
    {
      "article_id": 31,
      "name": "Kohvimasin De'Longhi Dolce Gusto Piccolo EDG100.W",
      "product_code": "257549",
      "price": 49.1666666667,
      "amount": 1,
      "vat": 0.2
    },
    {
      "article_id": 23420,
      "name": "Kohvikapslid Nescafe Dolce Gusto Espresso Intenso, 128 g, 16 tk",
      "product_code": "355836",
      "price": 5.0666666667,
      "amount": 2,
      "vat": 0.2
    },
    {
      "article_id": 23421,
      "name": "Kohvikapslid Nescafe Dolce Gusto Latte Macchiato, 194 g, 16 tk",
      "product_code": "000000000501267301",
      "price": 5.825,
      "amount": 1,
      "vat": 0.2
    }
  ]
};

// Function to calculate amount with VAT
function calculateAmountWithVAT(price, quantity, vat) {
  const amountWithoutVAT = price * quantity;
  const amountWithVAT = amountWithoutVAT * (1 + vat);
  return amountWithVAT;
}

let totalAmount = 0;

// Iterate through each item in the order
tellimus.rows.forEach(item => {
  // Extract item details
  const { name, quantity, price, vat } = item;

  // Calculate the amount for the item with VAT
  const amount = calculateAmountWithVAT(price, quantity, vat);

  // Add the amount to the total
  totalAmount += amount;

  // Print details for each item
  console.log(`Name: ${name}`);
  console.log(`Quantity: ${quantity}`);
  console.log(`Price: ${price}€`);
  console.log(`Amount: ${amount.toFixed(2)}€\n`);
});

// Print the total amount of the order
console.log(`Total Amount: ${totalAmount.toFixed(2)}€`);
