---
layout: project
type: project
image: images/bitcoin (2).jpg
title: Crypto Calculator
permalink: projects/Crypto calculator
# All dates must be YYYY-MM-DD format!
date: 2019-07-01
labels:
  - Andorid
  - Java
  - Alpha Vantage API
summary: I begun developing this app for my friend who buys and sells cryto to people in Hawaii who dont have access to the exchanges. 
---

 <img class="" src="../images/cryptoPic1.jpg">


Crypto calculator gets data from an API called Alpha Vantage. This API has data for crypto as well as stocks. I manualy grabbed the data from the API and then use text fields and buttons to display the data and do conversions. An update to this app will implement json parsing to get the data. It uses a variety of currency types as well as crypto types that are availible through the API.

Grabbing data from API:
---

```java
@Override
public void onClick(View v) {
 final String cryptoType1 = cryptoType.getSelectedItem().toString();
 final String currencyType1 = currencyType.getSelectedItem().toString();
 final String URL = ("https://www.alphavantage.co" +
      "/query?function=CURRENCY_EXCHANGE_RATE" +
       "&from_currency=" + cryptoType1 +
        "&to_currency=" + currencyType1 + "&apikey=4YYBRNYMR141GDIL");
     String results = "";
                
     fetchData getData = new fetchData();           
      try {
          results = getData.execute(URL).get();
     
      } catch (ExecutionException e) {
          e.printStackTrace();
      } catch (InterruptedException e) {
           e.printStackTrace();
              }
                
         crypto.setText(results);
          Double currencyTotal = 0.00;
                
       if((cryptoAmount.getText().toString().length() > 0
               && dollarAmount.getText().toString().length() > 0)
               || (cryptoAmount.getText().toString().length() == 0
               && dollarAmount.getText().toString().length() == 0)) {
       Toast.makeText(MainActivity.this, "Use One Input", Toast.LENGTH_SHORT).show();
                }
                
       else if(cryptoAmount.getText().toString().length() > 0) {
             dollarAmount.setText("");
             currencyTotal = Double.parseDouble(results) * Double.parseDouble(cryptoAmount.getText().toString());
                }

       else if(dollarAmount.getText().toString().length() > 0) {
             cryptoAmount.setText("");
             currencyTotal = Double.parseDouble(dollarAmount.getText().toString()) / Double.parseDouble(results);
                }
                
           total.setText(currencyTotal.toString());
                
                
            }
        });
    }
}
```

[Alpha Vantage](https://www.alphavantage.co/), [Git Repository](https://github.com/derekasola/Crypto-Calculator)




