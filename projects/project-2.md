---
layout: project
type: project
image: images/japanese (2).jpg
title: Japanese Notecard
permalink: projects/Japanese Notecard
# All dates must be YYYY-MM-DD format!
date: 2019-10-15
labels:
  - Android
  - java
summary: A quiz app to help me study Japanese.
---


<img class="ui medium right floated rounded image" src="../images/jap2.jpg">

This app was begun after my first semester of Japanese 101 fall 2019 during winter break. It uses images of hiragana, katakana, and will eventually kanji to be displayed. It detects left and right swipes to control the pictures and the text View values. I plan to add words, sentences, and even pronunciation with google translate.

Example of swipe commands:
---

```Java
 public void onSwipeRight() {  
                i -= 1;

                if (i < 0) {
                    i = 45;
                }

                String textView = (String) romanjiArray.getText(i);
                romangi.setText(textView);

                Drawable drawable = imgs.getDrawable(i);
                image.setImageDrawable(drawable);
            }

            public void onSwipeLeft() {
                i += 1;
                if (i > 45) {
                    i = 0;
                }

                String textView = (String) romanjiArray.getText(i);
                romangi.setText((CharSequence) textView);

                Drawable drawable = imgs.getDrawable(i);
                image.setImageDrawable(drawable);  
            }
```

[Git Repository](https://github.com/derekasola/Jappanese-App)
