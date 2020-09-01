# (more follow soon)

![IMG PREV](https://www.awesomescreenshot.com/upload/1417516/1457799/8a25a538-3cc9-43bf-4259-3f06aa6d59a6.png "Cards")

# Responsive and Inteligent
The Data For The Card's Is Stored In An Array Insided App.vue. Vue Will Then Create As Many Card's As There's Data. The Card's Only Show Until **sm** Breakpoint Is Triggered.

```javascript
 data() {
    return {
      Apartments: [
        {
          title: 'Manhattan Tower in NYC',
          img_link: 'https://images.unsplash.com/photo-1470219556762-1771e7f9427d?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1489&q=80',
          baths: 4,
          rooms: 8,
          size: 560,
          cost: 1250,
          per: 'Week',
          rating: 4,
          reviews: 256,
          description: 'The Presidio Residences on ...',
        },
        ....
     ]
```
# Card's are fully responsive and mobile ready

![IMG PREV](https://s3.amazonaws.com/awesomescreenshot/upload/1417516/1457799/10e1acef-3c58-4441-4e8e-f73881eea543.png?AWSAccessKeyId=AKIAJSCJQ2NM3XLFPVKA&Expires=1598948943&Signature=qdazsdnEiJiLADc0O5eTybNht%2Fo%3D "Title")
