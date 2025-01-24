``` mermaid 
erDiagram
          CUSTOMER }|..|{ DELIVERY-ADDRESS : has
          CUSTOMER ||--o{ ORDER : places
          CUSTOMER ||--o{ INVOICE : "liable for"
          DELIVERY-ADDRESS ||--o{ ORDER : receives
          INVOICE ||--|{ ORDER : covers
          ORDER ||--|{ ORDER-ITEM : includes
          Type-of-products-available||--|{ PRODUCT : contains
          PRODUCT ||--o{ ORDER-ITEM : "ordered in" 

```
This flowchart display the process when ordering from Nike. 
Once Nike receives the order, the pick the order item from it’s respective location based on the product type.
The customer places order from Nike they provide a delivery address to receive the order when the order is placed. 
When the customer receives the package it includes an invoice the covers what products were in the order. 
