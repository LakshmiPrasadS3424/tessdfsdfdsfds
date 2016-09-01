---
title: Using arrays in your emails
categories:
- email
- design
layout: articles
---

# Using arrays in your email
    
Vero allows you to refer to properties stored against a customer using the Liquid templating language, these are commonly referred to as merge tags:
`{{ user.first_name }}`

Likewise, if you track a property with an event, you can reference it with:
`{{ event.product_name }}`

However there are many cases where you will want to use complex data, such as an array of products, in your outgoing emails.

## Passing the array 
If you were to track the following:

  <script>
  _veroq.push(['track',{ products: [ {name: 'Item 123', price: 10},  {name: 'Item ABC', price: 20} ] }]);  
  </script>
 
You could referrnce the array in your email using [Liquid templating](https://github.com/Shopify/liquid/wiki/Liquid-for-Designers) as follows:

  {% raw %}
    {% for product in event.products %}
      {{product.name}}: ${{product.price}}
    {% endfor %}
  {% endraw %}
 
**Note**: that you can store arrays as both customer and event-level properties.
         
        
                
                
