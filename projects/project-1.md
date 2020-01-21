---
layout: project
type: project
image: images/crypto pic.jfif
title: Crypto calculator
permalink: projects/Crypto calculator
# All dates must be YYYY-MM-DD format!
date: 2019-07-01
labels:
  - Andorid
  - Java
summary: I begun developeing this app for m friend who buys and sells cryto to people in hawaii that dont have access to the exchanges.
---

<div class="ui small rounded images">
  
</div>

Crypto calculator gets data from an API called vantage alpha. this API has data for crypto as well as stocks. i used json parsing to retrive the data from the API and then use text fields and buttons to display the data and do conversions.

```js
byte ADCRead(byte ch)
{
    word value;
    ADC1SC1 = ch;
    while (ADC1SC1_COCO != 1)
    {   // wait until ADC conversion is completed   
    }
    return ADC1RL;  // lower 8-bit value out of 10-bit data from the ADC
}
```





